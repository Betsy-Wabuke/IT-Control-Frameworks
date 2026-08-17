# IT General Controls (ITGC) — Control Categories

## 1. Overview

IT General Controls can be grouped into major control areas that support the security, reliability, and effective operation of an organization's IT environment.

This repository uses five primary ITGC categories:

1. Access Management
2. Change Management
3. IT Operations
4. Backup and Recovery
5. Security Management

---

# 2. Access Management

## 2.1 Objective

Ensure that access to systems, applications, databases, networks, and information is:

* Authorized
* Appropriate
* Restricted according to business need
* Periodically reviewed
* Removed when no longer required
* Attributable to an individual user

## 2.2 Key Risks

* Unauthorized access
* Excessive user privileges
* Orphaned accounts
* Former employees retaining access
* Shared or generic accounts
* Inappropriate privileged access
* Lack of segregation of duties

## 2.3 Typical Controls

### User Provisioning

Access is granted only after documented authorization.

### User Deprovisioning

Access is removed promptly when employment or business need ends.

### User Access Reviews

User access is periodically reviewed and recertified.

### Privileged Access Management

Administrative access is restricted, approved, monitored, and attributable to named individuals.

### Multi-Factor Authentication

MFA is implemented for systems and accounts where required.

### Segregation of Duties

Conflicting responsibilities are appropriately separated.

### Generic Account Management

Generic or shared accounts are restricted and subject to compensating controls where they cannot technically be eliminated.

## 2.4 Evidence

* Access requests
* Approval records
* Active Directory reports
* Application user listings
* PAM reports
* Access review reports
* HR joiner/mover/leaver records
* MFA reports
* Audit logs

## 2.5 Example Risk

> Shared administrative accounts may be used to perform changes on critical systems without sufficient individual accountability.

## 2.6 Example Control

> All privileged activities must be performed using uniquely assigned named administrator accounts. Where shared accounts are technically unavoidable, appropriate compensating controls must be implemented to maintain individual accountability and traceability.

---

# 3. Change Management

## 3.1 Objective

Ensure changes to IT systems, applications, infrastructure, configurations, and databases are appropriately:

* Requested
* Assessed
* Tested
* Approved
* Implemented
* Documented
* Reviewed

## 3.2 Key Risks

* Unauthorized changes
* Untested changes
* System outages
* Introduction of vulnerabilities
* Data integrity issues
* Inadequate segregation of duties
* Changes that cannot be reversed

## 3.3 Typical Controls

### Change Request

Changes are formally documented before implementation.

### Change Risk Assessment

Changes are assessed according to potential impact and risk.

### Change Approval

Appropriate personnel authorize changes before implementation.

### Testing

Changes are tested in an appropriate environment before production deployment.

### Segregation of Duties

Where practical, developers or requestors should not independently approve and implement their own changes.

### Emergency Changes

Emergency changes follow a defined emergency change process and receive retrospective review where applicable.

### Backout Procedures

Changes have appropriate rollback or recovery procedures where necessary.

### Post-Implementation Review

Material changes are reviewed after implementation.

## 3.4 Evidence

* Change tickets
* Approval records
* Test results
* Deployment records
* Release notes
* Backout plans
* Emergency change records
* Post-implementation reviews

## 3.5 Example Risk

> Unauthorized or inadequately tested changes may result in system outages, security vulnerabilities, or data integrity issues.

---

# 4. IT Operations

## 4.1 Objective

Ensure day-to-day IT operations are performed consistently, monitored appropriately, and supported by documented procedures.

## 4.2 Key Risks

* Service disruption
* Processing failures
* Delayed incident resolution
* Job failures
* Inadequate monitoring
* Operational errors
* Capacity constraints

## 4.3 Typical Controls

### Incident Management

Incidents are logged, classified, assigned, investigated, escalated, and resolved.

### Problem Management

Recurring or significant incidents are investigated to identify root causes.

### Job Scheduling

Critical automated jobs are appropriately scheduled and monitored.

### System Monitoring

Critical systems and infrastructure are monitored for availability and performance.

### Capacity Management

Capacity is monitored to identify potential resource constraints.

### Operational Procedures

Critical IT activities are documented and performed according to approved procedures.

## 4.4 Evidence

* Incident tickets
* Incident reports
* SLA reports
* Job schedules
* Batch processing reports
* Monitoring dashboards
* Capacity reports
* Operating procedures
* Escalation records

## 4.5 Example Risk

> Failure to monitor critical system processes may result in prolonged service disruption or delayed detection of operational failures.

---

# 5. Backup and Recovery

## 5.1 Objective

Ensure organizational data and IT services can be recovered following:

* System failures
* Cybersecurity incidents
* Data corruption
* Hardware failures
* Operational errors
* Major disruptions

## 5.2 Key Risks

* Data loss
* Failed backups
* Inability to restore systems
* Inadequate backup retention
* Backup compromise
* Recovery delays

## 5.3 Typical Controls

### Backup Scheduling

Critical systems are backed up according to defined schedules.

### Backup Monitoring

Backup jobs are monitored for success and failure.

### Backup Retention

Backups are retained according to business and regulatory requirements.

### Backup Protection

Backups are protected from unauthorized access, modification, and destruction.

### Restoration Testing

Backups are periodically tested to confirm that data can actually be restored.

### Disaster Recovery Testing

Critical recovery procedures are periodically tested.

## 5.4 Evidence

* Backup schedules
* Backup logs
* Backup success/failure reports
* Restoration test reports
* DR test results
* Backup retention policies
* Recovery procedures

## 5.5 Example Risk

> Failure to maintain reliable and recoverable backups may result in permanent data loss and prolonged service disruption.

---

# 6. Security Management

## 6.1 Objective

Protect IT infrastructure, systems, applications, and information from cybersecurity threats.

