# 🚀 Complete Video-Based Cybersecurity Learning Roadmap

> **Target Career Path:** SOC Analyst L1 → Security Analyst → Cybersecurity Specialist → International Cybersecurity Specialist  
> **Background:** BCA | Trust & Safety Experience | Wipro | Google/Gemini Project Experience  
> **Target Certifications:** CompTIA Security+ (SY0-701) → CompTIA CySA+ (CS0-003) → SC-200 / BTL1

---

## 🎯 Career & Certification Strategy (Highest ROI Path)


[Phase 1: Core Foundation]  -->  [Phase 2: Blue Team & Hands-On]  -->  [Phase 3: Advanced Specialization]
CompTIA Security+                    CompTIA CySA+                            BTL1 / SC-200 / AWS Security
(Establishes Baseline)               (SOC & Alert Triage Focus)                  (Cloud & SOC Specialization)

1. **CompTIA Security+ (SY0-701):** Primary Target #1. Establishes core security knowledge, network defense concepts, and threat vectors. Globally recognized for entry-level SOC roles.
2. **CompTIA CySA+ (CS0-003):** Primary Target #2. Deeply relevant for SOC L1/L2. Covers threat detection, log analysis, SIEM tools, and incident response.
3. **Microsoft SC-200 (SOC Analyst) or BTL1 (Blue Team Level 1):** Practical, hands-on portfolio builders for SIEM (Sentinel) and incident triage.

---

# Phase 1: Core IT & Networking Infrastructure

## 🛡️ Section 1 — IT Fundamentals

### Computer Hardware & Operating Systems
**Priority:** 🔥 MUST LEARN

* **What to Learn:** CPU execution cycles, RAM volatile storage vs. persistent disk storage, BIOS/UEFI boot sequences, NICs, MAC physical addressing vs. IP logical addressing. Operating system architecture: filesystems (NTFS, ext4), processes, background services, user management, and DAC permissions.
* **🎥 Recommended Video:** Search YouTube for `"CompTIA A+ Core 1 Full Course" by NetworkChuck` or `"Computer Hardware & OS Fundamentals" by freeCodeCamp`.
* **Level:** Beginner
* **Notes to Take:**
  * Difference between volatile memory (RAM) and non-volatile storage (SSD/HDD).
  * UEFI Secure Boot process and why it prevents rootkits.
  * Difference between User Space and Kernel Space.
* **Practice:** Open Windows Task Manager (`taskmgr`) and Linux `top`/`htop`. Identify process IDs (PID), memory consumption, and parent-child process trees.
* **Lab:** Create a local virtual machine (VMware Workstation Player or VirtualBox) and install Ubuntu Desktop from an ISO.
* **Achievement:** Can explain how an OS boots from BIOS/UEFI to Kernel load, and identify running processes via CLI on both Windows and Linux without documentation.
* **Interview Questions:**
  1. *What is the difference between physical MAC addressing and logical IP addressing?*
  2. *What happens at the hardware/OS level during a cold boot?*
  3. *How does Kernel Mode differ from User Mode in modern operating systems?*
* **Cert Relevance:** CompTIA A+, CompTIA Security+, SOC Interviews.

---

## 🌐 Section 2 — Networking Fundamentals & Addressing

### Network Devices & Topology Architecture
**Priority:** 🔥 MUST LEARN

* **What to Learn:** Roles of Switches (L2), Routers (L3), Firewalls (L3/L7), Access Points, Modems, Gateways, and Load Balancers. Difference between Hubs (collision domain broadcasting) and Switches (micro-segmentation via MAC tables).
* **🎥 Recommended Video:** Search YouTube for `"Network Devices Explained" by Practical Networking` or `"CCNA 200-301 - Day 1" by Jeremy's IT Lab`.
* **Level:** Beginner to Intermediate
* **Notes to Take:**
  * Define Broadcast Domain vs. Collision Domain.
  * Draw how a packet moves through: `Host A -> L2 Switch -> Default Gateway (Router) -> Firewall -> Internet`.
* **Practice:** Draw a standard corporate office network layout showing where the L2 switches, L3 edge router, perimeter firewall, and internal servers sit.
* **Achievement:** Able to explain packet movement across L2 switches and L3 routers without hesitation.
* **Interview Questions:**
  1. *At which OSI layer does a managed switch operate vs. a router?*
  2. *What is a default gateway, and what happens if it is misconfigured on an endpoint?*

