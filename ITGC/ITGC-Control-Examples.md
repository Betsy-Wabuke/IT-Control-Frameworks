# IT General Controls — Practical Control Examples

## 1. Purpose

This document provides practical examples of IT General Controls (ITGCs), including:

* IT risks
* Control objectives
* Controls
* Control owners
* Evidence
* Testing procedures
* Findings
* Control effectiveness
* Remediation actions

The objective is to demonstrate how ITGCs can be applied in IT Risk, RCSA, IT Audit, and control-testing activities.

---

# 2. Access Management

## Risk 1 — Unauthorized User Access

### Risk

Unauthorized users may gain access to systems or applications, resulting in data exposure, fraud, unauthorized transactions, or operational disruption.

### Control Objective

Ensure access is granted only to authorized users based on approved business requirements.

### Controls

* Formal access requests
* Management approval
* Role-based access
* Least privilege
* Access reviews
* Joiner-Mover-Leaver controls
* Timely deprovisioning

### Control Owner

IT Access Management / System Administrator / Application Owner

### Evidence

* Access request forms
* Approval records
* User listings
* Access matrices
* HR records
* Deprovisioning records

### Testing

1. Obtain the current user listing.
2. Select a representative sample.
3. Verify access approval for each selected user.
4. Compare assigned access with job responsibilities.
5. Review terminated employees.
6. Verify timely removal of access.
7. Document exceptions.

### Effectiveness

**Effective:** Access is appropriately approved, provisioned, reviewed, and removed.

**Partially Effective:** The process exists but exceptions or delays are identified.

**Ineffective:** Access is routinely granted without authorization or retained after business need ends.

---

# 3. Access Management — Periodic User Access Reviews

## Risk 2 — Excessive or Inappropriate Access

### Risk

Users may retain access that is no longer required due to transfers, role changes, or changes in responsibilities.

### Control Objective

Ensure user access remains appropriate and is periodically reviewed by authorized management.

### Controls

* Quarterly or periodic access reviews
* Access recertification
* Role-based access
* Segregation of duties review
* Removal of inappropriate access

### Evidence

* Access review reports
* User-role matrices
* Management sign-offs
* Access removal tickets
* HR transfer records

### Testing

1. Obtain the access review population.
2. Verify that reviews were performed within the required period.
3. Confirm review by an authorized person.
4. Sample users and assess whether access remains appropriate.
5. Verify remediation of identified exceptions.
6. Confirm review completion.

### Example Finding

> Periodic user access reviews were performed; however, exceptions identified during the review were not consistently removed within the expected timeframe.

### Recommendation

> Establish defined remediation timelines for access-review exceptions and monitor outstanding items to closure.

---

# 4. Privileged Access Management

## Risk 3 — Excessive Privileged Access

### Risk

Users may receive administrative privileges beyond their legitimate job requirements.

### Control Objective

Ensure privileged access is restricted to authorized personnel and granted according to business need.

### Controls

* PAM
* Named administrator accounts
* Least privilege
* Privileged access approval
* MFA
* Periodic privileged access reviews

### Evidence

* PAM reports
* Privileged account listings
* Access approvals
* Access review reports
* MFA reports

### Testing

1. Obtain the privileged account listing.
2. Identify all privileged users.
3. Verify business justification.
4. Confirm approval.
5. Verify MFA.
6. Review periodic privileged access certification.
7. Identify excessive privileges.

---

# 5. Shared Administrative Accounts

## Risk 4 — Lack of Individual Accountability

### Risk

Shared administrative accounts may be used to make changes on critical systems, limiting accountability and traceability.

### Control Objective

Ensure privileged activities can be uniquely attributed to authorized individuals.

### Controls

* Named privileged accounts
* PAM
* MFA
* Session monitoring
* Audit logging
* Privileged access approval
* Periodic privileged access review

### Evidence

* Active Directory reports
* PAM reports
* Application account listings
* Audit trails
* Privileged session logs
* Access review records

### Testing

