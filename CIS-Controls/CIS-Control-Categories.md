# CIS Controls v8.1 — Control Categories

## 1. Overview

CIS Controls v8.1 contains 18 prioritized Controls designed to help organizations defend against common and significant cybersecurity threats.

The Controls cover the cybersecurity lifecycle from identifying assets and vulnerabilities through protection, monitoring, incident response, and recovery.

---

# 2. CIS Control 1 — Inventory and Control of Enterprise Assets

## Objective

Maintain an accurate inventory of enterprise assets and identify unauthorized or unmanaged devices.

## Examples

* Maintain an asset inventory.
* Identify asset owners.
* Track asset lifecycle.
* Detect unauthorized devices.
* Reconcile asset inventories regularly.

## Evidence

* Asset register
* CMDB
* GLPI records
* Network discovery reports
* Endpoint management reports

## IT Risk Example

**Risk:** Unknown or unmanaged devices may connect to the organization's network.

---

# 3. CIS Control 2 — Inventory and Control of Software Assets

## Objective

Maintain an accurate inventory of software installed within the environment.

## Examples

* Maintain approved software inventory.
* Identify unauthorized software.
* Track software versions.
* Remove unsupported software.
* Monitor software installation.

## Evidence

* Software inventory
* Endpoint management reports
* Application whitelisting reports

## IT Risk Example

**Risk:** Unauthorized or vulnerable software may introduce security weaknesses.

---

# 4. CIS Control 3 — Data Protection

## Objective

Identify, classify, securely handle, retain, and dispose of data.

## Examples

* Data classification
* Data inventory
* Encryption
* Data retention
* Secure disposal
* Data loss prevention

## Evidence

* Data classification policy
* DLP reports
* Encryption configurations
* Data retention records

## IT Risk Example

**Risk:** Sensitive information may be exposed, modified, or improperly retained.

---

# 5. CIS Control 4 — Secure Configuration of Enterprise Assets and Software

## Objective

Establish and maintain secure configurations for enterprise assets and software.

## Examples

* Secure configuration standards
* System hardening
* Configuration baselines
* Disable unnecessary services
* Remove default credentials
* Configuration monitoring

## Evidence

* Hardening standards
* Configuration baselines
* Configuration scan reports
* Security assessment reports

## IT Risk Example

**Risk:** Insecure configurations may expose systems to compromise.

---

# 6. CIS Control 5 — Account Management

## Objective

Manage user and administrator accounts throughout their lifecycle.

## Examples

* Unique user accounts
* Account creation approval
* Account deactivation
* Dormant account management
* Service account management
* Privileged account management

## Evidence

* Active Directory reports
* User listings
* Joiner-Mover-Leaver records
* Account review reports

## IT Risk Example

**Risk:** Former employees may retain active accounts.

---

# 7. CIS Control 6 — Access Control Management

## Objective

Manage access to enterprise assets and information according to business requirements.

## Examples

* Least privilege
* Role-based access
* MFA
* Privileged access controls
* Periodic access reviews
* Segregation of duties

## Evidence

* Access matrices
* Access review reports
* PAM reports
* MFA reports
* Access approvals

## IT Risk Example

**Risk:** Users may receive excessive privileges.

---

# 8. CIS Control 7 — Continuous Vulnerability Management

## Objective

Continuously identify, assess, prioritize, and remediate vulnerabilities.

## Examples

* Vulnerability scanning
* Risk-based prioritization
* Patch management
* Vulnerability remediation SLAs
* Exception management

## Evidence

* Nessus reports
* Vulnerability dashboards
* Patch reports
* Remediation tickets

## IT Risk Example

**Risk:** Critical vulnerabilities may remain unremediated and be exploited.

---

# 9. CIS Control 8 — Audit Log Management

## Objective

Collect, manage, protect, and analyze audit logs.

## Examples

* Centralized logging
* Log retention
* SIEM integration
* Log monitoring
* Time synchronization
* Protection against log tampering

## Evidence

* SIEM reports
* Log retention settings
* System logs
* Monitoring reports

## IT Risk Example

**Risk:** Security events may not be detected or investigated because required logs are unavailable.

---

# 10. CIS Control 9 — Email and Web Browser Protections

## Objective

Reduce risks associated with email and web-based threats.

## Examples

* Email filtering
* Anti-phishing protection
* Safe browsing
* URL filtering
* Attachment scanning
* Browser security configuration

## Evidence

* Email security reports
* Phishing reports
* Web filtering reports
* Security gateway configurations

## IT Risk Example

**Risk:** Users may be compromised through phishing emails or malicious websites.

---

# 11. CIS Control 10 — Malware Defenses

## Objective

Prevent and detect malware across enterprise assets.

## Examples

* Endpoint protection
* EDR
* Anti-malware
* Malware detection
* Automated remediation
* Centralized monitoring

## Evidence

* EDR reports
* Antivirus reports
* Malware alerts
* Endpoint compliance reports

## IT Risk Example

**Risk:** Malware may infect endpoints and compromise organizational systems.

---

# 12. CIS Control 11 — Data Recovery

## Objective

Ensure organizational data and systems can be recovered following disruption or compromise.

## Examples

* Automated backups
* Backup monitoring
* Offline or isolated backups
* Restoration testing
* Recovery procedures
* Backup protection

## Evidence