---

### OSI & TCP/IP Models
**Priority:** 🔥 MUST LEARN

* **What to Learn:** The 7 layers of the OSI model (Physical, Data Link, Network, Transport, Session, Presentation, Application) vs. the 4 layers of the TCP/IP model. Encapsulation (Data -> Segment -> Packet -> Frame -> Bits) and Decapsulation.
* **🎥 Recommended Video:** Search YouTube for `"OSI Model Explained" by Practical Networking`.
* **Level:** Beginner
* **Notes to Take:**
  * Layer 2 PDU = Frame (MAC headers).
  * Layer 3 PDU = Packet (IP headers).
  * Layer 4 PDU = Segment (TCP/UDP headers).
* **Practice:** Capture a basic web request in Wireshark and identify the header layers corresponding to OSI Layers 2, 3, 4, and 7.
* **Achievement:** Can list all 7 OSI layers, their corresponding Protocol Data Units (PDUs), and primary protocols operating at each layer.
* **Interview Questions:**
  1. *Explain the encapsulation process as data moves down the OSI model.*
  2. *Which layer does TLS/SSL operate on?*

---

### Subnetting (IPv4 & CIDR)
**Priority:** 🔥 MUST LEARN

* **What to Learn:** Binary to decimal conversion, Subnet Masks, CIDR notation (`/24`, `/26`, `/30`), calculating Network ID, Broadcast Address, Usable Host Range, Number of Hosts ($2^H - 2$), and Variable Length Subnet Masking (VLSM).

#### Subnetting Reference & Cheat Sheet

| CIDR | Subnet Mask | Total IPs | Usable Hosts | Use Case |
|---|---|---|---|---|
| `/24` | `255.255.255.0` | 256 | 254 | Standard User Subnet |
| `/26` | `255.255.255.192` | 64 | 62 | Small Department / DMZ |
| `/28` | `255.255.255.240` | 16 | 14 | Management / Server Pod |
| `/30` | `255.255.255.252` | 4 | 2 | Point-to-Point Router Link |

* **🎥 Recommended Video:** Search YouTube for `"Subnetting Masterclass" by Practical Networking` or `"Subnetting Made Easy" by Professor Messer`.
* **Level:** Intermediate
* **Notes to Take:**
  * Formula for hosts: $2^{(32 - \text{CIDR})} - 2$.
  * Block size formula: $256 - \text{Interesting Octet Subnet Mask}$.
* **Practice Exercises:**
  1. Convert `192.168.1.135/27` to binary. Identify Network Address, Broadcast Address, and First/Last usable IPs.
  2. Subnet `10.0.0.0/16` into subnets supporting at least 100 hosts each. What is the new CIDR mask?
  3. Given IP `172.16.50.40` with mask `255.255.240.0`, find the network ID.
* **Achievement:** Able to solve any `/24` through `/30` subnetting problem mentally or on paper within 60 seconds.
* **Interview Questions:**
  1. *Why are two IP addresses subtracted when calculating usable hosts in a subnet?*
  2. *What is the network address and broadcast address for `192.168.10.45/28`?*
* **Cert Relevance:** CCNA, Security+, SOC Interviews.

---

## 🔌 Section 3 — Network Protocols

### Protocol Analysis Grid

| Protocol | Default Port | Transport | Purpose | Security Risk / Vulnerability |
|---|---|---|---|---|
| **ARP** | N/A (L2) | N/A | Resolves IP to MAC address | Susceptible to ARP Spoofing / Poisoning (MITM) |
| **DNS** | 53 | UDP / TCP | Resolves Domain names to IP addresses | DNS Spoofing, Cache Poisoning, DNS Tunneling for Data Exfiltration |
| **DHCP** | 67/68 | UDP | Dynamically assigns IP configurations | DHCP Starvation attacks, Rogue DHCP servers |
| **HTTP / HTTPS** | 80 / 443 | TCP | Web traffic transmission | HTTP sends plaintext; HTTPS uses TLS to encrypt traffic |
| **SSH** | 22 | TCP | Encrypted command-line management | Brute force attacks, compromised SSH keys |
| **Telnet** | 23 | TCP | Unencrypted remote CLI management | Cleartext password transmission |
| **SMTP / IMAP** | 25 / 143 | TCP | Mail routing and retrieval | Phishing, spoofed senders (lacks SPF/DKIM/DMARC by default) |
| **Kerberos** | 88 | UDP/TCP | Active Directory authentication | Kerberoasting, Golden Ticket, AS-REP Roasting |
| **LDAP / LDAPS**| 389 / 636 | TCP | Directory query protocol | Plaintext authentication queries over 389 |
| **SMB** | 445 | TCP | Network file sharing | Remote Code Execution (e.g., EternalBlue / WannaCry) |

