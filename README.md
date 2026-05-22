<div align="center">

# Hey, I'm Mahesh 👋

[![Typing SVG](https://readme-typing-svg.demolab.com/?lines=SIEM+%26+Detection+Engineer;Penetration+Tester+%26+Security+Researcher;Splunk+%7C+Wazuh+%7C+Elastic+%7C+MITRE+ATT%26CK;Top+10%25+Globally+on+TryHackMe;2+IDOR+Vulnerabilities+Responsibly+Disclosed&font=Fira+Code&center=true&width=580&height=55&color=00FF87&vCenter=true&size=18&pause=1200)](https://tryhackme.com/p/Mahikolla)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mahesh-kumar-kolla/)
[![TryHackMe](https://img.shields.io/badge/-TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/Mahikolla)
[![Email](https://img.shields.io/badge/ProtonMail-8B89CC?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:MaheshKolla@protonmail.com)

</div>

---

## Who am I?

I'm a cybersecurity engineer who genuinely enjoys finding things that shouldn't be there.

Whether it's building a SIEM to catch attackers mid-move, fuzzing web apps until they give something up, or writing tools that cut recon time by 80% — this is the work I actually want to be doing.

- 🎓 B.Tech in Cybersecurity, **KL University, Vijayawada** — 9.08 CGPA, graduating Apr 2026
- 🔍 Found and reported **2 real IDOR vulnerabilities** in production apps — one was a university portal that let anyone read anyone else's records just by changing an ID in the URL
- 🛡️ Built a home SOC lab processing **~1,500 events/day** across Splunk, Wazuh, and Elastic with detections mapped to MITRE ATT&CK
- 🏆 **Top 10% globally on TryHackMe** · Top 10 at Hack Havoc CTF (CyberMaterial, 2024)
- 👨‍💻 Led **6+ hands-on security workshops** for 400+ students as Technical Director of my university's security club — across 3 academic years
- 🖥️ Personal Proxmox homelab: pfSense · Security Onion · DVWA · Metasploitable3
- 📍 India · Open to Relocate

---

## Certifications

| Certification | Status |
|---|---|
| CompTIA Security+ SY0-701 | 🔄 In Progress (Jun 2026) |
| ISC2 Certified in Cybersecurity (CC) | ✅ Mar 2025 |
| AWS Cloud Practitioner | ✅ Feb 2025 |
| Certified AppSec Practitioner | ✅ Jun 2023 |

---

## What I work with

<div align="center">

**Languages & Dev**

[![Skills](https://skillicons.dev/icons?i=py,js,ts,react,nextjs,bash,powershell,docker,git,linux,aws,mysql,mongodb,postgres&perline=7&theme=dark)](https://skillicons.dev)

**Security Toolkit**

![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![Elastic](https://img.shields.io/badge/Elastic-005571?style=flat-square&logo=elastic&logoColor=white)
![Kibana](https://img.shields.io/badge/Kibana-005571?style=flat-square&logo=kibana&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-3AAAFF?style=flat-square&logoColor=white)
![Zeek](https://img.shields.io/badge/Zeek-2980B9?style=flat-square&logoColor=white)
![Sigma](https://img.shields.io/badge/Sigma_Rules-111111?style=flat-square&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C01C00?style=flat-square&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-0E83CD?style=flat-square&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP_Top_10-000000?style=flat-square&logo=owasp&logoColor=white)
![IAM](https://img.shields.io/badge/IAM-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![GuardDuty](https://img.shields.io/badge/GuardDuty-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![CloudTrail](https://img.shields.io/badge/CloudTrail-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Atomic Red Team](https://img.shields.io/badge/Atomic_Red_Team-E74C3C?style=flat-square&logoColor=white)

</div>

---

## Things I've built

### 🔵 Security Monitoring & SIEM Lab

Most people learn SIEM tools by clicking through a dashboard. I built a lab.

I set up a multi-SIEM home SOC ingesting ~1,500 events/day from Linux endpoints — authentication, process, and network telemetry flowing through Splunk, Wazuh, and Elastic simultaneously. Then I wrote 8 detection rules in Sigma and SPL: SSH brute-force, suspicious PowerShell, credential dumping — all mapped to MITRE ATT&CK (T1110, T1059, T1003).

Then I ran Atomic Red Team simulations against it to see if the rules would actually fire. They did — **100% detection coverage** across every mapped technique. Documented triage workflows, IOC pivots, and false-positive tuning notes per rule.

`Splunk` `Wazuh` `Elastic` `Zeek`

---

### 🔴 Python VAPT Automation Toolkit

Recon is tedious when you do it manually. So I automated it.

One command chains subdomain enumeration → port scanning → service fingerprinting → NVD CVE/CVSS lookup into a single run. It wraps Nmap NSE scripts to parse service banners and auto-generates Markdown + JSON reports with CVE IDs and CVSS scores — the kind of output you can drop straight into a pentest report.

What used to take **~30 minutes per host now takes ~6**. That's the whole point.

`Python` `Nmap` `NVD API`

---

### 🟠 LinkFlow — URL Redirect Chain Analyzer

Looks like a normal shortened URL 😌 — acts like a security blind spot 👀

Ever clicked a `bit.ly` link without knowing where it actually leads? I built **LinkFlow** because you shouldn't have to click first and ask questions later 😅

→ Follows up to 10 redirects automatically  
→ Shows HTTP status codes at each hop  
→ Measures response time per hop  
→ Flags suspicious domains via **VirusTotal + Google Safe Browsing**  
→ Keeps history of your recent analyses  

Phishing attacks hide behind redirect chains. Marketing links break. That "urgent" email link might go through 4 hops before landing somewhere you didn't intend. Now you can see the full path before you get there.

**Security is about visibility — and sometimes that starts with knowing what URL you're actually visiting.**

🔗 [linkflows.vercel.app](https://linkflows.vercel.app)

`Next.js` `TypeScript` `VirusTotal API`

---

### 🔐 Responsible Disclosure

I didn't just read about IDOR vulnerabilities. I found two of them — in production.

One was a university student portal. Change the ID in the URL, and you're reading someone else's records. No authentication check. No rate limiting. Just a predictable parameter and an assumption that users wouldn't look.

I reproduced it via Burp Suite Repeater and parameter fuzzing, documented the impact, reported it through proper channels, and stayed in the loop until the patch was verified. Two vulnerabilities. Two fixes. Done right.

`Burp Suite` `IDOR` `Parameter Fuzzing`

---

## GitHub Stats

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com?user=Mahesh-Kumar-Kolla&theme=tokyonight&hide_border=true)

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=Mahesh-Kumar-Kolla&theme=tokyo-night&hide_border=true&area=true&custom_title=Contribution%20Activity)](https://github-readme-activity-graph.vercel.app)

[![TryHackMe](https://tryhackme-badges.s3.amazonaws.com/Mahikolla.png)](https://tryhackme.com/p/Mahikolla)

</div>

---

<div align="center">

*Open to SOC Analyst · Security Engineer · Penetration Tester roles*

</div>

![footer](https://capsule-render.vercel.app/api?type=waving&color=0:0a3d62,100:0D1117&height=100&section=footer)
