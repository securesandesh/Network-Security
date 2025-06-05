# 🛡️ Controls and Compliance Assessment – NovaNexus Games

## 📘 Case Study Overview

**NovaNexus Games** is a mid-sized U.S.-based company that develops and distributes video games globally. As their digital platform expands, their IT and security teams face increased responsibility to protect sensitive data and maintain compliance with both domestic and international regulations.

To ensure a robust cybersecurity posture, the IT Security Director has initiated an internal audit using the **NIST Cybersecurity Framework (CSF)** to evaluate current risks, gaps, and control implementation.

---

## 🎯 Scope & Objectives

**Scope:**  
This audit assesses the entire cybersecurity infrastructure of NovaNexus Games, including:

- On-prem and cloud infrastructure
- Customer data handling processes
- Internal IT systems and procedures
- Third-party service integrations

**Goals:**

- Identify missing or insufficient controls
- Evaluate compliance with standards such as PCI DSS, GDPR, and SOC 2
- Recommend remediation steps to minimize risk

---

## 🖥️ Assets Managed by IT

- Developer and staff devices (desktops, laptops, tablets)
- Cloud-based and on-prem game servers
- Payment processing systems
- Customer databases (containing sensitive information)
- Internal tools (build systems, DevOps, databases)
- Surveillance systems and access control hardware
- Legacy warehouse inventory software

---

## 🔎 Risk Assessment Summary

- **Overall Risk Score:** 7.5 / 10  
- **Primary Concerns:**
  - Over-permissive access privileges
  - Insecure storage of sensitive customer data
  - Lack of incident response and backup plans
  - Non-compliance with international standards

---

## ✅ Controls Assessment Checklist

| Control Present? | Control                   | Explanation |
|------------------|---------------------------|-------------|
| ❌               | Role-Based Access Control  | Developers have admin access to production — too permissive. |
| ❌               | Incident Response Plan     | No formal IR strategy in place. |
| ✅               | Firewalls                  | In place across cloud and on-prem environments. |
| ❓               | Password Policy            | Exists, but lacks enforcement of strong password practices. |
| ✅               | Antivirus                  | Active enterprise protection installed. |
| ❌               | Data Backups               | Infrequent and local only — no redundancy. |
| ❌               | Encryption at Rest         | Sensitive data stored unencrypted. |
| ❌               | IDS/IPS                    | No threat detection system deployed. |
| ✅               | Physical Security (HQ)     | CCTV, access cards, secure perimeter. |
| ✅               | Smoke Detection Systems    | Installed and periodically tested. |

---

## 📜 Compliance Assessment

### PCI DSS

| Compliant? | Best Practice                                  | Explanation |
|------------|------------------------------------------------|-------------|
| ❌         | Limit payment system access                    | Team leads and developers have access — needs restriction. |
| ❌         | Secure storage of credit card data             | Some customer data is not encrypted. |
| ❌         | Secure data transmission                       | APIs not all using TLS. |

### GDPR

| Compliant? | Best Practice                                    | Explanation |
|------------|--------------------------------------------------|-------------|
| ❌         | Documented handling of EU customer data          | No data processing agreements in place. |
| ✅         | Public privacy policies                          | Policy is live and updated. |

### SOC 2 (System and Organization Controls)

| Compliant? | Best Practice                                    | Explanation |
|------------|--------------------------------------------------|-------------|
| ❌         | Defined access management policies               | No documented procedures. |
| ✅         | System logging and monitoring                    | Logs collected centrally. |
| ❌         | Regular access reviews and data classification   | No defined data tiers or audits. |

---

## 💡 Recommendations

To improve the security posture and meet regulatory requirements, NovaNexus Games should:

- Implement **Role-Based Access Control (RBAC)** and audit permissions quarterly
- Develop and test a **formal Incident Response Plan**
- Enforce **multi-factor authentication (MFA)** and stronger password policies
- Deploy **IDS/IPS systems** and log correlation through a **SIEM platform**
- Encrypt all sensitive customer data **at rest and in transit**
- Design and implement a **cloud-based backup and recovery strategy**
- Ensure proper documentation and adherence to **PCI DSS** and **GDPR**

---

## 📂 Repository Contents

This repository includes:

- `controls-assessment-checklist.md`: List of security controls evaluated
- `compliance-checklist.md`: PCI DSS, GDPR, and SOC 2 audit status
- `risk-assessment-report.md`: Overview of current risk levels and recommendations
- `incident-response-plan-template.md`: (To be added)
- `backup-policy-template.md`: (To be added)

---

## 🔐 Framework Used

- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
- [PCI DSS](https://www.pcisecuritystandards.org)
- [GDPR](https://gdpr.eu/)
- [SOC 2](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/sorhome.html)

---

## 📣 License

This project is provided for educational purposes only. No commercial use permitted without permission.

---

