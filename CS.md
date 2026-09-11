Worked for 8s

Yes — this image is a very useful reference, but it contains far more material than you need at the beginning. If we apply the Pareto principle (80/20) aggressively, I would not follow the entire roadmap.

Your goal is not to become someone who knows a little about 200 cybersecurity topics.

Your goal is to become someone who can say:

> “I understand networks, operating systems, security fundamentals, and can investigate a security incident in a lab.”



Then get the certifications that prove the foundation.

Cisco's current CCNA covers network fundamentals, network access, IP connectivity, IP services, security fundamentals, and automation/programmability. 

And ISC2's current entry-level CC covers security principles, governance, IAM, network/cloud security, and security operations/incident response. 

So here's the Pareto version I would build specifically for YOU.

🛡️ Junaid's 80/20 Cybersecurity Roadmap

YOUR CURRENT POSITION
                           │
             BCA + Wipro Trust & Safety
                           │
                           ▼
                 ┌─────────────────┐
                 │ 1. NETWORKING   │
                 └────────┬────────┘
                          │
                        CCNA 🏆
                          │
                          ▼
                 ┌─────────────────┐
                 │ 2. LINUX       │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ 3. SECURITY     │
                 │    FUNDAMENTALS │
                 └────────┬────────┘
                          │
                       Security+
                          │
                          ▼
                 ┌─────────────────┐
                 │ 4. WINDOWS +    │
                 │    AD + LOGS    │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ 5. SOC / SIEM   │
                 │    INVESTIGATION│
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ 6. PORTFOLIO    │
                 │    + PROJECTS   │
                 └────────┬────────┘
                          │
                          ▼
                  🎯 SOC ANALYST L1
                          │
              ┌───────────┼───────────┐
              ▼           ▼           ▼
          Blue Team    Cloud       Pentest

That's the core.


---

🥇 TIER 1 — Networking

Priority: 10/10

This is your first major objective.

Don't try to learn everything in that image.

Focus on these:

Networking 80/20

Must know:

OSI model

TCP/IP model

Ethernet

MAC addresses

IP addresses

IPv4

Subnetting ⭐⭐⭐

IPv6 basics

ARP

ICMP

TCP vs UDP

Ports

DNS

DHCP

NAT

Routing

Switching

VLANs

Trunking

STP

ACLs

OSPF

Basic network security


Tools

Cisco Packet Tracer

and later:

Wireshark

Achievement

🏆 CCNA

Cisco's current CCNA is the 200-301 exam, 120 minutes, with no prerequisite; Cisco currently lists network fundamentals, network access, IP connectivity, IP services, security fundamentals and automation/programmability as the exam areas. 

Why CCNA is important for YOU

Because cybersecurity without networking becomes:

> “I know security terminology.”



Networking gives you:

> “I understand what is actually happening on the network.”



That's a huge difference.


---

🥈 TIER 2 — Linux

Priority: 9/10

Your image contains an enormous Linux section.

Ignore 80% of it initially.

Master:

Filesystem
Users
Groups
Permissions
Processes
Services
SSH
Networking
Logs
Bash
Package management

Commands

You should become comfortable with:

ls
cd
pwd
cat
less
grep
find
chmod
chown
ps
top
kill
systemctl
ip
ss
ping
curl
wget
ssh

Achievement

🏆 Linux Security Lab

Example:

> Ubuntu server → users → permissions → SSH → logs → failed login investigation.



You don't need a Linux certification immediately.

Skill > certificate here.


---

🥉 TIER 3 — Security Fundamentals

Priority: 10/10

This is where the image becomes enormous.

We reduce it to the concepts that actually matter.

Learn these deeply

Security principles

CIA Triad

Authentication

Authorization

Accounting

Least privilege

Defense in depth

Zero Trust


Threats

Malware

Phishing

Credential attacks

Brute force

MITM

DoS/DDoS

Social engineering

Insider threats


Network security

Firewall

IDS

IPS

VPN

Proxy

Segmentation

NAC


Cryptography

Understand the difference between:

Hashing
Encryption
Encoding
Digital signatures
Certificates
PKI

Identity

IAM

MFA

RBAC

Privileged accounts

Access control


Incident response

Preparation
↓
Detection
↓
Analysis
↓
Containment
↓
Eradication
↓
Recovery
↓
Lessons learned


---

🏆 Achievement — Security+

This becomes your second major certification.

I'd prioritize:

CCNA → Security+

rather than collecting five beginner certifications.


---

What about ISC2 CC?

The ISC2 Certified in Cybersecurity (CC) is legitimate and specifically designed for people entering cybersecurity; ISC2 says there is no work-experience requirement. 

