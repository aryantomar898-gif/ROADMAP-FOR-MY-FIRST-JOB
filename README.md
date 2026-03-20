# 🛡️ Cybersecurity Fresher Roadmap
### Based on Cloud Security / Zscaler Engineer JD (Applicable to 100+ Companies)

---

## 🗺️ OVERALL TIMELINE OVERVIEW

| Phase | Duration | Focus |
|-------|----------|-------|
| Phase 1 | Month 1–2 | Networking Foundations |
| Phase 2 | Month 2–3 | Security Concepts |
| Phase 3 | Month 3–4 | Cloud & Identity |
| Phase 4 | Month 4–5 | Scripting & Automation |
| Phase 5 | Month 5–6 | Zscaler / SASE / Zero Trust |
| Phase 6 | Month 6+ | Certifications & Projects |

---

## PHASE 1 — Networking Foundations
> *"Strong knowledge of networking concepts: TCP/IP, DNS, NAT, routing, subnets, proxy, tunneling, L2/L3"*

### What to Learn
- **OSI Model** — All 7 layers, what happens at each
- **TCP/IP** — How packets travel, 3-way handshake, ports
- **DNS** — How domain resolution works, record types (A, MX, CNAME)
- **NAT** — Why it exists, how it translates IPs
- **Subnetting** — CIDR notation, calculating subnets (very important!)
- **Routing** — Static vs dynamic, BGP basics, default gateway
- **Proxy** — Forward proxy vs reverse proxy, how traffic flows
- **Tunneling** — GRE, IPSec, SSH tunneling
- **L2 vs L3** — Switching vs routing, MAC vs IP

### Free Resources
- **Professor Messer** (YouTube) — CompTIA Network+ playlist (FREE, excellent)
- **Practical Networking** (YouTube) — Subnetting, routing explained visually
- **SubnettingPractice.com** — Practice subnetting daily
- **Cisco Packet Tracer** (free tool) — Build and simulate networks hands-on
- **TryHackMe** — "Pre-Security" path (networking module)

### Milestone ✅
> You should be able to: explain how a packet travels from your laptop to google.com and back, subnet a /24 network, explain what a proxy does.

---

## PHASE 2 — Security Concepts
> *"SSL/TLS inspection, VPNs, traffic decryption, identity systems (SSO, LDAP, SAML, MFA), log forwarding (Syslog, SIEM, JSON, APIs)"*

### SSL/TLS & Encryption
- How HTTPS works (certificates, handshake, PKI)
- What SSL/TLS inspection means (man-in-the-middle by design)
- Symmetric vs Asymmetric encryption
- Certificates: CA, self-signed, chain of trust

### VPNs
- Site-to-site vs Remote access VPN
- IPSec vs SSL VPN
- How split tunneling works

### Identity & Access Management
- **SSO (Single Sign-On)** — One login for many apps
- **LDAP** — How directory services work (Active Directory)
- **SAML** — XML-based auth standard used in enterprise SSO
- **MFA** — TOTP, push notifications, hardware tokens

### Log Management
- **Syslog** — Standard log forwarding protocol
- **SIEM** — What it does (Splunk, Microsoft Sentinel, IBM QRadar)
- **JSON** — Log format used by most modern tools
- **APIs** — REST APIs, how security tools communicate

### Free Resources
- **TryHackMe** — "SOC Level 1" path (covers SIEM, logs, alerts)
- **IBM QRadar / Microsoft Sentinel** — Free tiers / sandbox available
- **OWASP** — Understanding web security basics
- **YouTube: John Hammond, NetworkChuck** — TLS, VPN, MFA videos

### Milestone ✅
> You should be able to: explain what happens when you log into an SSO portal, describe how SIEM collects logs, explain TLS handshake.

---

## PHASE 3 — Cloud Platforms & Security
> *"AWS, Azure, GCP — IAM, VPC, Security Groups"*

### Pick ONE cloud first (Recommend: AWS)
- **IAM** — Users, roles, policies, least privilege principle
- **VPC** — Virtual private cloud, subnets, route tables
- **Security Groups** — Stateful firewalls at instance level
- **NACLs** — Stateless, subnet-level access control

