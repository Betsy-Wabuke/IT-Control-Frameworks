# COBIT Control Examples and Testing

## 1. Purpose

This document provides practical examples of IT risks, control objectives, controls, evidence, testing procedures, and control effectiveness assessments.

The objective is to demonstrate how COBIT concepts can be applied to real-world IT Risk and control activities.

---

## 2. Risk-to-Control Assessment Structure

A practical control assessment follows this sequence:

```text
Risk
 ↓
Risk Cause
 ↓
Risk Impact
 ↓
Control Objective
 ↓
Control
 ↓
Control Owner
 ↓
Evidence
 ↓
Control Testing
 ↓
Control Effectiveness
 ↓
Finding
 ↓
Remediation
```

---

# 3. Access Management

## Risk 1: Unauthorized User Access

### Risk

Unauthorized users may gain access to systems or applications, resulting in data exposure, fraud, or unauthorized transactions.

### Risk Causes

* Inadequate access approvals
* Poor user provisioning
* Delayed account deactivation
* Lack of periodic access reviews

### Control Objective

Ensure system access is granted only to authorized users based on approved business requirements.

### Controls

* Formal access request and approval
* Role-based access control
* Joiner-Mover-Leaver process
* Periodic access reviews
* Timely account deactivation

### Evidence

* Access request forms
* Approval records
* User listings
* Access review reports
* HR termination reports

### Testing Procedure

1. Select a sample of users.
2. Obtain their access approval records.
3. Verify that access was approved by an authorized person.
4. Compare assigned roles against job responsibilities.
5. Review terminated-user listings.
6. Verify that terminated users were deactivated promptly.
7. Document exceptions.

### Effectiveness Criteria

**Effective:** Access is consistently approved, appropriate, reviewed, and removed when no longer required.

**Partially Effective:** Controls exist but exceptions or delays are identified.

**Ineffective:** Access is granted without appropriate approval or users retain inappropriate access.

---

# 4. Privileged Access Management

## Risk 2: Shared Administrative Accounts

### Risk

Shared administrative accounts may be used to make changes on critical systems, resulting in lack of accountability and traceability.

### Control Objective

Ensure privileged activities can be uniquely attributed to authorized individuals.

### Controls

* Named administrator accounts
* Privileged Access Management (PAM)
* Multi-factor authentication
* Privileged access approval
* Session monitoring
* Audit logging
* Periodic privileged access reviews

### Evidence

* PAM reports
* Active Directory reports
* Application account listings
* Privileged activity logs
* Access approval records
* Access review reports

### Testing Procedure

1. Obtain the privileged account listing.
2. Identify shared administrative accounts.
3. Verify whether each account is assigned to a named individual.
4. Review PAM implementation.
5. Verify whether privileged sessions are logged.
6. Review privileged access approvals.
7. Review periodic access review evidence.
8. Document exceptions.

### Example Finding

> Shared administrative accounts were identified on critical systems. The use of these accounts limits the ability to attribute system changes to individual users.

### Recommended Action

> Eliminate shared administrative accounts and ensure privileged activities are performed through uniquely assigned named accounts. Where shared accounts are technically unavoidable, implement compensating controls such as PAM, session monitoring, MFA, and enhanced logging.

### Example Effectiveness

**Partially Effective**

PAM controls may be implemented; however, continued use of shared administrative accounts reduces accountability and traceability.

---

# 5. Change Management

## Risk 3: Unauthorized System Changes

### Risk

Unauthorized or inadequately tested changes may introduce system vulnerabilities, outages, or data integrity issues.

### Control Objective

Ensure changes to IT systems are properly authorized, tested, documented, and implemented.

### Controls

* Change request process
* Change approval
* Segregation of duties
* Testing before implementation
* Backout procedures
* Emergency change procedures
* Post-implementation review

### Evidence

* Change tickets
* Approval records
* Test results
* Deployment records
* Backout plans
* Post-implementation review reports

