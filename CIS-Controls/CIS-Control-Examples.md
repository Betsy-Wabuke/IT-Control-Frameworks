# CIS Controls — Practical Control Examples

## 1. Purpose

This document provides practical examples of cybersecurity risks and controls mapped to the CIS Controls.

The objective is to translate CIS Controls into an IT Risk and control-testing format:

**Risk → CIS Control → Safeguard → Evidence → Testing → Effectiveness → Remediation**

---

# 2. Enterprise Asset Management

## Risk

Unauthorized or unmanaged devices may connect to the organization's environment.

## CIS Control

**Control 1 — Inventory and Control of Enterprise Assets**

## Control

Maintain a complete and regularly reconciled inventory of enterprise assets.

## Evidence

* IT asset register
* CMDB
* GLPI records
* Endpoint management reports
* Network discovery results

## Testing

1. Obtain the approved asset inventory.
2. Compare the inventory against endpoint management records.
3. Compare against network discovery results.
4. Identify unmatched devices.
5. Investigate unidentified assets.
6. Document exceptions.

## Effectiveness

**Effective:** Asset sources are consistently reconciled and unauthorized assets are addressed.

**Partially Effective:** Some assets are missing or reconciliation is inconsistent.

**Ineffective:** No reliable inventory exists.

---

# 3. Software Asset Management

## Risk

Unauthorized or vulnerable software may introduce security weaknesses.

## CIS Control

**Control 2 — Inventory and Control of Software Assets**

## Controls

* Software inventory
* Approved software list
* Software version monitoring
* Removal of unauthorized software

## Evidence

* Software inventory
* Endpoint reports
* Application allowlists
* Software deployment records

## Testing

1. Obtain the software inventory.
2. Identify unsupported software.
3. Identify unauthorized applications.
4. Compare installed versions with approved versions.
5. Verify remediation of exceptions.

---

# 4. Data Protection

## Risk

Sensitive organizational information may be exposed, lost, or improperly handled.

## CIS Control

**Control 3 — Data Protection**

## Controls

* Data classification
* Encryption
* Data retention
* Data loss prevention
* Secure disposal

## Evidence

* Data classification records
* Encryption reports
* DLP alerts
* Retention schedules
* Disposal records

## Testing

1. Identify sensitive information.
2. Verify classification.
3. Check encryption requirements.
4. Review DLP controls.
5. Verify secure disposal.
6. Document exceptions.

---

# 5. Secure Configuration

## Risk

Insecure configurations may increase the attack surface of systems.

## CIS Control

**Control 4 — Secure Configuration of Enterprise Assets and Software**

## Controls

* Hardening standards
* Configuration baselines
* Removal of unnecessary services
* Secure default configurations
* Configuration monitoring

## Evidence

* Hardening guides
* Configuration baselines
* Configuration scan reports
* Compliance dashboards

## Testing

1. Select a sample of systems.
2. Obtain approved configuration standards.
3. Compare actual configurations with baselines.
4. Identify deviations.
5. Confirm remediation.

---

# 6. Account Management

## Risk

Inactive, unauthorized, or improperly managed accounts may be exploited.

## CIS Control

**Control 5 — Account Management**

## Controls

* Account approval
* Unique user IDs
* Joiner-Mover-Leaver process
* Dormant account review
* Service account management
* Administrative account management

## Evidence

* Active Directory reports
* User listings
* HR records
* Account approval records
* Deactivation records

## Testing

1. Obtain active account listings.
2. Compare accounts against HR records.
3. Identify terminated employees with active accounts.
4. Identify dormant accounts.
5. Verify service account ownership.
6. Confirm timely deactivation.

---

# 7. Access Control Management

## Risk

Users may receive access exceeding their business requirements.

## CIS Control

**Control 6 — Access Control Management**

## Controls

* Least privilege
* MFA
* Role-based access
* Privileged access management
* Access reviews
* Segregation of duties

## Evidence

* Access matrices
* PAM reports
* MFA reports
* User access reviews
* Approval records

## Testing

1. Select a sample of users.
2. Verify access approvals.
3. Compare privileges with job roles.
4. Review privileged users.
5. Verify MFA.
6. Review access recertification.

---

# 8. Vulnerability Management

## Risk

Critical vulnerabilities may remain unremediated and be exploited by attackers.

## CIS Control

**Control 7 — Continuous Vulnerability Management**

## Controls

* Vulnerability scanning
* Risk-based prioritization
* Patch management
* Remediation SLAs
* Exception management

## Evidence

* Nessus reports
* Vulnerability dashboards
* Patch compliance reports
* Remediation tickets
* Exception approvals

## Testing

1. Obtain the current vulnerability report.
2. Identify critical and high-risk vulnerabilities.
3. Compare vulnerabilities against remediation records.
4. Review SLA compliance.
5. Identify overdue vulnerabilities.
6. Review compensating controls.

## Example Finding

> Critical vulnerabilities remain open beyond the defined remediation timeline.