### Then understand the concept across all 3 clouds

| Concept | AWS | Azure | GCP |
|---------|-----|-------|-----|
| IAM | IAM | Azure AD / Entra ID | Cloud IAM |
| Virtual Network | VPC | VNet | VPC |
| Firewall | Security Groups | NSG | Firewall Rules |

### Free Resources
- **AWS Free Tier** — Create account, use hands-on labs
- **AWS Skill Builder** — Free cloud security courses
- **ACloudGuru / CloudSkillsBoost** — Paid but has free trials
- **TryHackMe** — "Cloud Security" rooms
- **A Cloud Guru YouTube** — AWS fundamentals

### Milestone ✅
> Launch a VM on AWS, configure security groups, create an IAM user with least-privilege policy.

---

## PHASE 4 — Scripting & Automation
> *"Python, PowerShell, Bash"*

### Priority Order for Cybersecurity: Python > Bash > PowerShell

### Python (Most Important)
- Variables, loops, functions, file I/O
- Working with APIs (requests library)
- Parsing JSON logs
- Building simple security tools (port scanner, log parser)

### Bash
- Linux command line basics
- Writing shell scripts
- Log parsing with grep, awk, sed
- Automating repetitive tasks

### PowerShell
- Used in Windows/Azure environments
- Active Directory automation
- Reading Windows Event Logs

### Free Resources
- **Automate the Boring Stuff with Python** (free at automatetheboringstuff.com)
- **OverTheWire: Bandit** — Learn Linux/Bash by hacking (free, fun)
- **TryHackMe** — Linux Fundamentals rooms
- **PowerShell for Beginners** — Microsoft Learn (free)

### Mini Projects to Build 🔨
1. Python script to parse a log file and extract failed login attempts
2. Bash script to check open ports on a server
3. Python script that calls a REST API and formats JSON output
4. PowerShell script to list all Active Directory users

### Milestone ✅
> Build a Python log parser that reads a syslog file, finds anomalies, and outputs a report.

---

## PHASE 5 — Zscaler / SASE / Zero Trust (Differentiator!)
> *"ZIA, ZPA, ZDX, Zero Trust, SASE, CASB, DLP, API Security"*

### Zero Trust Concepts
- "Never trust, always verify" — what this means in practice
- Identity-based access instead of network-based
- Micro-segmentation

### SASE (Secure Access Service Edge)
- Combines networking + security in the cloud
- Key vendors: Zscaler, Palo Alto Prisma, Cisco Umbrella, Netskope

### Zscaler Products
| Product | Purpose |
|---------|---------|
| ZIA (Zscaler Internet Access) | Secure internet access, replaces web proxy |
| ZPA (Zscaler Private Access) | Replace VPN, Zero Trust access to apps |
| ZDX (Zscaler Digital Experience) | Monitor user experience & performance |

### CASB, DLP, API Security
- **CASB** — Controls cloud app usage (shadow IT detection)
- **DLP** — Prevents sensitive data from leaving the org
- **API Security** — Securing API endpoints from misuse

### Free Resources
- **Zscaler Academy** (learning.zscaler.com) — FREE official training!
- **Zscaler YouTube Channel** — Product demos and architecture
- **Palo Alto EDU** — SASE/ZTNA free courses
- **Cloudflare Learning Center** — Zero Trust explained simply

### Milestone ✅
> Complete Zscaler Academy ZIA Fundamentals free course. Understand how ZIA replaces a traditional proxy.

---

## PHASE 6 — Certifications (Industry Recognized)

### Beginner (Start Here)
| Cert | Cost | Focus |
|------|------|-------|
| **CompTIA Security+** | ~$400 | Broad security baseline, most recognized |
| **CompTIA Network+** | ~$350 | Networking foundation |
| **Google Cybersecurity Certificate** | ~$200 (Coursera) | Practical intro, beginner-friendly |
| **ISC2 CC (Certified in Cybersecurity)** | FREE | Entry-level, globally recognized |