### Testing Procedure

1. Select a sample of system changes.
2. Verify that each change has a documented request.
3. Verify approval before implementation.
4. Confirm evidence of testing.
5. Check whether implementation was performed by an authorized individual.
6. Verify that emergency changes followed the appropriate process.
7. Review post-implementation evidence.

### Effectiveness

**Effective:** Changes are consistently authorized, tested, documented, and traceable.

**Partially Effective:** The process exists but exceptions are identified.

**Ineffective:** Changes are frequently implemented without approval, testing, or documentation.

---

# 6. Patch Management

## Risk 4: Unpatched Systems

### Risk

Systems with outdated security patches may be exploited by attackers, resulting in compromise, data loss, or service disruption.

### Control Objective

Ensure security patches are identified, prioritized, tested, and deployed within defined timelines.

### Controls

* Patch management policy
* Vulnerability scanning
* Patch prioritization
* Patch deployment
* Exception management
* Patch compliance monitoring

### Evidence

* Vulnerability reports
* Patch deployment reports
* Endpoint management reports
* Exception records
* Patch compliance dashboards

### Testing Procedure

1. Obtain the list of systems requiring patches.
2. Identify critical and high-risk vulnerabilities.
3. Compare identified vulnerabilities against patch deployment records.
4. Verify whether patches were deployed within the defined SLA.
5. Review overdue patches.
6. Check whether exceptions were formally approved.
7. Assess remediation status.

---

# 7. Backup and Recovery

## Risk 5: Data Loss Due to Inadequate Backups

### Risk

Failure to maintain reliable backups may result in permanent data loss and prolonged service disruption.

### Control Objective

Ensure critical data and systems are backed up and can be restored within defined recovery requirements.

### Controls

* Scheduled backups
* Backup monitoring
* Offsite or geographically separated backups
* Backup encryption
* Backup retention
* Restoration testing
* Disaster recovery testing

### Evidence

* Backup logs
* Backup reports
* Restoration test results
* Disaster recovery test reports
* Backup schedules

### Testing Procedure

1. Identify critical systems.
2. Verify that backups are configured.
3. Review backup success/failure reports.
4. Review backup retention.
5. Confirm that backups are appropriately protected.
6. Review evidence of restoration testing.
7. Document failed backups and unresolved exceptions.

---

# 8. Security Monitoring

## Risk 6: Security Events Not Detected

### Risk

Failure to monitor security events may result in delayed detection and response to cyber incidents.

### Control Objective

Ensure security events are monitored, investigated, and escalated appropriately.

### Controls

* SIEM monitoring
* Endpoint monitoring
* Security alerts
* Log collection
* Incident escalation
* Security event investigation
* Log retention

### Evidence

* SIEM reports
* Security alerts
* Incident tickets
* Investigation records
* Log monitoring dashboards
* Escalation records

### Testing Procedure

1. Obtain security monitoring reports.
2. Select a sample of security alerts.
3. Verify that alerts were investigated.
4. Check whether appropriate remediation was performed.
5. Verify escalation where required.
6. Compare endpoint security events against SIEM records.
7. Document monitoring gaps.

---

# 9. Incident Management

## Risk 7: Delayed Incident Response

### Risk

Failure to identify and respond to IT security incidents within defined timelines may increase operational, financial, and regulatory impact.

### Control Objective

Ensure incidents are identified, recorded, investigated, escalated, and resolved within defined service levels.

### Controls

* Incident management procedure
* Incident classification
* Incident escalation
* Incident SLA monitoring
* Root cause analysis
* Incident closure review

### Evidence

* Incident tickets
* Incident reports
* SLA reports
* Root cause analysis
* Escalation records
* Closure approvals

### Testing Procedure

1. Select a sample of incidents.
2. Verify incident classification.
3. Check response times.
4. Verify investigation evidence.
5. Review escalation records.
6. Check whether SLA requirements were met.
7. Review root cause analysis where applicable.