## Recommended Action

Prioritize remediation of critical vulnerabilities and establish management-approved exceptions for vulnerabilities that cannot be remediated within the required timeframe.

---

# 9. Audit Log Management

## Risk

Security events may not be detected or investigated because required logs are unavailable.

## CIS Control

**Control 8 — Audit Log Management**

## Controls

* Centralized logging
* SIEM integration
* Log retention
* Time synchronization
* Log monitoring
* Protection against log tampering

## Evidence

* SIEM reports
* System logs
* Log retention settings
* Time synchronization reports

## Testing

1. Identify critical systems.
2. Verify logging is enabled.
3. Verify logs are sent to the SIEM where required.
4. Check retention periods.
5. Review selected security events.
6. Verify investigation evidence.

---

# 10. Email and Web Browser Protection

## Risk

Users may be compromised through phishing emails or malicious websites.

## CIS Control

**Control 9 — Email and Web Browser Protections**

## Controls

* Email filtering
* Anti-phishing controls
* Attachment scanning
* URL filtering
* Browser security configuration

## Evidence

* Email security reports
* Phishing reports
* Web filtering reports
* Gateway configuration

## Testing

1. Review email security configuration.
2. Verify malicious attachment filtering.
3. Review phishing protection.
4. Verify web filtering.
5. Analyze phishing simulation results.

---

# 11. Malware Defenses

## Risk

Malware may infect endpoints and compromise systems.

## CIS Control

**Control 10 — Malware Defenses**

## Controls

* EDR
* Antivirus
* Malware detection
* Automated isolation
* Centralized monitoring

## Evidence

* EDR reports
* Antivirus dashboards
* Malware alerts
* Endpoint compliance reports

## Testing

1. Obtain endpoint security coverage reports.
2. Identify devices without active protection.
3. Review malware detections.
4. Verify remediation actions.
5. Review outdated security definitions.

---

# 12. Data Recovery

## Risk

Ransomware or system failures may result in permanent data loss.

## CIS Control

**Control 11 — Data Recovery**

## Controls

* Automated backups
* Backup monitoring
* Isolated backups
* Backup retention
* Restoration testing

## Evidence

* Backup reports
* Backup logs
* Restoration test results
* Disaster recovery reports

## Testing

1. Identify critical systems.
2. Verify backup configuration.
3. Review backup success rates.
4. Identify failed backups.
5. Review restoration tests.
6. Verify recovery requirements.

---

# 13. Network Infrastructure Management

## Risk

Poorly secured network devices may allow unauthorized access or lateral movement.

## CIS Control

**Control 12 — Network Infrastructure Management**

## Controls

* Network asset inventory
* Secure device configuration
* Firewall management
* Network segmentation
* Configuration backups

## Evidence

* Network diagrams
* Router configurations
* Switch configurations
* Firewall rules
* Configuration backups

## Testing

1. Obtain network device inventory.
2. Verify device ownership.
3. Review secure configurations.
4. Check for unnecessary services.
5. Review firewall rules.
6. Verify configuration backups.

---

# 14. Network Monitoring and Defense

## Risk

Malicious network activity may not be detected promptly.

## CIS Control

**Control 13 — Network Monitoring and Defense**

## Controls

* IDS/IPS
* Network monitoring
* Traffic analysis
* Firewall monitoring
* Network detection

## Evidence

* IDS/IPS reports
* Firewall logs
* Network monitoring reports
* SIEM alerts

## Testing

1. Identify critical network segments.
2. Verify monitoring coverage.
3. Review security alerts.
4. Verify alert investigation.
5. Check escalation and remediation.

---

# 15. Security Awareness Training

## Risk

Employees may inadvertently expose the organization to cybersecurity threats.

## CIS Control

**Control 14 — Security Awareness and Skills Training**

## Controls

* Security awareness training
* Phishing simulations
* Role-based security training
* Policy awareness
* Training completion tracking

## Evidence

* Training reports
* Phishing simulation results
* Awareness materials
* Policy acknowledgements

## Testing

1. Obtain the employee population.
2. Review training completion.
3. Identify overdue training.
4. Review phishing results.
5. Verify corrective actions.

---

# 16. Service Provider Management

## Risk

Third-party providers may introduce cybersecurity vulnerabilities.

## CIS Control

**Control 15 — Service Provider Management**

## Controls

* Vendor risk assessments
* Security due diligence
* Contractual security requirements
* Supplier reviews
* Third-party access management

## Evidence

* Vendor assessments
* Contracts
* Security questionnaires
* Supplier review reports
* Third-party access listings

## Testing

1. Obtain the critical supplier register.
2. Identify high-risk providers.
3. Review security assessments.
4. Verify contractual requirements.
5. Review supplier access.
6. Verify periodic reviews.

---

# 17. Application Security

## Risk

Application vulnerabilities may be exploited to compromise systems or data.

## CIS Control

**Control 16 — Application Software Security**