1. Obtain the privileged account population.
2. Identify generic or shared accounts.
3. Determine whether the accounts are technically necessary.
4. Verify whether named accounts are available.
5. Review PAM coverage.
6. Check whether activities are individually attributable.
7. Review compensating controls for unavoidable shared accounts.
8. Document exceptions.

### Example Finding

> Shared administrative accounts were identified on critical systems. The use of these accounts limits the ability to attribute system changes to individual administrators.

### Recommended Action

> Eliminate shared administrative accounts and ensure privileged activities are performed through uniquely assigned named accounts. Where shared accounts are technically unavoidable, implement compensating controls such as PAM, MFA, session monitoring, and enhanced audit logging.

### Example Effectiveness

**Partially Effective** where privileged-access controls exist but shared administrative accounts remain in use.

---

# 6. Change Management

## Risk 5 — Unauthorized Changes

### Risk

Unauthorized changes to production systems may introduce security vulnerabilities, system outages, or data integrity issues.

### Control Objective

Ensure production changes are formally requested, assessed, approved, tested, and implemented by authorized personnel.

### Controls

* Change request process
* Risk assessment
* Change approval
* Testing
* Segregation of duties
* Deployment authorization
* Backout procedures
* Post-implementation review

### Evidence

* Change tickets
* Approval records
* Test results
* Deployment records
* Release documentation
* Backout plans

### Testing

1. Select a sample of production changes.
2. Verify the change request.
3. Verify risk assessment.
4. Verify approval before implementation.
5. Review testing evidence.
6. Verify authorized implementation.
7. Check segregation of duties.
8. Review closure evidence.

---

# 7. Emergency Changes

## Risk 6 — Uncontrolled Emergency Changes

### Risk

Emergency changes may bypass normal controls and introduce unauthorized or insufficiently tested changes.

### Control Objective

Ensure emergency changes are properly authorized, documented, reviewed, and retrospectively assessed.

### Controls

* Emergency change procedure
* Emergency approval
* Documented justification
* Post-implementation review
* Retrospective testing where applicable

### Evidence

* Emergency change tickets
* Approval records
* Incident records
* Post-implementation reviews

### Testing

1. Identify emergency changes.
2. Verify documented justification.
3. Verify appropriate authorization.
4. Confirm implementation details were recorded.
5. Review post-implementation assessment.
6. Identify recurring emergency changes.

---

# 8. IT Operations

## Risk 7 — Inadequate Incident Management

### Risk

IT incidents may not be identified, escalated, investigated, or resolved within established timelines.

### Control Objective

Ensure incidents are properly recorded, prioritized, assigned, investigated, escalated, and resolved.

### Controls

* Incident management procedure
* Incident classification
* SLA monitoring
* Escalation procedures
* Incident tracking
* Closure review

### Evidence

* Incident tickets
* SLA reports
* Escalation records
* Incident reports
* Root cause analyses

### Testing

1. Select a sample of incidents.
2. Verify correct classification.
3. Review response and resolution times.
4. Check SLA compliance.
5. Verify escalation.
6. Review investigation evidence.
7. Confirm appropriate closure.

---

# 9. IT Operations — Job Monitoring

## Risk 8 — Failed Critical IT Jobs

### Risk

Failure of critical scheduled jobs may result in incomplete processing, inaccurate data, or service disruption.

### Control Objective

Ensure critical automated jobs are monitored and failures are identified and resolved promptly.

### Controls

* Job scheduling
* Automated job monitoring
* Failure alerts
* Exception handling
* Reconciliation procedures

### Evidence

* Job schedules
* Job execution logs
* Failure reports
* Monitoring alerts
* Exception reports

### Testing

1. Identify critical automated jobs.
2. Review scheduled jobs.
3. Inspect execution reports.
4. Identify failed jobs.
5. Verify that failures were investigated.
6. Confirm appropriate remediation.

---

# 10. System Monitoring

## Risk 9 — Delayed Detection of System Failures

### Risk

