# IT General Controls (ITGC)

## 1. Overview

IT General Controls (ITGCs) are foundational controls that support the security, reliability, availability, confidentiality, and integrity of an organization's IT environment.

ITGCs generally apply across the technology environment rather than to a single business application.

They are commonly assessed in:

* IT Risk Management
* RCSA
* IT Audit
* Internal Audit
* Financial Audit
* Cybersecurity Assessments
* Regulatory Reviews
* Compliance Assessments

---

## 2. Purpose of ITGCs

ITGCs help ensure that:

* Only authorized users access IT systems.
* Changes to systems are properly controlled.
* IT operations are performed reliably.
* Data and systems can be recovered after disruption.
* Security controls operate effectively.
* IT activities are appropriately monitored and recorded.

---

## 3. Core ITGC Categories

For this repository, ITGCs will be organized into five major categories:

```text
                         ITGC
                          |
        ┌─────────────────┼─────────────────┐
        ↓                 ↓                 ↓
 Access Management   Change Management   IT Operations
        |
        ├─────────────────┐
        ↓                 ↓
 Backup & Recovery   Security Management
```

### 1. Access Management

Controls governing access to systems and information.

Examples:

* User provisioning
* User deprovisioning
* Privileged access
* Access reviews
* Password controls
* MFA
* Segregation of duties
* Generic account management

### 2. Change Management

Controls governing changes to IT systems and infrastructure.

Examples:

* Change requests
* Change approvals
* Testing
* Segregation of duties
* Deployment controls
* Emergency changes
* Backout procedures

### 3. IT Operations

Controls supporting reliable and consistent IT operations.

Examples:

* Incident management
* Job scheduling
* System monitoring
* Batch processing
* Operational procedures
* Capacity monitoring

### 4. Backup and Recovery

Controls supporting recovery of systems and data.

Examples:

* Backup schedules
* Backup monitoring
* Backup retention
* Restoration testing
* Disaster recovery
* Business continuity

### 5. Security Management

Controls protecting IT systems and information from security threats.

Examples:

* Patch management
* Vulnerability management
* Malware protection
* Security monitoring
* Security incident management
* Security policies

---

# 4. ITGC Control Lifecycle

A practical ITGC assessment can follow:

```text
Risk
 ↓
Control Objective
 ↓
Control
 ↓
Control Owner
 ↓
Control Frequency
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
 ↓
Follow-up
```

---

# 5. Preventive, Detective and Corrective Controls

ITGCs can also be classified by their purpose.

## Preventive Controls

Designed to prevent an event from occurring.

Examples:

* MFA
* Access approval
* Change approval
* Least privilege
* Firewall restrictions

## Detective Controls

Designed to identify an event after or as it occurs.

Examples:

* Log monitoring
* Access reviews
* SIEM alerts
* Vulnerability scanning
* Exception reports

## Corrective Controls

Designed to restore or correct an issue.

Examples:

* Account removal
* Incident remediation
* System restoration
* Security patching
* Recovery procedures

---

# 6. Example — Access Management

## Risk

Unauthorized users may obtain access to critical systems.

## Control

All access to critical systems must be formally requested, approved, provisioned according to job responsibilities, periodically reviewed, and removed when no longer required.

## Evidence

* Access requests
* Approval records
* User listings
* Access reviews
* HR records
* Deprovisioning records

## Testing

1. Select a sample of users.
2. Verify access approval.
3. Compare assigned access to job responsibilities.
4. Verify periodic review.
5. Check terminated users.
6. Confirm timely removal.

---

# 7. Example — Shared Administrative Accounts

## Risk

Shared administrative accounts may be used to make changes on critical systems without sufficient individual accountability.

## Control Objective

Ensure privileged activities are uniquely attributable to authorized individuals.

## Controls

* Named administrator accounts
* PAM
* MFA
* Privileged access approval
* Session monitoring
* Audit logging
* Periodic privileged access reviews

## Evidence

* Privileged account listings
* PAM reports
* Audit logs
* Access approvals
* Access review reports

## Testing

1. Obtain privileged account listings.
2. Identify shared administrative accounts.
3. Verify ownership.
4. Review privileged access approvals.
5. Check activity logging.
6. Review PAM coverage.
7. Document exceptions.