## Controls

* Secure development lifecycle
* Code review
* Application security testing
* Vulnerability management
* Secure deployment
* Change controls

## Evidence

* SAST/DAST reports
* Code review records
* Penetration testing
* Change tickets
* Vulnerability reports

## Testing

1. Select critical applications.
2. Review security requirements.
3. Verify application security testing.
4. Review identified vulnerabilities.
5. Verify remediation.
6. Review deployment approvals.

---

# 18. Incident Response Management

## Risk

Security incidents may not be contained or resolved promptly.

## CIS Control

**Control 17 — Incident Response Management**

## Controls

* Incident response plan
* Incident classification
* Escalation matrix
* Response procedures
* Incident exercises
* Post-incident reviews

## Evidence

* Incident response plan
* Incident tickets
* Investigation reports
* Exercise results
* Root cause analysis

## Testing

1. Select a sample of security incidents.
2. Review incident classification.
3. Verify response timelines.
4. Review investigation.
5. Verify escalation.
6. Review containment.
7. Confirm closure and lessons learned.

---

# 19. Penetration Testing

## Risk

Security weaknesses may remain unidentified until exploited by attackers.

## CIS Control

**Control 18 — Penetration Testing**

## Controls

* External penetration testing
* Internal penetration testing
* Application penetration testing
* Network penetration testing
* Remediation tracking
* Retesting

## Evidence

* Penetration testing reports
* Vulnerability findings
* Remediation records
* Retest reports

## Testing

1. Review the penetration testing schedule.
2. Verify scope covers critical assets.
3. Review findings.
4. Verify remediation tracking.
5. Confirm high-risk findings were addressed.
6. Review retest results.

---

# 20. CIS Control Testing Matrix

| CIS Control | Risk Area                   | Example Control          | Evidence               | Testing                        |
| ----------- | --------------------------- | ------------------------ | ---------------------- | ------------------------------ |
| 1           | Unknown assets              | Asset inventory          | Asset register         | Reconcile asset sources        |
| 2           | Unauthorized software       | Software inventory       | Software report        | Identify unauthorized software |
| 3           | Data exposure               | Data protection          | DLP/encryption reports | Review sensitive data controls |
| 4           | Insecure configuration      | Secure baseline          | Configuration reports  | Compare systems to baseline    |
| 5           | Account compromise          | Account management       | AD reports             | Review account lifecycle       |
| 6           | Excessive access            | Access management        | Access reviews         | Sample user access             |
| 7           | Vulnerabilities             | Vulnerability management | Nessus report          | Review overdue vulnerabilities |
| 8           | Missing logs                | Audit logging            | SIEM reports           | Test logging coverage          |
| 9           | Phishing                    | Email protection         | Email reports          | Review filtering controls      |
| 10          | Malware                     | Endpoint protection      | EDR reports            | Test endpoint coverage         |
| 11          | Data loss                   | Recovery                 | Backup reports         | Test restoration evidence      |
| 12          | Network compromise          | Network management       | Device configurations  | Review configurations          |
| 13          | Network threats             | Network monitoring       | IDS/IPS reports        | Review alerts                  |
| 14          | Human error                 | Awareness                | Training reports       | Test completion                |
| 15          | Third-party risk            | Supplier security        | Vendor assessments     | Review critical suppliers      |
| 16          | Application vulnerabilities | Secure development       | Security test reports  | Review application testing     |
| 17          | Incident response           | Incident management      | Incident records       | Sample incidents               |
| 18          | Security weaknesses         | Pen testing              | Pentest reports        | Review remediation             |

---

# 21. Example IT Risk Tracker Entry

## Risk

Critical vulnerabilities may remain unremediated beyond defined timelines, exposing systems to exploitation.

## CIS Control

**Control 7 — Continuous Vulnerability Management**

## Control

Critical and high-risk vulnerabilities are identified through regular scanning, prioritized according to risk, and remediated within defined SLAs.

## Evidence

* Vulnerability reports
* Patch reports
* Remediation tickets
* Exception approvals

## Testing Result

Several critical vulnerabilities were identified beyond the defined remediation timeline.

## Effectiveness

**Partially Effective**

The vulnerability management process is established, but remediation is not consistently completed within the required timelines.

## Treatment

**Mitigate**

## Recommended Action

Implement enhanced tracking and escalation for overdue vulnerabilities and ensure formally approved exceptions are maintained for vulnerabilities that cannot be remediated within the required timeframe.

---

# 22. Key Takeaway

CIS Controls are most useful when converted into measurable, testable safeguards.

The practical model is:

```text
Cybersecurity Risk
        ↓
CIS Control
        ↓
Safeguard
        ↓
Evidence
        ↓
Control Testing
        ↓
Exception
        ↓
Effectiveness
        ↓
Risk Treatment
        ↓
Remediation
```

This makes CIS Controls highly suitable for cybersecurity assessments, IT Risk, RCSA, IT audit, and security improvement programs.