* **🎥 Recommended Video:** Search YouTube for `"Network Protocols Explained"` by *NetworkChuck* or *IBM Technology*.
* **Practice:** Open Wireshark, run `nslookup google.com`, and inspect the DNS Query/Response packet structure. Locate the Transaction ID and Flags.
* **Achievement:** Can recite key ports, underlying transport layer, function, and attack vectors for the top 15 infrastructure protocols.

---

## 🔀 Section 4 & 5 — Switching & Routing (Cisco Packet Tracer Focus)

### Core Switching & Routing Concepts
**Priority:** 🔥 MUST LEARN (Switching) / ⭐ HIGH PRIORITY (Routing)

* **What to Learn:** Ethernet Frame headers, MAC address table population mechanics, 802.1Q VLAN tagging, Access vs. Trunk links, Spanning Tree Protocol (STP) loop prevention, BPDU Guard, Port Security, Static Routing, Default Routes, and Router-on-a-Stick Inter-VLAN routing.


+---------------------------------------------+
|           Cisco Router (Gateway)            |
|               Gig0/0.10 & .20               |
+----------------------+----------------------+
| 802.1Q Trunk Link
+----------------------+----------------------+
|           L2 Managed Switch                 |
+-----------+---------------------+-----------+
| Access (VLAN 10)    | Access (VLAN 20)
+-----------+---------+   +-------+-----------+
|   User PC (VLAN 10) |   | Server (VLAN 20)  |
|    192.168.10.10    |   |   192.168.20.10   |
+---------------------+   +-------------------+

* **🎥 Recommended Video:** Search YouTube for `"Cisco Packet Tracer Lab Tutorial"` or `"VLANs and Trunks"` by *Jeremy's IT Lab*.
* **Lab Exercise (Packet Tracer):**
  1. Build the topology shown above with 1 Router, 1 Switch, and 2 PCs.
  2. Configure VLAN 10 (Sales) and VLAN 20 (HR) on the switch.
  3. Assign switch ports as Access ports for respective VLANs.
  4. Configure a 802.1Q Trunk port connecting Switch to Router.
  5. Configure sub-interfaces on Router (`Gig0/0.10` and `Gig0/0.20`) for Inter-VLAN routing.
  6. Enable **Port Security** on PC-facing ports: limit MAC addresses to 1, set violation mode to `restrict` or `shutdown`.
* **Achievement:** Able to configure Inter-VLAN routing and Port Security from scratch in Cisco Packet Tracer without referencing CLI syntax guides.

---

# Phase 2: System Administration & Defensive Architecture

## 🐧 Section 7 — Linux Administration for Defenders

### Command Line Mastery & Forensic Basics
**Priority:** 🔥 MUST LEARN

* **What to Learn:** Linux FHS (Filesystem Hierarchy Standard: `/etc`, `/var/log`, `/proc`, `/home`, `/root`), User/Group management, UNIX File Permissions (`chmod` octal/symbolic, `chown`), Systemd service management (`systemctl`), process listing, and log analysis (`journalctl`, `grep`, `awk`, `sed`).

