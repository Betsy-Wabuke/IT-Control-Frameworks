# ISO/IEC 27001 Control Examples

## 1. Purpose

This document provides practical examples of information-security risks and controls that can be assessed using an ISO/IEC 27001-aligned approach.

The objective is to connect information-security requirements with:

**Risk → Control → Evidence → Testing → Effectiveness → Remediation**

---

# 2. Access Control

## Risk

Unauthorized users may gain access to systems, applications, or sensitive information.

## Control Objective

Ensure access to information and systems is restricted to authorized users based on business requirements.

## Controls

* User access approval
* Role-based access control
* Least privilege
* Access reviews
* User provisioning and deprovisioning
* Segregation of duties

## Evidence

* Access request forms
* Approval records
* User listings
* Access review reports
* HR records
* Access removal records

## Testing Procedure

1. Obtain the system user listing.
2. Select a sample of users.
3. Verify that access was formally requested and approved.
4. Compare access privileges against job responsibilities.
5. Review evidence of periodic access reviews.
6. Check terminated users.
7. Verify timely removal of access.
8. Document exceptions.

## Effectiveness

**Effective:** Access is appropriately authorized, reviewed, and removed.

**Partially Effective:** Controls exist but exceptions or delays are identified.

**Ineffective:** Users have access without appropriate authorization or review.

---

# 3. Identity and Authentication

## Risk

Weak authentication mechanisms may allow unauthorized individuals to compromise user accounts.

## Control Objective

Ensure users are appropriately authenticated before accessing information systems.

## Controls

* Strong password requirements
* Multi-factor authentication
* Account lockout
* Secure authentication mechanisms
* Unique user IDs
* Authentication monitoring

## Evidence

* Authentication policies
* Active Directory configuration
* MFA reports
* Authentication logs
* System configuration screenshots

## Testing Procedure

1. Review authentication policies.
2. Verify password requirements.
3. Verify MFA implementation for critical systems.
4. Review account lockout configuration.
5. Check whether shared user accounts exist.
6. Review authentication logs for unusual activity.

---

# 4. Privileged Access

## Risk

Excessive or shared administrative access may result in unauthorized system changes and lack of accountability.

## Control Objective

Ensure privileged access is restricted, authorized, monitored, and attributable to individual users.

## Controls

* Named administrator accounts
* Privileged Access Management
* MFA
* Privileged access approval
* Session monitoring
* Administrative activity logging
* Periodic privileged access reviews

## Evidence

* PAM reports
* Privileged account listings
* Access approvals
* Audit logs
* Session recordings
* Access review reports

## Testing Procedure

1. Obtain privileged account listings.
2. Identify shared administrative accounts.
3. Verify each account has a named owner.
4. Confirm privileged access approval.
5. Review MFA configuration.
6. Verify administrative activities are logged.
7. Review privileged access recertification.

## Example Finding

> Shared administrative accounts were identified on critical systems, limiting individual accountability and traceability of privileged activities.

## Recommended Action

Eliminate shared administrative accounts and ensure privileged activities are performed using uniquely assigned named accounts. Where technically unavoidable, implement compensating controls such as PAM, MFA, session monitoring, and enhanced logging.

---

# 5. Asset Management

## Risk

The organization may be unable to identify or protect all IT assets because asset records are incomplete or outdated.

## Control Objective

Maintain an accurate inventory of information assets and associated ownership.

## Controls

* IT asset register
* Asset ownership
* Asset classification
* Periodic asset reconciliation
* Asset lifecycle management

## Evidence

* Asset register
* CMDB
* GLPI records
* Endpoint management reports
* Network discovery reports
* Asset disposal records

## Testing Procedure

1. Obtain the IT asset register.
2. Select a sample of assets.
3. Verify assets against physical or technical records.
4. Compare asset inventory with endpoint management data.
5. Verify asset ownership.
6. Identify unregistered assets.
7. Document discrepancies.

---

# 6. Vulnerability and Patch Management

## Risk

Unpatched vulnerabilities may be exploited by attackers.

## Control Objective

Identify, assess, prioritize, and remediate vulnerabilities within defined timelines.

## Controls

* Vulnerability scanning
* Patch management
* Risk-based prioritization
* Patch deployment
* Exception management
* Vulnerability monitoring

## Evidence

* Vulnerability reports
* Nessus reports
* Endpoint management reports
* Patch compliance reports
* Remediation tickets
* Approved exceptions

## Testing Procedure