But here's my Pareto judgment:

If money/time are limited:

Skip CC and go toward Security+.

If you want a quick entry-level cybersecurity credential:

CC can be useful.

It isn't a bad certification. It's just that CCNA + Security+ gives you a stronger overall foundation for your particular path.

Also, ISC2 updated the CC exam outline effective September 1, 2026, so if you pursue it, use the current exam material rather than old courses. 


---

🟦 TIER 4 — Windows + Active Directory

This is one area I'd add strongly to the image's roadmap for your SOC Analyst goal.

Priority: 9/10

Learn:

Windows

Users

Groups

Services

Processes

Event Viewer

Windows Defender

PowerShell basics

Windows networking

Security logs


Active Directory

Understand:

Domain
Domain Controller
Users
Groups
Organizational Units
Group Policy
Kerberos
LDAP
NTLM
DNS

You don't need to become an AD administrator.

You need to understand how attacks and investigations work in an enterprise Windows environment.


---

🟨 TIER 5 — SOC / SIEM

Priority: 10/10

This is where your existing professional background becomes particularly useful.

Your resume already demonstrates investigation support, risk assessment, abuse detection, trend analysis, and high-volume analytical decision-making. 

Now we add actual cybersecurity investigation skills.

Learn:

SOC

Alert

Event

Incident

IOC

TTP

False positive

Escalation

Severity

Incident triage


Logs

Learn to investigate:

Windows Event Logs
Linux logs
Authentication logs
Firewall logs
DNS logs
Web logs

SIEM

Learn one properly.

I'd start with:

Microsoft Sentinel OR Splunk

Don't learn five SIEMs simultaneously.


---

🔎 TIER 6 — Wireshark + Nmap

Priority: 9/10

These two tools give you enormous practical value.

Wireshark

Learn to answer:

> "What actually happened on the network?"



Understand:

Source IP
Destination IP
Protocol
Port
DNS
TCP handshake
HTTP/HTTPS
Packets
Sessions

Nmap

Learn:

Host discovery
Port scanning
Service detection
Basic enumeration

Only against systems you own or are explicitly authorized to test.


---

🧪 TIER 7 — Projects

This is where I want you to beat the certificate-collector problem.

You need perhaps 4 excellent projects, not 25 mediocre ones.

Project 1 — Network Investigation

Packet Tracer + Wireshark

Build a network.

Capture traffic.

Analyze it.

Produce:

Network diagram
Packet captures
Observations
Findings
Troubleshooting report


---

Project 2 — Linux Security Investigation

Create a Linux lab.

Generate controlled failed SSH logins.

Investigate:

Source IP
Username
Timestamp
Number of attempts
Pattern

Write an incident report.


---

Project 3 — SOC Investigation

Build a small SIEM lab.

Generate security events.

Investigate:

Alert
↓
Evidence
↓
Timeline
↓
IOC
↓
Analysis
↓
Severity
↓
Response recommendation

This is extremely valuable for your target role.


---

Project 4 — Phishing Investigation

Create a simulated phishing case.

Analyze:

Sender
Domain
URL
Headers
Attachments
Indicators
User impact
Recommended response

Again: controlled/educational environment only.


---

🐍 TIER 8 — Programming

The image includes Python, Go, JavaScript, C++, Bash, PowerShell, etc.

Don't do that.

That's exactly where Pareto saves you.

For cybersecurity:

Learn:

Python + Bash + PowerShell basics

That's enough initially.

You already have JavaScript experience, so you don't need to spend months relearning programming from scratch.

Python focus

files
strings
regex
JSON
HTTP requests
APIs
CSV
log parsing
automation

Your goal isn't:

> Become a software engineer.



Your goal is:

> Automate repetitive security work.




---

☁️ TIER 9 — Cloud

Priority: 7/10 initially

Don't start here.

After your networking/security foundation, learn:

Cloud fundamentals

IAM

VPC/VNet

Security groups

Network ACLs

Encryption

Logging

Monitoring

Storage security

Secrets

Identity


Then choose:

AWS OR Azure

Not both initially.

Certification

Later, one cloud certification can be useful.

But don't let cloud distract you from CCNA + Security+ + SOC skills.


---

🚫 What I would NOT prioritize initially

This is where the Pareto principle becomes really powerful.

The image contains:

CEH

CISSP

CISM

CRISC

OSCP

GPEN

GWAPT

GCIH

CCSP

CASP+

CISA

etc.


You don't need these now.

Especially don't chase CISSP yet.

CISSP is a later-career certification, not your first cybersecurity milestone.

Don't chase OSCP yet.