---

# 10. User Access Review

## Risk 8: Excessive User Access

### Risk

Users may retain access that is no longer required because of role changes, transfers, or changes in responsibilities.

### Control Objective

Ensure user access remains appropriate based on current job responsibilities.

### Controls

* Periodic access reviews
* Role-based access control
* Joiner-Mover-Leaver controls
* Segregation of duties
* Access recertification

### Evidence

* Access review reports
* User-role matrices
* HR records
* Access removal records
* Management sign-offs

### Testing Procedure

1. Obtain the user population.
2. Select a sample.
3. Compare user roles with current job responsibilities.
4. Identify inappropriate access.
5. Verify management review and approval.
6. Confirm that inappropriate access was removed.

---

# 11. Control Assessment Matrix

| Risk Area           | Example Risk           | Primary Control     | Evidence             | Typical Effectiveness |
| ------------------- | ---------------------- | ------------------- | -------------------- | --------------------- |
| Access Management   | Unauthorized access    | Access approval     | Access request       | Effective             |
| Privileged Access   | Shared admin accounts  | Named accounts/PAM  | PAM report           | Partially Effective   |
| Change Management   | Unauthorized changes   | Change approval     | Change tickets       | Effective             |
| Patch Management    | Unpatched systems      | Patch management    | Patch report         | Partially Effective   |
| Backup              | Data loss              | Scheduled backups   | Backup logs          | Effective             |
| Security Monitoring | Missed security events | SIEM monitoring     | SIEM reports         | Partially Effective   |
| Incident Management | Delayed response       | Incident management | Incident tickets     | Effective             |
| Access Review       | Excessive access       | Periodic review     | Access review report | Partially Effective   |

---

# 12. Control Effectiveness Rating

A simple three-level assessment can be used:

### Effective

The control is appropriately designed and operating consistently.

### Partially Effective

The control exists and operates but has weaknesses, exceptions, or inconsistencies.

### Ineffective

The control is absent, poorly designed, or not operating as intended.

---

# 13. From Control Testing to IT Risk Tracker

Control testing results can feed directly into an IT Risk Tracker.

Example:

| Risk                     | Control                   | Finding                           | Effectiveness       | Action   |
| ------------------------ | ------------------------- | --------------------------------- | ------------------- | -------- |
| Shared admin accounts    | Named privileged accounts | Shared accounts identified        | Partially Effective | Mitigate |
| Unauthorized changes     | Change approval           | Approval evidence available       | Effective           | Accept   |
| Unpatched systems        | Patch management          | Critical patches overdue          | Partially Effective | Mitigate |
| Excessive access         | Access review             | Inappropriate access identified   | Ineffective         | Mitigate |
| Security monitoring gaps | SIEM monitoring           | Some events not reflected in SIEM | Ineffective         | Mitigate |

---

# 14. Practical Control Testing Checklist

Before concluding a control assessment, verify:

* [ ] Risk identified
* [ ] Control objective defined
* [ ] Control identified
* [ ] Control owner identified
* [ ] Control frequency established
* [ ] Evidence obtained
* [ ] Sample selected
* [ ] Testing performed
* [ ] Exceptions documented
* [ ] Root cause identified
* [ ] Control effectiveness assessed
* [ ] Residual risk assessed
* [ ] Remediation action defined
* [ ] Action owner assigned
* [ ] Target date established
* [ ] Finding added to IT Risk Tracker where applicable

---

# 15. Key Takeaway

A framework becomes useful when it can be translated into practical control activities.

The objective is not simply to say:

> "This control aligns with COBIT."

The stronger approach is:

> **Risk → Control Objective → Control → Framework Mapping → Evidence → Testing → Finding → Effectiveness → Remediation**

This approach creates a clear connection between IT governance frameworks and day-to-day IT Risk management.