1. Obtain the latest vulnerability report.
2. Identify critical and high-risk vulnerabilities.
3. Compare vulnerabilities against patch records.
4. Verify remediation timelines.
5. Identify overdue vulnerabilities.
6. Review approved exceptions.
7. Determine whether compensating controls exist.

---

# 7. Logging and Monitoring

## Risk

Security events may not be detected or investigated because system activities are not adequately logged and monitored.

## Control Objective

Ensure relevant security events are logged, monitored, retained, and investigated.

## Controls

* Centralized logging
* SIEM
* Security monitoring
* Log retention
* Alerting
* Log review
* Incident escalation

## Evidence

* SIEM reports
* Log management reports
* Security alerts
* Investigation tickets
* Log retention configuration

## Testing Procedure

1. Identify critical systems.
2. Verify that logs are generated.
3. Confirm logs are sent to the SIEM where required.
4. Review sample security alerts.
5. Verify alerts were investigated.
6. Check log retention.
7. Compare security events between source systems and the SIEM.

---

# 8. Incident Management

## Risk

Security incidents may not be detected, investigated, or resolved within appropriate timelines.

## Control Objective

Ensure information-security incidents are appropriately reported, assessed, investigated, escalated, and resolved.

## Controls

* Incident response procedures
* Incident classification
* Escalation procedures
* Incident logging
* Root cause analysis
* Lessons learned

## Evidence

* Incident tickets
* Incident reports
* Investigation records
* Root cause analysis
* Escalation records
* Closure documentation

## Testing Procedure

1. Select a sample of security incidents.
2. Verify incident classification.
3. Review response and resolution times.
4. Verify investigation evidence.
5. Review escalation.
6. Confirm root cause analysis where applicable.
7. Check closure documentation.

---

# 9. Backup and Recovery

## Risk

Failure to maintain reliable backups may result in permanent data loss or prolonged service disruption.

## Control Objective

Ensure critical information is backed up and can be recovered when required.

## Controls

* Scheduled backups
* Backup monitoring
* Backup encryption
* Backup retention
* Offsite backups
* Restoration testing

## Evidence

* Backup reports
* Backup logs
* Restoration test results
* Disaster recovery test reports
* Backup schedules

## Testing Procedure

1. Identify critical systems.
2. Verify backup schedules.
3. Review backup success and failure reports.
4. Check backup retention.
5. Verify protection of backup data.
6. Review restoration testing.
7. Investigate failed backups.

---

# 10. Cryptography

## Risk

Sensitive information may be exposed because appropriate encryption mechanisms are not implemented.

## Control Objective

Protect sensitive information through appropriate cryptographic controls.

## Controls

* Encryption at rest
* Encryption in transit
* TLS
* Key management
* Secure key storage
* Cryptographic standards

## Evidence

* Encryption configurations
* TLS certificates
* Key-management records
* System configurations
* Security policies

## Testing Procedure

1. Identify systems handling sensitive information.
2. Verify encryption at rest.
3. Verify encryption in transit.
4. Review TLS configurations.
5. Review key-management practices.
6. Identify weak or expired certificates.

---

# 11. Change Management

## Risk

Unauthorized or inadequately tested changes may introduce vulnerabilities or service disruption.

## Control Objective

Ensure information systems are changed through controlled, authorized, tested, and documented processes.

## Controls

* Change requests
* Change approval
* Testing
* Segregation of duties
* Backout procedures
* Emergency change procedures

## Evidence

* Change tickets
* Approval records
* Test results
* Deployment records
* Emergency change records

## Testing Procedure

1. Select a sample of changes.
2. Verify change requests.
3. Confirm approval.
4. Review testing evidence.
5. Verify implementation authorization.
6. Review emergency changes.
7. Check post-implementation review.

---

# 12. Supplier Security

## Risk

Third-party suppliers may introduce information-security vulnerabilities or expose organizational information.

## Control Objective

Ensure information-security risks associated with suppliers are identified, assessed, and managed.

## Controls

* Vendor due diligence
* Security requirements in contracts
* Supplier risk assessments
* Periodic supplier reviews
* Third-party access controls
* Supplier incident reporting requirements

## Evidence

* Vendor assessments
* Contracts
* SLAs
* Security questionnaires
* Supplier review reports
* Access listings

## Testing Procedure

1. Obtain the supplier register.
2. Identify critical suppliers.
3. Review supplier risk assessments.
4. Verify security requirements in contracts.
5. Review supplier access.
6. Verify periodic supplier reviews.
7. Identify outstanding security issues.

---

# 13. Security Awareness

## Risk