Critical system failures may not be detected promptly due to inadequate monitoring.

### Control Objective

Ensure critical infrastructure and services are monitored for availability, performance, and security events.

### Controls

* Infrastructure monitoring
* Availability monitoring
* Performance monitoring
* Alerting
* Escalation procedures

### Evidence

* Monitoring dashboards
* Alert reports
* Incident tickets
* Availability reports
* Performance reports

### Testing

1. Identify critical infrastructure.
2. Verify monitoring coverage.
3. Review selected alerts.
4. Confirm alert escalation.
5. Trace alerts to incidents where appropriate.
6. Document monitoring gaps.

---

# 11. Backup and Recovery

## Risk 10 — Failed or Incomplete Backups

### Risk

Critical data may not be recoverable because scheduled backups failed or were not completed.

### Control Objective

Ensure critical systems and information are backed up according to defined requirements and backup failures are promptly addressed.

### Controls

* Scheduled backups
* Backup monitoring
* Backup failure alerts
* Backup retention
* Backup review

### Evidence

* Backup schedules
* Backup logs
* Backup status reports
* Failure reports
* Exception records

### Testing

1. Identify critical systems.
2. Review configured backup schedules.
3. Inspect backup success rates.
4. Identify failed backups.
5. Verify investigation and remediation.
6. Confirm retention requirements.

---

# 12. Backup Restoration Testing

## Risk 11 — Backups Cannot Be Reliably Restored

### Risk

Backups may appear successful but fail when restoration is required.

### Control Objective

Ensure backup data is periodically tested to confirm recoverability.

### Controls

* Restoration testing
* Disaster recovery testing
* Recovery procedures
* Test documentation
* Remediation of failed restoration tests

### Evidence

* Restore test reports
* DR test reports
* Recovery logs
* Test results
* Remediation plans

### Testing

1. Obtain restoration test records.
2. Verify test frequency.
3. Review systems included in testing.
4. Assess test results.
5. Identify failed restoration attempts.
6. Confirm remediation.

---

# 13. Security Management — Vulnerability Management

## Risk 12 — Unpatched Vulnerabilities

### Risk

Known vulnerabilities may remain unremediated and be exploited by attackers.

### Control Objective

Ensure vulnerabilities are identified, prioritized, tracked, and remediated within established timelines.

### Controls

* Vulnerability scanning
* Risk-based prioritization
* Patch management
* Remediation SLAs
* Exception management

### Evidence

* Nessus reports
* Vulnerability dashboards
* Patch reports
* Remediation tickets
* Approved exceptions

### Testing

1. Obtain the latest vulnerability report.
2. Identify critical and high-risk vulnerabilities.
3. Compare findings with remediation records.
4. Assess SLA compliance.
5. Identify overdue vulnerabilities.
6. Review exceptions.
7. Evaluate compensating controls.

### Example Finding

> Critical vulnerabilities were identified on selected systems beyond the defined remediation timeline.

### Recommended Action

> Strengthen vulnerability remediation tracking and escalation to ensure critical vulnerabilities are addressed within approved timelines or covered by formally documented exceptions and compensating controls.

---

# 14. Security Management — Malware Protection

## Risk 13 — Inadequate Endpoint Protection

### Risk

Endpoints or servers without active and current security protection may be susceptible to malware infection.

### Control Objective

Ensure supported systems have active and up-to-date endpoint protection.

### Controls

* EDR/antivirus
* Centralized endpoint monitoring
* Definition updates
* Malware alerting
* Automated isolation where applicable

### Evidence

* EDR reports
* Antivirus dashboards
* Endpoint compliance reports
* Malware alerts
* Definition update reports

### Testing

1. Obtain endpoint security coverage.
2. Identify systems without active protection.
3. Identify outdated security definitions.
4. Review malware alerts.
5. Verify remediation actions.
6. Document exceptions.

---

# 15. Security Monitoring

## Risk 14 — Security Events Not Detected

### Risk

