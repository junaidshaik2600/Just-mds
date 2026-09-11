# 🛡️ Junaid's 80/20 Cybersecurity Career Roadmap

## 🎯 Career Goal

**Current Position:**
> Trust & Safety Associate — Wipro / Google Gemini Project

⬇️

**First Cybersecurity Target:**
> SOC Analyst / Security Analyst — L1

⬇️

**Long-Term Target:**
> Security Analyst → Incident Response / Threat Hunting / Cloud Security / Detection Engineering

⬇️

**International Career Goal:**
> Build globally recognized certifications + practical cybersecurity experience + a strong portfolio.

---

# 🧭 THE CORE ROADMAP

```text
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


---

🥇 TIER 1 — NETWORKING

Priority: 10/10

Networking is the first major objective.

Learn — Networking 80/20

Networking Fundamentals

OSI Model

TCP/IP Model

Ethernet

MAC Addresses

IP Addresses

IPv4

Subnetting ⭐⭐⭐

IPv6 Basics

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

Basic Network Security


Tools

Cisco Packet Tracer

Wireshark


Practical Labs

Build networks in Cisco Packet Tracer.

Example:

PC1 ──┐
      │
PC2 ── Switch ── Router ── Server
      │
PC3 ──┘

Practice troubleshooting:

Incorrect IP address

Incorrect subnet mask

Missing default gateway

VLAN problems

Trunk problems

Routing problems

DNS problems

ACL problems


🏆 Achievement #1 — CCNA

Cisco Certified Network Associate (CCNA)

Goal

> Pass CCNA on the first attempt.



Preparation Method

Learn
  ↓
Understand
  ↓
Practice
  ↓
Packet Tracer Labs
  ↓
Troubleshooting
  ↓
Practice Questions
  ↓
Mock Exams
  ↓
CCNA Exam 🏆

Important: Do not book the exam until you can consistently perform well on practice exams and explain networking concepts without memorization.


---

🥈 TIER 2 — LINUX

Priority: 9/10

Do not try to learn every Linux topic.

Focus on the 80/20 fundamentals.

Learn

Linux Filesystem

Users

Groups

Permissions

Processes

Services

SSH

Networking

Logs

Bash

Package Management


Commands

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

🧪 Practical Project

Linux Security Investigation Lab

Build an Ubuntu server.

Practice:

Creating users

Creating groups

Configuring permissions

Configuring SSH

Monitoring services

Reviewing logs

Investigating failed login attempts


🏆 Achievement #2

> Build and document a Linux security lab.



Priority: Skill > Certification

Do not immediately spend money on a Linux certification.


---

🥉 TIER 3 — CYBERSECURITY FUNDAMENTALS

Priority: 10/10

Security Principles

Learn:

CIA Triad

Authentication

Authorization

Accounting

Least Privilege

Defense in Depth

Zero Trust

Security Controls


Threats

Learn:

Malware

Phishing

Credential Attacks

Brute Force

MITM

DoS/DDoS

Social Engineering

Insider Threats


Network Security

Learn:

Firewall

IDS

IPS

VPN

Proxy

Network Segmentation

NAC


Cryptography

Understand the difference between:

Hashing
Encryption
Encoding
Digital Signatures
Certificates
PKI

Identity & Access Management

Learn:

IAM

MFA

RBAC

Privileged Accounts

Access Control

Least Privilege


Incident Response

Understand:

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
Lessons Learned


---

🏆 Achievement #3 — CompTIA Security+

After building networking + Linux + security fundamentals:

> CompTIA Security+



Goal

Use Security+ to validate your broad cybersecurity foundation.

Recommended Sequence

CCNA
  ↓
Linux
  ↓
Security Fundamentals
  ↓
Security+


---

🟦 TIER 4 — WINDOWS + ACTIVE DIRECTORY

Priority: 9/10

This is extremely important for SOC Analyst work because many enterprise environments use Windows.

Windows Fundamentals

Learn:

Users

Groups

Services

Processes

Event Viewer

Windows Defender

PowerShell Basics

Windows Networking

Security Logs


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


Goal

You do not need to become a Windows/AD administrator.

You need to understand:

> How enterprise Windows environments work and how security analysts investigate suspicious activity within them.




---

🟨 TIER 5 — SOC / SIEM

Priority: 10/10

This is where your Trust & Safety experience can become particularly valuable.

Learn SOC Fundamentals

Alert

Event

Incident

IOC

TTP

False Positive

Escalation

Severity

Incident Triage

Threat Detection

Incident Investigation


Learn Logs

Windows

Windows Event Logs

Authentication Logs

Security Logs


Linux

Authentication Logs

System Logs

Application Logs


Network

Firewall Logs

DNS Logs

Web Logs

Network Traffic


SIEM

Learn one SIEM properly.

Recommended starting options:

Microsoft Sentinel

Splunk


Do not try to master five SIEM platforms at the same time.


---

🔎 TIER 6 — WIRESHARK + NMAP

Priority: 9/10

Wireshark

Goal:

> Understand what actually happened on a network.



Learn to identify:

Source IP
Destination IP
Protocol
Port
DNS Requests
TCP Handshake
HTTP/HTTPS
Packets
Sessions

Project

Perform a controlled network traffic investigation.

Produce:

Network Diagram
Packet Capture
Traffic Analysis
Findings
Investigation Report


---

Nmap

Learn:

Host Discovery

Port Scanning

Service Detection

Basic Enumeration


Only scan systems you own or have explicit authorization to test.


---

🧪 TIER 7 — CYBERSECURITY PROJECTS

Priority: 10/10

Do not build 25 weak projects.

Build 4 excellent projects.


---

🏆 Project 1 — Network Traffic Investigation

Tools

Cisco Packet Tracer

Wireshark


Build

A small network.

Investigate

IP addresses

Protocols

Ports

DNS

TCP connections

Network behavior


Deliverables

Network Diagram
Packet Capture
Analysis
Findings
Troubleshooting Report


---

🏆 Project 2 — Linux Security Investigation

Build

Linux security lab.

Simulate

Controlled failed SSH login attempts.

Investigate

Source IP
Username
Timestamp
Number of Attempts
Attack Pattern

Deliverables

Incident Summary
Evidence
Timeline
Investigation
Findings
Recommended Response


---

🏆 Project 3 — SOC / SIEM Investigation

Build

A small SIEM lab.

Generate

Controlled security events.

Investigate

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
Response Recommendation

Deliverables

Detection rule/query

Investigation notes

Timeline

Incident report

Recommended response



---

🏆 Project 4 — Phishing Investigation

Create a controlled phishing investigation.

Analyze:

Sender
Domain
URL
Email Headers
Attachments
Indicators
User Impact
Recommended Response

Create a professional incident report.


---

🐍 TIER 8 — PROGRAMMING FOR CYBERSECURITY

Priority: 7/10

Do NOT try to learn:

Go

C++

Rust

Java

JavaScript

Python

Bash

PowerShell


all at once.

You already have JavaScript experience.

For cybersecurity, prioritize:

Python

Learn:

Files
Strings
Regex
JSON
HTTP Requests
APIs
CSV
Log Parsing
Automation

Bash

Learn basic Linux automation.

PowerShell

Learn basic Windows automation and investigation.

Goal

Not:

> Become a software engineer.



Instead:

> Automate repetitive cybersecurity tasks.




---

☁️ TIER 9 — CLOUD SECURITY

Priority: 7/10 initially

Do this AFTER networking + Linux + Security+ fundamentals.

Learn

IAM

VPC/VNet

Security Groups

Network ACLs

Encryption

Logging

Monitoring

Storage Security

Secrets

Identity


Then choose:

AWS
OR
Azure

Do not learn both deeply at the beginning.


---

🚫 THINGS TO DELAY

Do not chase every certification shown on large cybersecurity roadmaps.

Delay:

CEH

CISSP

CISM

CRISC

OSCP

GPEN

GWAPT

GCIH

CCSP

CISA

CASP+

Other advanced certifications


Especially:

❌ CISSP — Not Yet

Save it for later in your career when you have the required professional experience.

❌ OSCP — Not Yet

Only pursue it after you have strong:

Networking

Linux

Web security

Enumeration

Active Directory

Pentesting fundamentals


and you've decided that offensive security is actually your direction.

❌ Certificate Collection

Avoid:

20 courses
10 certificates
0 projects
0 practical experience

Instead:

2–3 strong certifications
+
4 strong projects
+
Hands-on labs
+
Real work experience


---

🎯 THE 80/20 TOP 10

If everything became overwhelming, reduce the entire roadmap to these 10 skills:

Priority	Skill	Importance

1	Networking	⭐⭐⭐⭐⭐
2	Linux	⭐⭐⭐⭐⭐
3	Security Fundamentals	⭐⭐⭐⭐⭐
4	Windows	⭐⭐⭐⭐⭐
5	Active Directory	⭐⭐⭐⭐
6	Wireshark	⭐⭐⭐⭐
7	SIEM	⭐⭐⭐⭐⭐
8	Incident Response	⭐⭐⭐⭐⭐
9	Python/Bash/PowerShell	⭐⭐⭐⭐
10	Cloud/IAM	⭐⭐⭐⭐



---

🏆 CERTIFICATION ROADMAP

Stage 1

🏆 CCNA

Purpose:

> Validate networking knowledge.




---

Stage 2

🏆 CompTIA Security+

Purpose:

> Validate broad cybersecurity fundamentals.




---

Stage 3

Choose ONE specialization.

🛡️ Blue Team / SOC

Possible path:

Security+
   ↓
SOC
   ↓
CySA+
   ↓
Incident Response
   ↓
Threat Hunting

☁️ Cloud Security

Security+
   ↓
Cloud Fundamentals
   ↓
AWS/Azure
   ↓
Cloud Security

🔴 Pentesting

Security+
   ↓
Linux
   ↓
Web Security
   ↓
Active Directory
   ↓
Pentesting
   ↓
eJPT / PNPT
   ↓
OSCP

Do not choose your specialization until you have built the foundation.


---

🗺️ COMPLETE ACHIEVEMENT LADDER

LEVEL 1 — Foundation

[ ] Networking Fundamentals

[ ] Linux Fundamentals

[ ] Windows Fundamentals

[ ] Security Fundamentals

[ ] Build Cybersecurity Home Lab



---

LEVEL 2 — International Certifications

[ ] 🏆 CCNA

[ ] 🏆 CompTIA Security+


Optional:

[ ] ISC2 Certified in Cybersecurity (CC)



---

LEVEL 3 — Practical Skills

[ ] Wireshark Investigation

[ ] Nmap Lab

[ ] Linux Security Investigation

[ ] Windows/AD Investigation

[ ] SIEM Investigation

[ ] Incident Response Practice



---

LEVEL 4 — Portfolio

[ ] GitHub Cybersecurity Portfolio

[ ] 4 High-Quality Projects

[ ] Network Diagrams

[ ] Packet Captures

[ ] Detection Queries

[ ] Incident Reports

[ ] Investigation Timelines



---

LEVEL 5 — Career

Target:

[ ] SOC Analyst L1

[ ] Junior Security Analyst

[ ] Cybersecurity Analyst

[ ] Security Operations Analyst



---

LEVEL 6 — Specialization

Choose ONE:

[ ] 🛡️ Blue Team / SOC

[ ] 🔍 Incident Response

[ ] 🎯 Threat Hunting

[ ] ☁️ Cloud Security

[ ] 🔴 Pentesting

[ ] 🕵️ DFIR

[ ] 🤖 AI Security



---

📅 12-MONTH PARETO PLAN

Months 1–3

NETWORKING

Focus:

TCP/IP
OSI
IPv4
Subnetting
Switching
VLANs
Routing
OSPF
ACLs
NAT
DNS
DHCP


Cisco Packet Tracer


Troubleshooting

Target

> 🏆 CCNA




---

Months 4–5

LINUX + WINDOWS

Learn:

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

Learn:

CIA
IAM
Cryptography
Network Security
Threats
Vulnerabilities
Risk
Incident Response

Target

> 🏆 Security+




---

Months 7–9

SOC

Learn:

Wireshark
Nmap
Windows Logs
Linux Logs
SIEM
IOC
MITRE ATT&CK
Alert Triage
Incident Investigation


---

Months 9–11

PROJECTS

Complete:

[ ] Network Investigation

[ ] Linux Security Investigation

[ ] SOC/SIEM Investigation

[ ] Phishing Investigation



---

Months 11–12

CAREER PREPARATION

[ ] Cybersecurity Resume

[ ] LinkedIn

[ ] GitHub

[ ] SOC Interview Preparation

[ ] Networking Interview Questions

[ ] Security Interview Questions

[ ] Apply for SOC Analyst L1 roles

[ ] Apply for Junior Security Analyst roles

[ ] Apply for Security Operations roles



---

🧠 THE GOLDEN RULE

Whenever you find another huge cybersecurity roadmap, ask:

> "Will this skill help me understand networks, operating systems, security, detection, investigation, or automation?"



If YES:

Prioritize it.

If MAYBE:

Learn it later.

If NO:

Ignore it for now.


---

🔥 YOUR CORE PATH

BCA
  ↓
Wipro Trust & Safety
  ↓
Networking
  ↓
CCNA 🏆
  ↓
Linux
  ↓
Windows + Active Directory
  ↓
Security Fundamentals
  ↓
Security+ 🏆
  ↓
Wireshark + Nmap
  ↓
SIEM
  ↓
Incident Response
  ↓
Cybersecurity Projects
  ↓
GitHub Portfolio
  ↓
SOC Analyst L1 🎯
  ↓
Security Analyst
  ↓
Specialization
  ↓
International Cybersecurity Career 🌍


---

💡 WHY THIS PATH FITS ME

My current professional experience already gives me experience in:

Trust & Safety Operations

User-Generated Content Moderation

Policy Enforcement

Platform Safety

Risk Assessment

Abuse Detection

Investigation Support

Trend Analysis

Process Improvement

Analytical Reasoning

High-volume decision making


The next step is to add:

Networking
+
Linux
+
Windows/AD
+
Security
+
SIEM
+
Incident Response
+
Hands-on Projects

This transforms my profile from:

> Trust & Safety professional interested in cybersecurity



into:

> IT professional with Trust & Safety experience + cybersecurity certifications + practical security investigation skills.




---

🏆 FINAL 80/20 STRATEGY

Do these extremely well:

1. Networking


2. CCNA


3. Linux


4. Windows + Active Directory


5. Security Fundamentals


6. Security+


7. Wireshark


8. SIEM


9. Incident Response


10. 4 Strong Cybersecurity Projects



Do NOT try to master everything.

The goal is:

> Deep enough to perform, broad enough to understand, and focused enough to get hired.




---

🎯 FINAL TARGET

🛡️ CYBERSECURITY

                         YOU
                          │
                          ▼
                    🏆 CCNA
                          │
                          ▼
                     🐧 LINUX
                          │
                          ▼
                 🪟 WINDOWS + AD
                          │
                          ▼
                 🔐 SECURITY+
                          │
                          ▼
                🔎 WIRESHARK / NMAP
                          │
                          ▼
                    📊 SIEM
                          │
                          ▼
               🚨 INCIDENT RESPONSE
                          │
                          ▼
                  🧪 4 PROJECTS
                          │
                          ▼
                  💻 GITHUB PORTFOLIO
                          │
                          ▼
                  🎯 SOC ANALYST L1
                          │
                          ▼
                🌍 INTERNATIONAL
                   CYBERSECURITY

Rule: Certifications prove knowledge.
Labs prove ability.
Projects prove application.
Work experience proves professional capability.

Your goal is to build all four.