Employees may unintentionally expose the organization to cybersecurity threats due to insufficient security awareness.

## Control Objective

Ensure employees understand their information-security responsibilities.

## Controls

* Security awareness training
* Phishing simulations
* Acceptable-use policies
* Security communications
* Training completion monitoring

## Evidence

* Training attendance reports
* Learning management system reports
* Phishing simulation results
* Awareness materials
* Policy acknowledgements

## Testing Procedure

1. Obtain the employee population.
2. Review training completion rates.
3. Identify employees who have not completed required training.
4. Review phishing simulation results.
5. Verify follow-up actions.
6. Review policy acknowledgement records.

---

# 14. Business Continuity

## Risk

A major IT disruption may prevent critical services from operating within acceptable timeframes.

## Control Objective

Ensure information-security and technology continuity requirements are incorporated into business continuity and disaster recovery arrangements.

## Controls

* Business continuity plans
* Disaster recovery plans
* Recovery Time Objectives
* Recovery Point Objectives
* Disaster recovery testing
* Alternative processing arrangements

## Evidence

* BCP documents
* DR plans
* DR test reports
* RTO/RPO documentation
* Recovery test results

## Testing Procedure

1. Identify critical systems.
2. Review their RTO and RPO.
3. Verify documented recovery procedures.
4. Review disaster recovery testing.
5. Check whether recovery objectives were achieved.
6. Document deficiencies.

---

# 15. Control Assessment Matrix

| Control Area             | Risk                        | Control                | Evidence         | Testing                        |
| ------------------------ | --------------------------- | ---------------------- | ---------------- | ------------------------------ |
| Access Control           | Unauthorized access         | Access approval        | Access requests  | Sample user access             |
| Privileged Access        | Shared accounts             | Named accounts/PAM     | PAM reports      | Review privileged accounts     |
| Asset Management         | Unknown assets              | Asset inventory        | Asset register   | Reconcile assets               |
| Vulnerability Management | Exploitable vulnerabilities | Vulnerability scanning | Nessus reports   | Review overdue vulnerabilities |
| Logging                  | Undetected events           | SIEM monitoring        | SIEM reports     | Trace security alerts          |
| Incident Management      | Delayed response            | Incident management    | Incident tickets | Test incident samples          |
| Backup                   | Data loss                   | Scheduled backups      | Backup reports   | Review backup success          |
| Cryptography             | Data exposure               | Encryption             | Configuration    | Verify encryption              |
| Change Management        | Unauthorized changes        | Change approval        | Change tickets   | Sample changes                 |
| Supplier Security        | Third-party risk            | Vendor assessment      | Vendor reviews   | Test critical suppliers        |
| Awareness                | Human error                 | Security training      | Training reports | Review completion              |
| Business Continuity      | Service disruption          | DR testing             | DR reports       | Review test results            |

---

# 16. Control Effectiveness

### Effective

The control is appropriately designed and operates consistently.

### Partially Effective

The control exists but has weaknesses, exceptions, or inconsistent execution.

### Ineffective

The control is absent, inadequately designed, or does not operate as intended.

---

# 17. IT Risk Tracker Integration

The results of ISO/IEC 27001 control testing can feed directly into an IT Risk Tracker.

Example:

| Risk                     | Control                   | Effectiveness       | Treatment | Action                       |
| ------------------------ | ------------------------- | ------------------- | --------- | ---------------------------- |
| Shared admin accounts    | Named privileged accounts | Partially Effective | Mitigate  | Eliminate shared accounts    |
| Critical vulnerabilities | Patch management          | Partially Effective | Mitigate  | Remediate overdue patches    |
| SIEM monitoring gaps     | Centralized logging       | Ineffective         | Mitigate  | Resolve log integration gaps |
| Excessive access         | Access reviews            | Partially Effective | Mitigate  | Remove inappropriate access  |
| Data loss                | Backup and recovery       | Effective           | Accept    | Continue monitoring          |

---

# 18. Key Takeaway

ISO/IEC 27001 provides a strong information-security perspective for IT Risk and control assessments.

The practical approach is:

```text
Information-Security Risk
        ↓
Control Objective
        ↓
Security Control
        ↓
Evidence
        ↓
Control Testing
        ↓
Effectiveness
        ↓
Finding
        ↓
Risk Treatment
        ↓
Remediation
        ↓
Continuous Improvement
```

This approach allows ISO/IEC 27001 controls to be integrated into RCSA, IT Risk Registers, IT Risk Trackers, IT Audit, and cybersecurity governance activities.