Security events may not be detected or investigated because critical logs are not collected or monitored.

### Control Objective

Ensure security events from critical systems are appropriately logged, monitored, and investigated.

### Controls

* SIEM
* Log collection
* Security monitoring
* Alerting
* Log retention
* Incident escalation

### Evidence

* SIEM reports
* System logs
* Security alerts
* Monitoring dashboards
* Investigation tickets

### Testing

1. Identify critical systems.
2. Verify logging is enabled.
3. Verify integration with centralized monitoring.
4. Select security alerts.
5. Confirm alerts were investigated.
6. Review escalation.
7. Document monitoring gaps.

---

# 16. Security Incident Management

## Risk 15 — Delayed Cybersecurity Incident Response

### Risk

Cybersecurity incidents may not be contained or resolved promptly, increasing operational, financial, and regulatory impact.

### Control Objective

Ensure security incidents are promptly identified, investigated, escalated, contained, and resolved.

### Controls

* Incident response plan
* Incident classification
* Escalation matrix
* Investigation procedures
* Containment procedures
* Lessons learned

### Evidence

* Incident response plans
* Incident tickets
* Investigation reports
* Escalation records
* Root cause analysis

### Testing

1. Select security incidents.
2. Verify classification.
3. Review detection and response times.
4. Verify investigation.
5. Review escalation.
6. Confirm containment.
7. Review post-incident actions.

---

# 17. Security Configuration Management

## Risk 16 — Insecure System Configuration

### Risk

Systems may contain insecure configurations that increase their exposure to cyber threats.

### Control Objective

Ensure systems are configured according to approved security baselines.

### Controls

* Secure configuration standards
* Hardening
* Configuration baselines
* Periodic compliance reviews
* Configuration monitoring

### Evidence

* Hardening standards
* Configuration reports
* Compliance scans
* System configuration records

### Testing

1. Select a sample of systems.
2. Obtain approved security baselines.
3. Compare configurations against standards.
4. Identify deviations.
5. Verify corrective actions.

---

# 18. Segregation of Duties

## Risk 17 — Incompatible IT Responsibilities

### Risk

One individual may have excessive control over a process by being able to request, approve, and implement the same activity.

### Control Objective

Separate conflicting responsibilities to reduce the risk of fraud, error, or unauthorized activity.

### Controls

* Role separation
* Approval controls
* Privileged access restrictions
* Change-management segregation
* Periodic SoD reviews

### Evidence

* Role matrices
* User listings
* Approval records
* SoD conflict reports

### Testing

1. Identify critical IT roles.
2. Obtain role assignments.
3. Identify incompatible combinations.
4. Verify compensating controls.
5. Review access-remediation records.

---

# 19. Generic and Service Accounts

## Risk 18 — Uncontrolled Generic Accounts

### Risk

Generic or service accounts may be used without clear ownership, accountability, monitoring, or lifecycle management.

### Control Objective

Ensure generic and service accounts are formally approved, owned, secured, monitored, and periodically reviewed.

### Controls

* Documented ownership
* Business justification
* Password management
* PAM
* Restrictions on interactive access
* Periodic review
* Activity logging

### Evidence

* Service account register
* Account approvals
* PAM records
* Password-management records
* Audit logs

### Testing

1. Obtain the generic/service-account listing.
2. Verify business justification.
3. Confirm account ownership.
4. Review access privileges.
5. Verify password controls.
6. Check activity logging.
7. Review periodic recertification.

---

# 20. ITGC Control Assessment Matrix