* Backup reports
* Backup logs
* Restoration test results
* Disaster recovery reports

## IT Risk Example

**Risk:** Data may be permanently lost following ransomware or system failure.

---

# 13. CIS Control 12 — Network Infrastructure Management

## Objective

Establish and maintain secure network infrastructure.

## Examples

* Network device inventory
* Secure configuration
* Firewall management
* Network segmentation
* Infrastructure monitoring
* Configuration backups

## Evidence

* Network diagrams
* Firewall configurations
* Router/switch configurations
* Configuration reports

## IT Risk Example

**Risk:** Poorly secured network infrastructure may allow unauthorized access or lateral movement.

---

# 14. CIS Control 13 — Network Monitoring and Defense

## Objective

Monitor networks to detect and respond to potentially harmful activity.

## Examples

* Network traffic monitoring
* IDS/IPS
* Network detection
* Security alerts
* Traffic analysis
* Segmentation monitoring

## Evidence

* IDS/IPS reports
* Network monitoring dashboards
* SIEM alerts
* Firewall logs

## IT Risk Example

**Risk:** Malicious network activity may not be detected promptly.

---

# 15. CIS Control 14 — Security Awareness and Skills Training

## Objective

Ensure employees and relevant third parties understand cybersecurity responsibilities.

## Examples

* Security awareness training
* Phishing simulations
* Role-based security training
* Policy awareness
* Training completion monitoring

## Evidence

* Training completion reports
* Phishing simulation results
* Awareness materials
* Policy acknowledgements

## IT Risk Example

**Risk:** Employees may inadvertently expose the organization to cyber threats.

---

# 16. CIS Control 15 — Service Provider Management

## Objective

Manage cybersecurity risks associated with third-party service providers.

## Examples

* Vendor risk assessments
* Security requirements
* Supplier due diligence
* Contractual security requirements
* Periodic supplier reviews
* Third-party access management

## Evidence

* Vendor assessments
* Contracts
* Security questionnaires
* Supplier review reports
* Third-party access listings

## IT Risk Example

**Risk:** A third-party service provider may expose organizational data or systems to compromise.

---

# 17. CIS Control 16 — Application Software Security

## Objective

Manage security risks associated with internally developed and acquired applications.

## Examples

* Secure development practices
* Application security testing
* Vulnerability remediation
* Code review
* Application access controls
* Secure deployment

## Evidence

* Security test reports
* Code review records
* Vulnerability reports
* Change records
* Application security assessments

## IT Risk Example

**Risk:** Application vulnerabilities may be exploited to compromise organizational data.

---

# 18. CIS Control 17 — Incident Response Management

## Objective

Establish and maintain an incident response capability.

## Examples

* Incident response plans
* Incident classification
* Escalation procedures
* Response playbooks
* Incident exercises
* Post-incident reviews

## Evidence

* Incident response plans
* Incident tickets
* Response reports
* Exercise results
* Root cause analysis

## IT Risk Example

**Risk:** Cybersecurity incidents may not be contained or resolved within acceptable timeframes.

---

# 19. CIS Control 18 — Penetration Testing

## Objective

Test the effectiveness and resilience of security controls through penetration testing.

## Examples

* External penetration testing
* Internal penetration testing
* Application penetration testing
* Network penetration testing
* Remediation tracking
* Retesting

## Evidence

* Penetration test reports
* Vulnerability findings
* Remediation records
* Retest reports

## IT Risk Example

**Risk:** Security weaknesses may remain unidentified until exploited by attackers.

---

# 20. CIS Controls Summary

| #  | CIS Control                          | Primary Focus                          |
| -- | ------------------------------------ | -------------------------------------- |
| 1  | Enterprise Asset Inventory           | Know what assets exist                 |
| 2  | Software Asset Inventory             | Know what software exists              |
| 3  | Data Protection                      | Protect organizational data            |
| 4  | Secure Configuration                 | Harden assets and software             |
| 5  | Account Management                   | Manage accounts                        |
| 6  | Access Control Management            | Control access                         |
| 7  | Vulnerability Management             | Identify and remediate vulnerabilities |
| 8  | Audit Log Management                 | Capture and analyze logs               |
| 9  | Email & Browser Protections          | Defend against web/email threats       |
| 10 | Malware Defenses                     | Prevent and detect malware             |
| 11 | Data Recovery                        | Recover data and systems               |
| 12 | Network Infrastructure Management    | Secure network infrastructure          |
| 13 | Network Monitoring & Defense         | Detect network threats                 |
| 14 | Security Awareness & Skills Training | Strengthen human security              |
| 15 | Service Provider Management          | Manage third-party risk                |
| 16 | Application Software Security        | Secure applications                    |
| 17 | Incident Response Management         | Respond to incidents                   |
| 18 | Penetration Testing                  | Validate security controls             |

---

# 21. CIS Controls and Control Testing

A CIS safeguard can be assessed using the same control-testing lifecycle used elsewhere in this repository:

```text
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
Exception
 ↓
Effectiveness
 ↓
Risk Treatment
 ↓
Remediation
```

## Key Takeaway

CIS Controls provide a practical bridge between cybersecurity risk and technical or operational safeguards.

The next document, `CIS-Control-Examples.md`, will convert these 18 Controls into detailed examples of:

**Risk → Safeguard → Evidence → Testing → Effectiveness → Remediation**
