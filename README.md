# 🚨 Incident Response Playbooks — NIST 800-61 & SOC Operations Case Study

This project contains a full suite of **Incident Response (IR) Playbooks** aligned with industry standards:
- **NIST SP 800-61 (Computer Security Incident Handling Guide)**
- **SANS Incident Response Process**
- **ISO 27035 (Incident Management)**
- **MITRE ATT&CK Framework**

These playbooks demonstrate enterprise-grade IR capability suitable for:
- SOC teams  
- Cybersecurity Consultants  
- IR Analysts  
- Blue Team Operations  
- MSSP environments  

---

# 📘 1. Project Summary

The goal of this project is to build **actionable, step-by-step IR playbooks** covering the most common cyber incidents faced by modern organizations, including:

- Malware infections  
- Ransomware attacks  
- Phishing incidents  
- Unauthorized access  
- Data breach / exfiltration  
- DDoS attacks  
- Insider threats  

Each playbook outlines:
- Triage steps  
- Containment strategy  
- Forensic collection  
- Eradication  
- Recovery  
- Communication plan  
- Lessons learned  

---

# 🎯 2. Objectives

- Create practical, SOC-ready IR playbooks  
- Standardize detection, triage, and response actions  
- Improve cyber resilience  
- Reduce incident impact and downtime  
- Align response workflows with NIST/SANS  
- Enable efficient escalation and communication  

---

# 🧩 3. NIST 800-61 Incident Response Lifecycle

       ┌────────────────────────────┐
       │ 1. Preparation              │
       └─────────┬──────────────────┘
                 │
       ┌─────────▼─────────┐
       │ 2. Detection &     │
       │    Analysis        │
       └─────────┬─────────┘
                 │
       ┌─────────▼─────────┐
       │ 3. Containment,    │
       │    Eradication &   │
       │    Recovery        │
       └─────────┬─────────┘
                 │
       ┌─────────▼─────────┐
       │ 4. Lessons Learned │
       └────────────────────┘

---

# 📦 4. Playbooks Included

This project provides playbooks for:

1. **Malware / Virus Infection**  
2. **Ransomware Attack**  
3. **Phishing Email Incident**  
4. **Unauthorized Access / Account Compromise**  
5. **Web Application Attack (SQLi, XSS, LFI)**  
6. **Data Exfiltration / Data Breach**  
7. **DDoS Attack**  
8. **Insider Threat Incident**  

Each playbook follows a structured, repeatable IR pattern.

---

# 🔥 5. Playbook #1 — Malware / Virus Infection

### ✔ Detection
- Alerts from EDR/SIEM  
- User reports suspicious pop-ups  
- Unusual outbound C2 connections  

### ✔ Triage
- Identify affected machine  
- Check running processes  
- Validate suspicious files  

### ✔ Containment
- Disconnect machine from the network  
- Block malicious domains/IPs  
- Disable compromised user accounts  

### ✔ Eradication
- Remove malware via EDR  
- Patch vulnerable applications  
- Reset credentials  

### ✔ Recovery
- Restore from clean backup  
- Reconnect device  
- Validate system integrity  

### ✔ MITRE Mapping
- T1059: Command Execution  
- T1071: C2 Traffic  

---

# 🔥 6. Playbook #2 — Ransomware Attack

### ✔ Detection
- Sudden file encryption  
- Ransom note observed  
- SIEM alert for mass file modifications  

### ✔ Containment
- Isolate infected endpoints  
- Disable SMB file sharing  
- Stop affected services  

### ✔ Eradication
- Identify ransomware strain  
- Kill malicious processes  
- Remove persistence mechanisms  

### ✔ Recovery
- Restore from verified backups  
- Reset admin credentials  
- Harden access controls  

### ✔ Communication
- Notify leadership  
- Prepare legal/compliance briefing  

### ✔ MITRE Mapping
- T1486: Data Encryption for Impact  
- T1489: Service Stop  

---

# 📧 7. Playbook #3 — Phishing Email Incident

### ✔ Detection
- User reports suspicious email  
- Email contains malicious attachment/link  

### ✔ Triage
- Identify affected users  
- Analyze headers, sender domain, URL  

### ✔ Containment
- Block malicious sender  
- Quarantine email from all inboxes  

### ✔ Eradication
- Remove malicious artifacts  
- Delete suspicious rules (e.g., Outlook rules)  

### ✔ Recovery
- User password reset  
- Awareness training  

### ✔ MITRE Mapping
- T1566: Phishing  
- T1059: Malicious scripts  

