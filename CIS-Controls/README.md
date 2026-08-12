# CIS Controls

## 1. Overview

The CIS Controls are a prioritized set of cybersecurity safeguards developed by the Center for Internet Security (CIS).

They provide practical and actionable security measures that organizations can use to reduce common cybersecurity risks.

Unlike broader governance frameworks, CIS Controls are particularly useful for translating cybersecurity requirements into **specific technical and operational safeguards**.

---

## 2. Purpose

The CIS Controls can help organizations:

* Identify cybersecurity weaknesses
* Prioritize security improvements
* Reduce attack surface
* Improve endpoint security
* Strengthen identity and access management
* Improve vulnerability management
* Improve logging and monitoring
* Protect sensitive data
* Support cybersecurity assessments
* Support IT Risk and RCSA activities

---

## 3. CIS Controls v8.1

CIS Controls v8.1 organizes cybersecurity safeguards into **18 Controls**.

The Controls address areas such as:

* Asset management
* Software management
* Data protection
* Secure configuration
* Account management
* Access control
* Vulnerability management
* Audit logging
* Email and browser protection
* Malware defenses
* Network infrastructure
* Network monitoring
* Security awareness
* Service provider management
* Application security
* Incident response
* Penetration testing

---

## 4. CIS Implementation Groups

CIS Controls can be prioritized using Implementation Groups (IGs).

### IG1 — Essential Cyber Hygiene

Focuses on foundational safeguards that every organization should implement.

Examples:

* Asset inventory
* Software inventory
* Account management
* Data protection
* Secure configuration
* Vulnerability management
* Malware defenses

### IG2 — Expanding Security

Adds safeguards for organizations with greater cybersecurity requirements and resources.

### IG3 — Advanced Security

Addresses more sophisticated environments and organizations facing significant cybersecurity threats.

```text id="h35n4w"
                  CIS CONTROLS
                       |
          ┌────────────┼────────────┐
          ↓            ↓            ↓
         IG1          IG2          IG3
       Essential    Expanding     Advanced
       Controls      Controls     Controls
```

---

## 5. CIS Controls and IT Risk

CIS Controls can be used to translate an IT Risk into practical security safeguards.

Example:

### Risk

Critical systems may remain vulnerable because security patches are not deployed within defined timelines.

### CIS Control

Vulnerability Management.

### Safeguards

* Identify vulnerabilities
* Prioritize vulnerabilities
* Track remediation
* Deploy security patches
* Monitor overdue vulnerabilities

### Evidence

* Vulnerability scans
* Patch reports
* Remediation tickets
* Exception records

---

## 6. CIS Controls and RCSA

CIS Controls can support RCSA by providing practical safeguards that can be assessed for effectiveness.

```text id="gk1e3h"
Risk
 ↓
CIS Control
 ↓
Safeguard
 ↓
Control Owner
 ↓
Evidence
 ↓
Testing
 ↓
Effectiveness
 ↓
Finding
 ↓
Remediation
```

---

## 7. CIS Controls and IT Risk Tracker

CIS Control mappings can be added to the IT Risk Tracker.

| Risk                    | Control                  | CIS Area                 | Effectiveness       | Treatment |
| ----------------------- | ------------------------ | ------------------------ | ------------------- | --------- |
| Unknown devices         | Asset inventory          | Asset Management         | Partially Effective | Mitigate  |
| Unauthorized accounts   | Account management       | Account Management       | Effective           | Accept    |
| Unpatched systems       | Vulnerability management | Vulnerability Management | Partially Effective | Mitigate  |
| Security events missed  | Audit logging            | Audit Log Management     | Partially Effective | Mitigate  |
| Malware infection       | Malware defenses         | Malware Defenses         | Effective           | Accept    |
| Weak security awareness | Awareness training       | Security Awareness       | Partially Effective | Mitigate  |

---

## 8. CIS Controls vs Other Frameworks

| Framework     | Primary Focus                      |
| ------------- | ---------------------------------- |
| COBIT         | IT Governance and Management       |
| ISO/IEC 27001 | Information Security Management    |
| NIST CSF      | Cybersecurity Risk Management      |
| CIS Controls  | Practical Cybersecurity Safeguards |
| ITGC          | IT General Controls                |
| COSO          | Enterprise Internal Controls       |
| PCI DSS       | Payment Card Security              |

### Key Difference

A useful way to think about the frameworks is:

> **COBIT:** How should IT be governed?

> **ISO/IEC 27001:** How should information security be managed?

> **NIST CSF:** How should cybersecurity risk be managed?

> **CIS Controls:** What practical safeguards should we implement?

---

## 9. Example

### Risk

Shared administrative accounts may be used to perform unauthorized activities on critical systems.

### Safeguard

Implement unique accounts for administrators and manage privileged access appropriately.

### Evidence

* Active Directory reports
* PAM reports
* Privileged account listings
* Audit logs

### Testing

* Identify privileged accounts.
* Identify shared accounts.
* Verify named ownership.
* Review privileged access.
* Review activity logs.
* Assess control effectiveness.

### Possible Assessment

**Partially Effective**

PAM may be implemented, but shared administrative accounts remain in use.

---

## 10. Key Takeaway

CIS Controls are particularly valuable because they translate cybersecurity principles into practical safeguards.

The overall approach is:

**Identify → Prioritize → Implement → Monitor → Test → Improve**

The CIS Controls section of this repository will focus on turning common IT and cybersecurity risks into actionable controls that can be tested and tracked.
