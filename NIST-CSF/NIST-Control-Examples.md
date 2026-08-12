# NIST CSF Control Examples

## 1. Purpose

This document provides practical examples of cybersecurity risks and controls mapped to the six NIST CSF 2.0 Functions.

The objective is to demonstrate how NIST CSF can be applied to:

* IT Risk
* RCSA
* Cybersecurity assessments
* Control testing
* IT audit
* Risk remediation

---

# 2. Asset Management

## Risk

The organization may not identify unauthorized or unmanaged devices connected to its environment.

## NIST Function

**Identify**

## Control

Maintain an accurate inventory of hardware, software, applications, and critical information assets.

## Evidence

* Asset register
* CMDB
* GLPI records
* Endpoint management reports
* Network discovery reports

## Testing

1. Obtain the asset register.
2. Compare it against endpoint management records.
3. Compare it against network discovery results.
4. Identify discrepancies.
5. Investigate unmanaged assets.
6. Document exceptions.

## Effectiveness

**Partially Effective** if unidentified or unregistered assets are found.

---

# 3. Access Management

## Risk

Unauthorized users may gain access to critical systems.

## NIST Function

**Protect**

## Controls

* MFA
* Least privilege
* Role-based access
* Access approvals
* Periodic access reviews
* User deprovisioning

## Evidence

* User access reports
* MFA reports
* Access approvals
* Access review records
* HR termination reports

## Testing

1. Select a sample of users.
2. Verify access approval.
3. Compare privileges with job roles.
4. Verify MFA.
5. Review terminated users.
6. Verify timely deactivation.

---

# 4. Privileged Access

## Risk

Shared administrative accounts may result in unauthorized system changes without individual accountability.

## NIST Function

**Protect**

## Controls

* Named privileged accounts
* PAM
* MFA
* Privileged access approval
* Session monitoring
* Audit logging

## Evidence

* PAM reports
* Privileged account listings
* Access approvals
* Session logs
* Audit trails

## Testing

1. Obtain privileged account listings.
2. Identify shared accounts.
3. Verify account ownership.
4. Review access approval.
5. Verify privileged activity logging.
6. Review PAM controls.

## Possible Rating

**Partially Effective**

Where PAM exists but shared administrative accounts remain in use.

---

# 5. Vulnerability Management

## Risk

Unidentified or unremediated vulnerabilities may be exploited.

## NIST Function

**Identify / Protect**

## Controls

* Vulnerability scanning
* Patch management
* Risk-based prioritization
* Remediation SLAs
* Exception management

## Evidence

* Nessus reports
* Vulnerability dashboards
* Patch reports
* Remediation tickets
* Exception approvals

## Testing

1. Obtain the vulnerability report.
2. Identify critical and high-risk vulnerabilities.
3. Review remediation status.
4. Compare remediation against SLA.
5. Investigate overdue vulnerabilities.
6. Review approved exceptions.

---

# 6. Security Monitoring

## Risk

Cybersecurity events may not be detected promptly.

## NIST Function

**Detect**

## Controls

* SIEM
* EDR
* Network monitoring
* Log monitoring
* Security alerts
* Threat detection

## Evidence

* SIEM dashboards
* EDR reports
* Security alerts
* System logs
* Monitoring reports

## Testing

1. Identify critical systems.
2. Verify that security logs are generated.
3. Verify integration with monitoring platforms.
4. Select security alerts.
5. Verify investigation.
6. Confirm appropriate escalation.

---

# 7. Incident Response

## Risk

Cybersecurity incidents may not be contained or investigated promptly.

## NIST Function

**Respond**

## Controls

* Incident response plan
* Incident classification
* Escalation procedures
* Containment procedures
* Investigation procedures
* Incident communication

## Evidence

* Incident response plan
* Incident tickets
* Investigation reports
* Escalation records
* Root cause analysis

## Testing

1. Select a sample of security incidents.
2. Verify classification.
3. Review response time.
4. Review investigation.
5. Verify escalation.
6. Confirm containment.
7. Review closure and lessons learned.

---

# 8. Backup and Recovery

## Risk

A cyberattack or system failure may cause permanent data loss.

## NIST Function

**Recover**

## Controls

* Scheduled backups
* Backup monitoring
* Offline/offsite backups
* Backup encryption
* Restoration testing
* Disaster recovery testing

## Evidence

* Backup reports
* Backup logs
* Restoration test results
* DR test reports

## Testing

1. Identify critical systems.
2. Verify backup schedules.
3. Review backup success rates.
4. Identify failed backups.
5. Review restoration testing.
6. Verify recovery objectives.

---

# 9. Security Awareness

## Risk

Employees may fall victim to phishing or other social-engineering attacks.

## NIST Function

**Protect**

## Controls

* Security awareness training
* Phishing simulations
* Security communications
* Acceptable-use policies
* Training completion monitoring

## Evidence

* Training reports
* Phishing simulation results
* Awareness materials
* Policy acknowledgements

## Testing

1. Obtain the employee population.
2. Review training completion.
3. Identify outstanding training.
4. Review phishing simulation results.
5. Verify follow-up actions.