```bash
# Essential Defensive Linux Commands Reference

# View active listening ports and connected sockets with process names
ss -tulpn

# Search for failed SSH login attempts in real-time
grep "Failed password" /var/log/auth.log | tail -n 20

# Find files modified in the last 24 hours with SUID bit set
find / -perm -4000 -mtime -1 2>/dev/null

# Filter out non-comment lines from configuration files
grep -v "^#" /etc/ssh/sshd_config | grep -v "^$"

 * 🎥 Recommended Video: Search YouTube for "Linux for Cybersecurity" by The Cyber Mentor or "Linux Terminal Basics" by freeCodeCamp.
 * Practice: Set up an SSH service on your Linux VM. Modify SSH config (/etc/ssh/sshd_config) to disable root login and change default port 22 to 2222. Restart service and verify with ss -tulpn.
 * Achievement: Can parse system logs using pipe chains (cat, grep, awk, sort, uniq -c) to identify brute-force login attacks.
 * Interview Questions:
   * What does permission 755 vs 644 mean on a Linux file?
   * Where are system logs located on systemd-based Linux distributions, and how do you view authentication attempts?
🪟 Section 8 & 9 — Windows & Active Directory (AD) Environment
Active Directory Architecture & Defensive Monitoring
Priority: 🔥 MUST LEARN
 * What to Learn: Active Directory Domain Services (AD DS), Domain Controllers (DC), OUs, Security Groups, Group Policy Objects (GPO), Kerberos vs. NTLM authentication, Domain Trusts, and core Windows Event IDs for security monitoring.
High-Value Windows Security Event IDs for SOC Analysts
| Event ID | Event Description | SOC Triage Significance |
|---|---|---|
| 4624 | Successful Account Logon | Track user activity and logon types (Type 2=Interactive, Type 3=Network, Type 10=RDP). |
| 4625 | Failed Account Logon | Primary indicator for password spraying, brute-force attacks, or credential stuffing. |
| 4672 | Special Privileges Assigned | Indicates explicit administrator-level access logon. |
| 4688 | New Process Created | Crucial for process execution tracking (Cmd execution, PowerShell launching suspicious scripts). |
| 4720 | User Account Created | Persistence detection; alerts when unauthorized accounts are added. |
| 4768 / 4769 | Kerberos TGT Requested / Service Ticket Requested | Ticket requests analysis (Kerberoasting / AS-REP Roasting indicators). |
 * 🎥 Recommended Video: Search YouTube for "Active Directory Basics for Beginners" by TCM Security or IBM Technology.
 * Lab Setup: Set up a local home lab using VirtualBox/VMware:
   * Install Windows Server (Evaluation ISO).
   * Promote server to a Domain Controller (Active Directory Domain Services role).
   * Create a Domain (e.g., corp.local), add Organizational Units (OUs), and create domain users.
   * Join a Windows 10/11 VM to the domain and test logging in with domain user credentials.
 * Achievement: Understand Kerberos authentication flow (AS-REQ, AS-REP, TGS-REQ, TGS-REP) and can locate failed/successful authentication logs in Windows Event Viewer (eventvwr.msc).
Phase 3: SOC Analyst Core Skills & Security Operations
🚨 Section 10, 14 & 15 — Cybersecurity Fundamentals, IR & SOC Operations
Incident Response Lifecycle (NIST SP 800-61 Rev. 2)
Priority: 🔥 MUST LEARN
  +-------------------+      +-------------------+      +-------------------+
  |  1. Preparation   | ---> | 2. Detection &    | ---> | 3. Containment,   |
  |                   |      |    Analysis       |      | Eradication & Rec.|
  +-------------------+      +-------------------+      +---------+---------+
                                                                  |
                             +-------------------+                |
                             | 4. Post-Incident  | <--------------+
                             |    Activity       |
                             +-------------------+

 * What to Learn:
   * CIA Triad: Confidentiality, Integrity, Availability.
   * Least Privilege & Defense in Depth: Applying multi-layered security controls (Physical, Network, Host, Application, Data).
   * Alert Triage: Differentiating True Positives (TP), False Positives (FP), True Negatives (TN), and False Negatives (FN).
   * Indicators of Compromise (IOCs): Hashes (MD5/SHA256), IP addresses, Domain names, File paths, Registry keys.
   * Tactics, Techniques, and Procedures (TTPs): Behavioral patterns mapped to attacker frameworks.
 * 🎥 Recommended Video: Search YouTube for "SOC Analyst Training / Incident Response Lifecycle" by SOC101, Cybersecurity Meg, or TCM Security.
 * Practice: Write a standard operating procedure (SOP) for an L1 SOC Analyst handling a suspicious email attachment alert. Define initial triage, scoping, containment steps, and escalation triggers.
 * Achievement: Can explain the complete NIST incident response framework and detail step-by-step triage actions for a suspected malware infection.
📈 Section 16 — SIEM & Log Analysis (Splunk & Sentinel)
Hands-On SIEM Operations
Priority: 🔥 MUST LEARN
 * What to Learn: Log ingestion, normalization, correlation rules, search queries, dashboards, and alert generation. Focus on Splunk (SPL) or Microsoft Sentinel (KQL).
// Microsoft Sentinel (KQL) Sample Query: Detecting Potential Password Spraying
SecurityEvent
| where EventID == 4625
| summarize FailedCount = count() by TargetUserName, IpAddress, bin(TimeGenerated, 5m)
| where FailedCount > 10
| project TimeGenerated, TargetUserName, IpAddress, FailedCount
| sort by FailedCount desc

# Splunk Search Processing Language (SPL) Sample Query: Failed Logins by IP
index=windows EventCode=4625 
| stats count by TargetUserName, Source_Network_Address 
| where count > 10 
| sort - count

 * 🎥 Recommended Video: Search YouTube for "Splunk Tutorial for Beginners" by NetworkChuck or "Microsoft Sentinel KQL Tutorial" by Microsoft Security / Cyber Insecurity.
 * Lab: Sign up for a free TryHackMe account and complete the "Splunk Basics" or "Microsoft Sentinel" rooms.
 * Achievement: Can write basic SPL/KQL queries to filter logs by Event ID, summarize count by source IP, and isolate suspicious activity.
 * Interview Questions:
   * What is the difference between a SIEM and a Log Aggregator?
   * How do you tune a SIEM correlation rule to reduce False Positives?
🦈 Section 17 — Network Traffic Analysis (Wireshark)
Deep Packet Inspection
Priority: 🔥 MUST LEARN
 * What to Learn: Packet capture syntax, display filters, protocol breakdown, TCP 3-way handshake analysis (SYN -> SYN-ACK -> ACK), identifying cleartext credentials, following TCP/HTTP streams, and detecting anomalies (port scans, beaconing).
Key Wireshark Display Filters for Triage
# Show all HTTP POST requests (often contains logins or data exfiltration)
http.request.method == "POST"

# Filter for SYN packets with ACK bit not set (Port Scan indicator)
tcp.flags.syn == 1 and tcp.flags.ack == 0

# Filter DNS queries for non-existent domains (Potential C2 beaconing/DGA)
dns.flags.rcode == 3

# Display traffic for a specific IP address
ip.addr == 192.168.1.50

 * 🎥 Recommended Video: Search YouTube for "Wireshark Tutorial for Beginners" by Chris Greer (Wireshark Certified Network Analyst).
 * Practice: Download sample PCAP files from Malware Traffic Analysis (malware-traffic-analysis.net) or Wireshark sample captures. Extract an executable file delivered over unencrypted HTTP.
 * Achievement: Can analyze a PCAP file in Wireshark, reconstruct a user session via TCP Stream, and pinpoint malicious network activity.
🔎 Section 18 & 19 — Vulnerability Assessment & Nmap
Network Enumeration & Vulnerability Management
Priority: 🔥 MUST LEARN (Nmap) / ⭐ HIGH PRIORITY (Vulnerability Scanning)
 * What to Learn: TCP SYN Stealth Scan (-sS), TCP Connect Scan (-sT), UDP Scan (-sU), Service Version Detection (-sV), OS Detection (-O), Aggressive Scan (-A), Nmap Scripting Engine (NSE) (--script). Vulnerability lifecycle: Identification, Prioritization (CVSS v3 score metrics), Remediation, Verification.
# Nmap Scanning Command Reference

# Quick SYN scan for top 100 ports with version detection
nmap -sS -sV --top-ports 100 192.168.1.10 -oN quick_scan.txt

# Full comprehensive scan: All ports, service detection, default OS scripts
nmap -p- -sV -sC -O -T4 192.168.1.10 -oA full_capture

# Scan for specific vulnerability using NSE scripts (e.g., SMB vulnerabilities)
nmap --script smb-vuln* -p 445 192.168.1.10

 * 🎥 Recommended Video: Search YouTube for "Nmap Tutorial for Beginners" by NetworkChuck or David Bombal.
 * Lab: Run Nmap scans against legal target scanme.nmap.org or local VMs installed via Metasploitable2.
 * Achievement: Understand differences between TCP SYN and Connect scans, execute targeted Nmap commands safely, and interpret output reports.
Phase 4: Threat Intelligence, Frameworks & Advanced Topics
🕵️ Section 20 & 21 — Threat Intelligence & MITRE ATT&CK Framework
Adversary Mapping & TTPs
Priority: 🔥 MUST LEARN
 * What to Learn: MITRE ATT&CK Matrix structure: Tactics (The "Why" - e.g., Initial Access, Execution, Persistence) vs. Techniques (The "How" - e.g., Phishing, PowerShell) vs. Sub-techniques and Procedures. Cyber Kill Chain phases. Threat intelligence consumption (STIX/TAXII standards, VirusTotal, AbuseIPDB).
   [Tactics: What is the adversary trying to achieve?]
   ├── Initial Access (TA0001)
   ├── Execution (TA0002)
   ├── Persistence (TA0003)
   └── Credential Access (TA0006)
          │
          └── [Technique: How do they accomplish it?]
              └── T1110 - Brute Force
                     │
                     └── [Sub-Technique: Specific Implementation]
                         ├── T1110.001 - Password Guessing
                         └── T1110.003 - Password Spraying

 * 🎥 Recommended Video: Search YouTube for "MITRE ATT&CK Framework Explained" by IBM Technology or TCM Security.
 * Practice: Take a public threat intelligence report (e.g., Mandiant or CISA advisory) and map the listed adversary behavior to specific MITRE ATT&CK Tactic and Technique IDs.
 * Achievement: Able to explain how to use MITRE ATT&CK to correlate disparate SIEM alerts into a unified threat campaign story.
🐍 Section 26 — Python & Scripting for Automation
Python for Security Analysts
Priority: ⭐ HIGH PRIORITY
 * What to Learn: Basic data types, file I/O (reading log files), regular expressions (re module) for extracting IP addresses/hashes, querying REST APIs using requests (e.g., querying VirusTotal API for file hash reputation).
import re
import requests

# Python Script: Extract IP Addresses from a Log File and Verify via API
def extract_and_check_ips(log_file_path):
    ip_pattern = r'\b(?:[0-9]{1,3}\.){3}[0-9]{1,3}\b'
    
    with open(log_file_path, 'r') as file:
        log_data = file.read()
        
    found_ips = set(re.findall(ip_pattern, log_data))
    print(f"[+] Found {len(found_ips)} unique IP addresses in log file.")
    
    for ip in found_ips:
        # Example check against AbuseIPDB or local blocklist logic
        print(f"[-] Inspecting IP: {ip}")

if __name__ == "__main__":
    # Replace with path to actual sample log file
    extract_and_check_ips("sample_auth.log")

 * 🎥 Recommended Video: Search YouTube for "Python for Cybersecurity" by freeCodeCamp or Automate the Boring Stuff with Python.
 * Practice: Write a script that parses a web server access log file, counts the requests per IP, and flags any IP making more than 100 requests per minute.
 * Achievement: Can write functional Python scripts to automate repetitive log parsing tasks.
Phase 5: Practical Portfolio Projects
These 3 core portfolio projects are tailored for your resume to demonstrate hands-on SOC L1 capability.
+---------------------------------------------------------------------------------+
|                            PRACTICAL SOC PROJECTS                               |
+---------------------------------------------------------------------------------+
|  Project 1: Home-Lab SIEM (Splunk / Elastic) Ingestion & Detection Engine       |
|  Project 2: Phishing Analysis & Malware Triage Pipeline                         |
|  Project 3: PCAP Incident Investigation & Wireshark Forensic Analysis           |
+---------------------------------------------------------------------------------+

Project 1: Home-Lab SIEM (Splunk/Sentinel) & Detection Engine
 * Objective: Build a functional cloud/local SIEM environment, ingest Windows/Linux logs, generate telemetry via simulated attacks, and write custom detection rules.
 * Architecture: Windows 10 Endpoint VM + Ubuntu VM running Splunk Enterprise or connected to Microsoft Sentinel.
 * Tools: VirtualBox/VMware, Windows Event Forwarding / Splunk Universal Forwarder, Atomic Red Team.
 * Steps:
   * Install Splunk Enterprise (Free trial/Developer license) on Ubuntu VM or set up a free Azure trial for Microsoft Sentinel.
   * Install Splunk Universal Forwarder on Windows 10 VM; configure it to forward Application, System, and Security logs.
   * Enable Sysmon (System Monitor) on Windows VM for advanced process tracking (Event ID 1: Process Creation).
   * Execute simulated attacks using Atomic Red Team scripts (e.g., running PowerShell encoded commands or adding a local admin user).
   * Build custom SIEM alerts for: Process Execution from AppData directory and Account Creation (Event ID 4720).
 * Resume Bullet: Designed and deployed a Splunk SIEM home lab ingesting Windows Security and Sysmon logs; authored custom SPL correlation rules detecting malicious credential dumping and unauthorized user creation.
Project 2: Phishing Analysis & Malware Triage Pipeline
 * Objective: Analyze raw .eml/.msg phishing emails, extract metadata and headers, inspect malicious attachments safely, and correlate IOCs.
 * Tools: EML Analyzer, MXToolbox Email Header Analyzer, CyberChef, Hybrid-Analysis / VirusTotal, Any.Run.
 * Steps:
   * Obtain safe phishing samples from PhishTool or downloadable public phishing repositories.
   * Parse email headers to verify SPF, DKIM, and DMARC alignment status and trace origin IP hops.
   * Extract obfuscated URLs or malicious scripts from email body; decode using CyberChef (Base64/URL decoding).
   * Submit extracted file hashes or domain IOCs to VirusTotal and AbuseIPDB.
   * Write a comprehensive Incident Triage Report detailing findings, risk severity rating, and suggested blocklist actions.
 * Resume Bullet: Analyzed raw email artifacts and headers to evaluate SPF/DKIM validation status; utilized CyberChef and sandbox environments to isolate obfuscated payloads and extract actionable IOCs.
Project 3: PCAP Incident Investigation & Wireshark Forensic Analysis
 * Objective: Perform network forensic analysis on an enterprise network compromise capture to reconstruct the attack timeline.
 * Tools: Wireshark, NetworkMiner, TShark.
 * Steps:
   * Download an incident capture file from Malware Traffic Analysis.
   * Filter network traffic to identify the initial infection vector (e.g., malicious ZIP file downloaded over HTTP).
   * Track Command and Control (C2) beaconing behavior by isolating repeating outbound connections to suspicious IP addresses/ports.
   * Reconstruct DNS queries to identify domain generation algorithms (DGA) used by malware.
   * Document a full attack chronology report: Initial Access -> Payload Download -> Internal Enumeration -> C2 Beaconing.
 * Resume Bullet: Conducted deep packet inspection using Wireshark on PCAP data captures; reconstructed multi-stage attack timelines and identified C2 beaconing patterns.
📊 SOC Readiness Progress Tracker
| Topic / Section | Priority | Core Skill Focus | Video Watched | Practice Complete | Lab Complete | Interview Ready |
|---|---|---|---|---|---|---|
| Hardware & OS | 🔥 | Process Trees, Services, Permissions | ⬜ | ⬜ | ⬜ | ⬜ |
| Networking & OSI | 🔥 | Encapsulation, PDU, Device Roles | ⬜ | ⬜ | ⬜ | ⬜ |
| Subnetting | 🔥 | CIDR, Host Ranges, VLSM | ⬜ | ⬜ | ⬜ | ⬜ |
| Network Protocols | 🔥 | Ports, Security Risks, DNS/DHCP | ⬜ | ⬜ | ⬜ | ⬜ |
| Switching & Routing | ⭐ | VLANs, Trunks, Port Security | ⬜ | ⬜ | ⬜ | ⬜ |
| Linux Administration | 🔥 | Commands, Permissions, Log Parsing | ⬜ | ⬜ | ⬜ | ⬜ |
| Windows & AD | 🔥 | Event IDs, Kerberos, Domain Controllers | ⬜ | ⬜ | ⬜ | ⬜ |
| Incident Response | 🔥 | NIST Framework, Triage, SOPs | ⬜ | ⬜ | ⬜ | ⬜ |
| SIEM Operations | 🔥 | SPL / KQL Queries, Alert Tuning | ⬜ | ⬜ | ⬜ | ⬜ |
| Wireshark Analysis | 🔥 | Packet Filtering, Stream Following | ⬜ | ⬜ | ⬜ | ⬜ |
| Nmap & Scanning | 🔥 | Port Scans, Version Detection, NSE | ⬜ | ⬜ | ⬜ | ⬜ |
| Threat Intel / MITRE | 🔥 | TTP Mapping, Cyber Kill Chain | ⬜ | ⬜ | ⬜ | ⬜ |
| Python Scripting | ⭐ | Regex, File Parsing, API Requests | ⬜ | ⬜ | ⬜ | ⬜ |