### Cloud Security (Mid-Level Goal)
| Cert | Focus |
|------|-------|
| **AWS Cloud Practitioner** | Cloud basics (free exam vouchers available) |
| **AWS Security Specialty** | Advanced cloud security |
| **AZ-500 (Azure Security)** | Microsoft security stack |
| **CCSP** | Cloud security (ISC2, prestigious) |

### Zscaler Specific
- **ZCCA-IA** — Zscaler Certified Cloud Associate (Internet Access)
- **ZCCP-IA** — Professional level
- Available via Zscaler Academy

### Pro Tips 💡
- **Start with ISC2 CC** — It's FREE and globally recognized
- **Then CompTIA Security+** — Required by many job postings
- Do **free practice exams** on ExamTopics, Jason Dion Udemy courses

---

## PREFERRED SKILLS — Nice to Have (Build These Later)

### Firewalls
- Learn Palo Alto NGFW concepts (free Palo Alto EDU courses)
- Understand firewall rules, zones, policies

### ServiceNow / Jira / ITSM
- Create free developer account on ServiceNow
- Learn to create incidents, change requests
- Understand ITIL basics (incident, change, problem management)

### Threat Modeling
- **STRIDE framework** — Spoofing, Tampering, Repudiation, Info Disclosure, DoS, Elevation
- **MITRE ATT&CK** — Free framework, used in every SOC
- **Microsoft Threat Modeling Tool** — Free download

---

## DOCUMENTATION & COMMUNICATION SKILLS
> *"Excellent documentation and communication skills"*

### Practice By:
- Writing post-incident reports (templates on GitHub)
- Documenting your lab setups (use Notion or Obsidian)
- Creating architecture diagrams (draw.io — free)
- Contributing to GitHub with README files

---

## 🔨 HANDS-ON LAB PLATFORMS (All Free or Cheap)

| Platform | What You Learn | Cost |
|----------|---------------|------|
| **TryHackMe** | Everything — great for beginners | Free/£10/mo |
| **HackTheBox** | Advanced labs | Free tier |
| **OverTheWire** | Linux, scripting | Free |
| **LetsDefend** | SOC analyst skills, SIEM | Free tier |
| **Cybrary** | Video courses + labs | Free tier |
| **SANS Cyberaces** | Networking, OS, security | Free |
| **Blue Team Labs Online** | Defensive security | Free tier |

---

## 📅 YOUR DAILY STUDY PLAN

| Day | Activity |
|-----|----------|
| Mon/Wed/Fri | Theory — video courses, reading |
| Tue/Thu | Hands-on — TryHackMe, labs, scripts |
| Saturday | Build a mini project or practice certification questions |
| Sunday | Review the week, update notes, plan next week |

**Daily minimum: 1.5 – 2 hours**

---

## 🎯 JOB READINESS CHECKLIST

- [ ] CompTIA Security+ or ISC2 CC certified
- [ ] At least 1 cloud certification (AWS/Azure)
- [ ] 3–5 GitHub projects (log parser, port scanner, etc.)
- [ ] TryHackMe profile with 50+ rooms completed
- [ ] Completed Zscaler Academy free courses
- [ ] LinkedIn updated with skills and projects
- [ ] Can explain Zero Trust, SASE, ZIA/ZPA in an interview
- [ ] Comfortable reading and writing Python scripts
- [ ] Understanding of MITRE ATT&CK framework

---

## 💼 COMPANIES THAT HIRE FOR THIS PROFILE

Beyond Zscaler, this skillset is in demand at:
- **MSSPs**: Secureworks, Trustwave, AT&T Cybersecurity
- **Big Tech**: Microsoft, Google, AWS (cloud security teams)
- **Consulting**: Deloitte, KPMG, PwC, Accenture (cybersecurity practice)
- **Telecom**: Verizon, BT, Tata Communications
- **Banks & Finance**: All major banks have large security teams
- **Product Companies**: Palo Alto Networks, Fortinet, CrowdStrike, Netskope

---

*"Cybersecurity is a marathon, not a sprint. Be consistent, build in public, and document everything."*