---

# 🔐 8. Playbook #4 — Unauthorized Access / Account Compromise

### ✔ Detection
- Impossible travel logins  
- Successful login after multiple failures  
- Unknown device or location  

### ✔ Triage
- Verify user activity  
- Check SIEM & IAM logs  
- Identify accessed resources  

### ✔ Containment
- Force password reset  
- Revoke session tokens  
- Require MFA re-enrollment  

### ✔ Eradication
- Remove backdoor authentication methods  
- Disable malicious OAuth tokens  

### ✔ Recovery
- Monitor for abnormal access  
- Conduct account review  

### ✔ MITRE Mapping
- T1078: Valid Accounts  
- T1021: Lateral Movement  

---

# 🌐 9. Playbook #5 — Web Application Attack

### Threats Covered
- SQL Injection  
- XSS  
- Path Traversal  
- Brute Force  

### ✔ Detection
- WAF alerts  
- Suricata/SIEM events  

### ✔ Containment
- Block malicious IP  
- Enable WAF rule set  
- Patch vulnerable code  

### ✔ Recovery
- Rerun vulnerability scanners  
- Deploy secure code changes  

---

# 📤 10. Playbook #6 — Data Exfiltration

### ✔ Detection
- Unusual outbound traffic  
- Large data transfers  
- DNS tunneling indicators  

### ✔ Containment
- Block suspicious outbound connections  
- Disable compromised accounts  

### ✔ Eradication
- Remove malware or reverse shells  
- Patch exploited vulnerabilities  

### ✔ Recovery
- Validate no further leaks  
- Conduct forensic data analysis  

### ✔ MITRE Mapping
- T1048: Exfiltration over Alternative Protocol  

---

# 🌩️ 11. Playbook #7 — DDoS Attack

### ✔ Detection
- Traffic spike on a single service  
- Increased load balancer CPU  
- Firewall logs showing SYN floods  

### ✔ Containment
- Enable DDoS protection  
- Geo-block as needed  
- Rate limiting & throttling  

### ✔ Eradication
- None — DDoS requires mitigation, not removal  

### ✔ Recovery
- Restore normal access  
- Conduct post-incident review  

---

# 🕵️‍♂️ 12. Playbook #8 — Insider Threat

### ✔ Detection
- Unusual file downloads  
- Unauthorized access attempts  
- Data transfer to personal email  

### ✔ Containment
- Lock account  
- Revoke access tokens  
- Begin investigation  

### ✔ Eradication
- Remove unauthorized tools  
- Disable external sharing  

### ✔ Recovery
- Review privilege levels  
- Implement least privilege  

---

# 📊 13. IR Severity Classification Matrix

| Severity | Impact | Response Time | Example |
|---------|--------|---------------|---------|
| Critical | Org-wide risk | Immediate | Ransomware |
| High | System compromise | < 1 hour | Unauthorized access |
| Medium | Limited impact | Same day | Phishing |
| Low | Minimal risk | 24–72h | Minor alerts |

---

# 🧠 14. Roles & Responsibilities (RACI Matrix)

| Role | Detect | Contain | Eradicate | Approve | Communicate |
|------|---------|----------|------------|----------|-------------|
| SOC Analyst | R | R | C | - | C |
| Incident Manager | C | A | A | A | A |
| Forensics Team | C | C | R | - | C |
| IT Ops | - | C | R | - | - |
| Leadership | - | - | - | A | A |

(R = Responsible, A = Accountable, C = Consulted)

---

# 📦 15. Deliverables Included

- Full set of 8 IR Playbooks  
- NIST-aligned IR lifecycle  
- MITRE mapping tables  
- Triage & containment steps  
- Communication workflow  
- Severity matrix  
- RACI responsibilities map  
- ASCII incident diagrams  

---

# 📈 16. Key Outcomes

- Standardized SOC incident workflows  
- Faster triage & containment  
- Reduced incident impact  
- Strengthened IR maturity  
- Improved communication & escalation  
- Aligned with compliance standards  

---

# 🧾 17. Conclusion

This Incident Response Playbook Suite demonstrates professional cybersecurity capabilities in:

- SOC operations  
- Incident detection and containment  
- Forensic investigation  
- Risk reduction  
- Executive reporting  
- MITRE TTP mapping  

It reflects **real-world consulting deliverables** used by IR teams in enterprise environments.

---

# 📬 Contact

**GitHub:** https://github.com/rajbharti-cyber  
**LinkedIn:** https://www.linkedin.com/in/rajbharti-cybersecurity/