---

# 10. Configuration Management

## Risk

Insecure system configurations may increase the attack surface.

## NIST Function

**Protect**

## Controls

* Secure configuration standards
* Configuration baselines
* Hardening standards
* Configuration monitoring
* Periodic reviews

## Evidence

* Configuration baselines
* System configuration reports
* Hardening checklists
* Vulnerability reports

## Testing

1. Select a sample of systems.
2. Obtain configuration standards.
3. Compare actual configurations against approved baselines.
4. Identify deviations.
5. Verify remediation.

---

# 11. Security Event Analysis

## Risk

Security alerts may be generated but not properly investigated.

## NIST Function

**Detect**

## Controls

* Alert triage
* SIEM correlation
* Security investigation
* Threat intelligence
* Escalation procedures

## Evidence

* SIEM alerts
* Investigation tickets
* Analyst notes
* Escalation records

## Testing

1. Select security alerts.
2. Verify analyst review.
3. Confirm investigation.
4. Determine whether the alert was correctly classified.
5. Verify escalation where required.
6. Check closure evidence.

---

# 12. Communications During Incidents

## Risk

Poor communication during a cyber incident may delay containment and recovery.

## NIST Function

**Respond**

## Controls

* Incident communication plan
* Escalation matrix
* Defined notification requirements
* Management reporting
* Stakeholder communication

## Evidence

* Communication plans
* Escalation matrix
* Incident reports
* Notification records

## Testing

Review a sample of incidents and verify whether the required stakeholders were notified within defined timelines.

---

# 13. Recovery Planning

## Risk

The organization may be unable to restore critical systems following a major cybersecurity incident.

## NIST Function

**Recover**

## Controls

* Disaster recovery plans
* Business continuity plans
* Recovery procedures
* RTO/RPO requirements
* Recovery testing

## Evidence

* DR plans
* BCP documents
* DR test reports
* RTO/RPO documentation
* Recovery records

## Testing

1. Identify critical systems.
2. Review RTO and RPO requirements.
3. Review recovery procedures.
4. Inspect DR test results.
5. Verify whether recovery objectives were achieved.
6. Document gaps.

---

# 14. Control Assessment Matrix

| Risk                    | Control                  | NIST Function    | Evidence              | Testing                        |
| ----------------------- | ------------------------ | ---------------- | --------------------- | ------------------------------ |
| Unknown assets          | Asset inventory          | Identify         | Asset register        | Reconcile asset sources        |
| Unauthorized access     | MFA/access control       | Protect          | Access reports        | Sample user accounts           |
| Shared admin accounts   | PAM/named accounts       | Protect          | PAM reports           | Review privileged accounts     |
| Unpatched systems       | Vulnerability management | Identify/Protect | Vulnerability report  | Review overdue vulnerabilities |
| Missed security events  | SIEM/EDR                 | Detect           | SIEM reports          | Trace security alerts          |
| Delayed response        | Incident response        | Respond          | Incident tickets      | Test incident samples          |
| Data loss               | Backup/DR                | Recover          | Backup reports        | Test restoration evidence      |
| Phishing                | Awareness training       | Protect          | Training reports      | Review training completion     |
| Insecure configurations | Configuration management | Protect          | Configuration reports | Compare against baseline       |

---

# 15. Control Effectiveness

### Effective

The control is appropriately designed and operates consistently.

### Partially Effective

The control exists but has weaknesses, exceptions, or inconsistent execution.

### Ineffective

The control is absent, poorly designed, or not operating as intended.

---

# 16. Example IT Risk Tracker Entry

### Risk

Security events generated by endpoint security tools may not be detected and investigated through the organization's centralized SIEM.

### Control

Security events from critical security tools are integrated into the SIEM and monitored by the security team.

### NIST Function

**Detect**

### Evidence

* SIEM reports
* Endpoint security reports
* Security alerts
* Incident tickets

### Testing

Compare security events generated by endpoint security tools against SIEM records and verify that identified events were investigated and appropriately remediated.

### Finding

Some endpoint security events were identified without corresponding SIEM records demonstrating centralized detection and investigation.

### Effectiveness

**Partially Effective / Ineffective**, depending on the extent and significance of the integration gap.

### Recommended Action

Review and remediate SIEM integrations for critical security tools and establish monitoring to confirm that security events are consistently ingested, detected, investigated, and tracked to resolution.

---

# 17. NIST CSF Control Testing Model

```text
Risk
 ↓
NIST CSF Function
 ↓
Control Objective
 ↓
Control
 ↓
Evidence
 ↓
Testing
 ↓
Exception
 ↓
Control Effectiveness
 ↓
Residual Risk
 ↓
Remediation
```

---

# 18. Key Takeaway

NIST CSF is most useful when its Functions are translated into measurable cybersecurity controls.

The practical objective is:

**Govern cybersecurity risk → Identify assets and threats → Protect systems → Detect events → Respond to incidents → Recover operations.**

This creates a continuous cybersecurity risk-management cycle that can be integrated into IT Risk, RCSA, IT Audit, and cybersecurity monitoring processes.