| #  | ITGC Area         | Risk                              | Key Control              | Evidence              | Typical Assessment  |
| -- | ----------------- | --------------------------------- | ------------------------ | --------------------- | ------------------- |
| 1  | Access            | Unauthorized access               | Access approval          | Access records        | Effective           |
| 2  | Access            | Excessive access                  | Periodic access review   | Review reports        | Partially Effective |
| 3  | Privileged Access | Excessive admin access            | PAM                      | PAM reports           | Partially Effective |
| 4  | Privileged Access | Shared accounts                   | Named accounts           | Account listings      | Partially Effective |
| 5  | Change            | Unauthorized changes              | Change approval          | Change tickets        | Effective           |
| 6  | Change            | Emergency changes bypass controls | Emergency change process | Emergency tickets     | Partially Effective |
| 7  | Operations        | Delayed incident resolution       | Incident management      | Incident records      | Effective           |
| 8  | Operations        | Failed jobs                       | Job monitoring           | Job reports           | Effective           |
| 9  | Operations        | System outages                    | Monitoring               | Monitoring reports    | Partially Effective |
| 10 | Backup            | Failed backups                    | Backup monitoring        | Backup reports        | Partially Effective |
| 11 | Recovery          | Unreliable restoration            | Restore testing          | Test reports          | Effective           |
| 12 | Security          | Unpatched systems                 | Vulnerability management | Nessus reports        | Partially Effective |
| 13 | Security          | Malware                           | EDR/antivirus            | EDR reports           | Effective           |
| 14 | Security          | Missed events                     | SIEM monitoring          | SIEM reports          | Partially Effective |
| 15 | Security          | Delayed incident response         | Incident response        | Incident reports      | Effective           |
| 16 | Security          | Insecure configuration            | Hardening baseline       | Configuration reports | Partially Effective |
| 17 | SoD               | Incompatible access               | SoD controls             | Conflict reports      | Effective           |
| 18 | Accounts          | Uncontrolled generic accounts     | Account management       | Account register      | Partially Effective |

---

# 21. ITGC Control Testing Template

For each control assessed, document:

| Assessment Field  | Description                                   |
| ----------------- | --------------------------------------------- |
| Process           | ITGC process being assessed                   |
| Risk              | What could go wrong?                          |
| Control Objective | What is the control intended to achieve?      |
| Control           | What has management implemented?              |
| Control Owner     | Who operates the control?                     |
| Frequency         | How often does the control operate?           |
| Evidence          | What proves the control operated?             |
| Population        | What universe is being tested?                |
| Sample            | What items were selected?                     |
| Testing Procedure | How was the control tested?                   |
| Exception         | What deviation was identified?                |
| Effectiveness     | Effective / Partially Effective / Ineffective |
| Residual Risk     | Risk remaining after controls                 |
| Action            | Remediation required                          |
| Owner             | Person responsible for remediation            |
| Target Date       | Expected closure date                         |

---

# 22. Control Testing Example

## Process

Access Management

## Risk

Shared privileged accounts may reduce accountability for administrative changes.

## Control Objective

Ensure privileged activities can be uniquely attributed to authorized users.

## Control

Privileged activities are performed through uniquely assigned administrator accounts.

## Evidence

* Active Directory account listing
* PAM reports
* Audit logs
* Privileged access review

## Testing

A sample of privileged accounts was reviewed to determine whether accounts were uniquely assigned and whether administrative activity could be attributed to individual users.

## Result

Shared administrative accounts were identified on critical systems.

## Effectiveness

**Partially Effective**

## Recommendation

Eliminate shared administrative accounts where technically feasible. Where unavoidable, implement compensating controls that preserve individual accountability and traceability.

## Treatment

**Mitigate**

---

# 23. ITGC Assessment Lifecycle

```text
Risk Identification
        ↓
Control Identification
        ↓
Control Design Assessment
        ↓
Evidence Collection
        ↓
Operating Effectiveness Testing
        ↓
Exception Identification
        ↓
Control Rating
        ↓
Residual Risk Assessment
        ↓
Remediation
        ↓
Follow-up Testing
        ↓
Closure
```

---

# 24. Key Takeaway

ITGC testing should establish more than whether a control exists.

A complete assessment should determine whether the control is:

**Designed appropriately → Implemented → Operating consistently → Supported by evidence → Producing the intended outcome**

The results should then feed into the organization's IT Risk Tracker, RCSA, audit findings, and remediation processes.