## 6.2 Key Risks

* Malware infections
* Exploitation of vulnerabilities
* Unauthorized system changes
* Data breaches
* Security incidents
* Inadequate security monitoring
* Weak security configurations

## 6.3 Typical Controls

### Vulnerability Management

Vulnerabilities are identified, prioritized, tracked, and remediated.

### Patch Management

Security patches are deployed within defined timelines based on risk.

### Malware Protection

Endpoints and servers are protected using appropriate security technologies.

### Security Monitoring

Security events are continuously monitored and investigated.

### Security Incident Management

Security incidents are detected, investigated, contained, escalated, and resolved.

### Security Configuration

Systems are hardened according to approved security baselines.

### Security Awareness

Personnel receive appropriate information-security awareness training.

## 6.4 Evidence

* Vulnerability reports
* Patch reports
* EDR/antivirus reports
* SIEM reports
* Security alerts
* Incident tickets
* Configuration compliance reports
* Security awareness reports

## 6.5 Example Risk

> Unpatched vulnerabilities may be exploited by attackers, resulting in system compromise or data loss.

---

# 7. Cross-Category Control Relationships

ITGC categories are interconnected.

For example:

```text
Access Management
       ↓
Authorized Administrator
       ↓
Change Management
       ↓
Approved System Change
       ↓
IT Operations
       ↓
System Monitoring
       ↓
Security Management
       ↓
Security Event Detection
       ↓
Backup & Recovery
       ↓
Service Restoration
```

A weakness in one category can affect other control areas.

---

# 8. ITGC Risk and Control Matrix

| ITGC Category       | Example Risk                | Typical Control               | Primary Evidence      |
| ------------------- | --------------------------- | ----------------------------- | --------------------- |
| Access Management   | Unauthorized access         | Access approval and review    | Access reports        |
| Access Management   | Shared admin accounts       | Named privileged accounts/PAM | PAM reports           |
| Change Management   | Unauthorized changes        | Change approval               | Change tickets        |
| Change Management   | Untested changes            | Pre-production testing        | Test evidence         |
| IT Operations       | Delayed incident response   | Incident management           | Incident tickets      |
| IT Operations       | Processing failure          | Job monitoring                | Job reports           |
| Backup & Recovery   | Data loss                   | Scheduled backups             | Backup reports        |
| Backup & Recovery   | Failed restoration          | Restoration testing           | Restore test results  |
| Security Management | Exploitable vulnerabilities | Vulnerability management      | Vulnerability reports |
| Security Management | Malware infection           | EDR/antivirus                 | EDR reports           |
| Security Management | Missed threats              | SIEM monitoring               | SIEM reports          |

---

# 9. Control Classification

ITGC controls can also be classified according to their control nature.

## Preventive

Designed to prevent undesirable events.

Examples:

* Access approval
* MFA
* Change approval
* Secure configuration
* Least privilege

## Detective

Designed to identify events or control failures.

Examples:

* Access reviews
* SIEM monitoring
* Vulnerability scanning
* Backup failure monitoring
* Exception reports

## Corrective

Designed to restore or correct conditions after an event.

Examples:

* Account removal
* Security patching
* Incident remediation
* System restoration
* Disaster recovery

---

# 10. ITGC Control Frequency

Controls may operate at different frequencies.

| Frequency     | Example                             |
| ------------- | ----------------------------------- |
| Continuous    | SIEM monitoring                     |
| Daily         | Backup monitoring                   |
| Weekly        | Vulnerability or operational review |
| Monthly       | Patch compliance review             |
| Quarterly     | User access review                  |
| Semi-annually | Privileged access recertification   |
| Annually      | DR testing or policy review         |
| Event-driven  | User provisioning/deprovisioning    |

The appropriate frequency should be determined based on risk, business requirements, regulatory obligations, and the nature of the control.

---

# 11. ITGC Control Testing

A control assessment should consider both:

### Design Effectiveness

Does the control adequately address the identified risk?

### Operating Effectiveness

Does the control actually operate as designed and consistently produce the intended result?

```text
Risk
 ↓
Control Design
 ↓
Implementation
 ↓
Operating Effectiveness
 ↓
Evidence
 ↓
Testing Result
 ↓
Control Rating
```

A control can therefore exist on paper but still be ineffective if it is not consistently operating.

---

# 12. Practical Control Rating

### Effective

The control is appropriately designed, implemented, and operating consistently.

### Partially Effective

The control is implemented and generally operates but has weaknesses, exceptions, or inconsistencies.

### Ineffective

The control is absent, inadequately designed, or fails to operate as intended.

---

# 13. Framework Alignment

ITGCs can be mapped to the frameworks covered earlier in this repository.

| ITGC Category       | COBIT | ISO/IEC 27001 | NIST CSF        | CIS Controls |
| ------------------- | ----- | ------------- | --------------- | ------------ |
| Access Management   | Yes   | Yes           | Protect         | 5, 6         |
| Change Management   | Yes   | Yes           | Protect         | 4, 16        |
| IT Operations       | Yes   | Yes           | Detect, Respond | 8, 13, 17    |
| Backup & Recovery   | Yes   | Yes           | Recover         | 11           |
| Security Management | Yes   | Yes           | Protect, Detect | 7, 8, 10, 13 |

This is a high-level mapping and should be validated against the organization's specific framework version, scope, and control implementation.

---

# 14. Key Takeaway

ITGCs provide a practical foundation for evaluating whether an organization's technology environment is operating securely and reliably.

The five primary areas are:

**Access Management → Change Management → IT Operations → Backup & Recovery → Security Management**

The next stage is to convert these categories into detailed control scenarios and testing procedures so that each ITGC can be assessed using real evidence and linked directly to the IT Risk Tracker.