## Assessment

**Partially Effective** may be appropriate where privileged access controls exist but shared accounts remain in use.

## Recommended Action

Ensure privileged activities are performed using uniquely assigned named accounts. Where a shared account is technically unavoidable, apply appropriate compensating controls and ensure activities remain individually attributable.

---

# 8. Example — Change Management

## Risk

Unauthorized or inadequately tested changes may cause system outages, vulnerabilities, or data integrity issues.

## Control

All production changes are formally requested, risk-assessed, tested, approved, implemented by authorized personnel, and documented.

## Evidence

* Change tickets
* Approvals
* Test results
* Deployment records
* Backout plans

## Testing

Sample production changes and verify:

* Request
* Risk assessment
* Approval
* Testing
* Implementation
* Segregation of duties
* Closure

---

# 9. Example — Backup

## Risk

Failure to maintain reliable backups may result in data loss and prolonged service disruption.

## Control

Critical systems are backed up according to defined schedules, monitored for failures, retained appropriately, and periodically tested for restoration.

## Evidence

* Backup reports
* Backup logs
* Restoration tests
* DR reports

## Testing

1. Identify critical systems.
2. Review backup configuration.
3. Inspect successful and failed backups.
4. Review backup retention.
5. Review restoration testing.
6. Document exceptions.

---

# 10. ITGC and Control Effectiveness

### Effective

The control is suitably designed and consistently operating as intended.

### Partially Effective

The control exists and operates but has exceptions, weaknesses, or inconsistent execution.

### Ineffective

The control is absent, inadequately designed, or not operating as intended.

---

# 11. ITGC and the IT Risk Tracker

ITGC results can feed directly into the organization's IT Risk Tracker.

Example:

| Risk                  | ITGC Area           | Control                | Effectiveness       | Treatment |
| --------------------- | ------------------- | ---------------------- | ------------------- | --------- |
| Shared admin accounts | Access Management   | Named accounts/PAM     | Partially Effective | Mitigate  |
| Excessive access      | Access Management   | Periodic access review | Partially Effective | Mitigate  |
| Unauthorized changes  | Change Management   | Change approval        | Effective           | Accept    |
| Failed backups        | Backup & Recovery   | Backup monitoring      | Partially Effective | Mitigate  |
| Unpatched systems     | Security Management | Patch management       | Partially Effective | Mitigate  |
| Delayed incidents     | IT Operations       | Incident management    | Effective           | Accept    |

---

# 12. ITGC and Framework Mapping

ITGCs can be mapped to the other frameworks in this repository.

| ITGC Area           | COBIT | ISO/IEC 27001 | NIST CSF       | CIS Controls |
| ------------------- | ----- | ------------- | -------------- | ------------ |
| Access Management   | Yes   | Yes           | Protect        | 5, 6         |
| Change Management   | Yes   | Yes           | Protect        | 4, 16        |
| IT Operations       | Yes   | Yes           | Detect/Respond | 8, 13, 17    |
| Backup & Recovery   | Yes   | Yes           | Recover        | 11           |
| Security Management | Yes   | Yes           | Protect/Detect | 7, 8, 10, 13 |

This mapping will be expanded in the repository's final **Control Mapping** section.

---

# 13. Practical ITGC Assessment Model

An ITGC reviewer should be able to answer:

### What is the risk?

What could go wrong?

### What is the control?

What has management implemented to address the risk?

### Who owns the control?

Who is responsible for operating it?

### How frequently does it operate?

Daily, weekly, monthly, quarterly, annually, or event-driven?

### What evidence exists?

What demonstrates that the control operated?

### How is it tested?

What procedure will establish whether the control operated effectively?

### What was the result?

Effective, partially effective, or ineffective?

### What happens next?

Accept, mitigate, transfer, or avoid the associated risk, as appropriate.

---

# 14. Key Takeaway

ITGCs provide a practical control structure for assessing the technology environment.

The core areas are:

**Access Management → Change Management → IT Operations → Backup & Recovery → Security Management**

The objective is not merely to confirm that policies exist. The assessment should determine whether controls are:

* Appropriately designed
* Implemented
* Operating consistently
* Supported by evidence
* Producing the intended outcome

That distinction is critical in IT Risk and control testing.