OSCP becomes meaningful after you have strong fundamentals and you know you actually want offensive security.

Don't chase CEH just because it says "ethical hacking."

There are better uses of your early learning time.


---

🎯 Your REAL 20%

If I had to cut everything in that huge image down to 10 things, I'd give you:

Priority	Skill	Why

🥇	Networking	Foundation of cybersecurity
🥈	Linux	Core security environment
🥉	Security fundamentals	Understand attacks/defenses
4	Windows	Enterprise environment
5	Active Directory	Critical enterprise knowledge
6	Wireshark	Network investigation
7	SIEM	SOC job skill
8	Incident response	Core analyst capability
9	Python/Bash/PowerShell	Automation
10	Cloud/IAM	Modern enterprise security


And the certification side:

CERTIFICATIONS

                       CCNA
                        🏆
                        │
                        ▼
                    Security+
                        🏆
                        │
                        ▼
              Choose specialization
                        │
              ┌─────────┼─────────┐
              ▼         ▼         ▼
           CySA+     Cloud      Pentest


---

🏆 Your "Best of the Best" Achievement Ladder

I would make these your milestones:

LEVEL 1 — Foundation

☐ Networking fundamentals
☐ Linux fundamentals
☐ Windows fundamentals
☐ Security fundamentals

LEVEL 2 — International certifications

🏆 CCNA

🏆 CompTIA Security+

LEVEL 3 — Practical capability

🏆 Wireshark investigation project
🏆 Linux security investigation
🏆 Windows/AD investigation
🏆 SIEM investigation

LEVEL 4 — Portfolio

🏆 GitHub cybersecurity portfolio
🏆 4 polished security projects
🏆 Incident reports
🏆 Network diagrams
🏆 Detection queries/rules

LEVEL 5 — Job

🎯 SOC Analyst L1
🎯 Security Analyst
🎯 Junior Cybersecurity Analyst

LEVEL 6 — Specialization

Then choose ONE:

🛡️ Blue Team / SOC
☁️ Cloud Security
🔴 Pentesting
🔍 DFIR
🎯 Threat Hunting


---

📅 Your first 12 months — Pareto edition

I'd structure your time approximately like this:

Months 1–3

NETWORKING

TCP/IP
OSI
IPv4
Subnetting
Switching
VLAN
Routing
OSPF
ACL
NAT
DNS
DHCP


Packet Tracer labs

↓

🏆 CCNA


---

Months 4–5

LINUX + WINDOWS

Linux
Bash
Windows
PowerShell
Logs
Processes
Services
Permissions
SSH


---

Months 5–7

SECURITY

CIA
IAM
Cryptography
Network Security
Threats
Vulnerabilities
Risk
Incident Response

↓

🏆 Security+


---

Months 7–9

SOC

Wireshark
Nmap
Windows logs
Linux logs
SIEM
IOC
MITRE ATT&CK
Alert triage
Incident investigation


---

Months 9–11

PROJECTS

Build the four projects.


---

Months 11–12

CAREER

Cybersecurity resume
LinkedIn
GitHub
SOC interview preparation
Networking
Applications

And start applying.

Do not wait until you have 10 certifications before applying.


---

⭐ And there's one thing I'd specifically exploit from YOUR background

Your existing Wipro experience is not something I want you to hide.

You already work in a high-volume environment involving platform safety, policy enforcement, risk assessment, abuse detection, investigation support and trend analysis. 

Your AI experience also includes dataset validation, model testing/evaluation and ethical AI evaluation. 

Eventually, your career story could become:

> BCA → Trust & Safety / AI platform operations → Networking + Security → SOC Analyst → Security Operations / AI Security



That's much stronger than pretending you started your career as a cybersecurity professional.

And because you already have experience around an AI platform, AI security / AI abuse / AI platform security could eventually become an interesting specialization for you.


---

🔥 Final Pareto rule for you

Whenever you see another giant cybersecurity roadmap, ask:

> "Will this skill help me understand networks, operating systems, security, detection, investigation, or automation?"



If yes → prioritize it.

If maybe → later.

If no → ignore it for now.

Your first major target is therefore crystal clear:

🎯 CCNA → Linux → Security+ → Windows/AD → Wireshark/Nmap → SIEM → 4 Projects → SOC Analyst

Not:

> 50 courses → 20 certificates → still no practical experience.



That's the difference between learning cybersecurity and building a cybersecurity career.

Confidence: High. The roadmap is intentionally narrower than the image because your goal is maximum career return per hour and per rupee, not maximum topic coverage. Cisco confirms the current CCNA scope, while ISC2 confirms its CC is an entry-level credential; I would treat the latter as optional rather than adding it automatically. 