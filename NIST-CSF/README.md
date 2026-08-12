# NIST Cybersecurity Framework (CSF)

## 1. Overview

The NIST Cybersecurity Framework (CSF) provides a structured approach for organizations to manage cybersecurity risks.

It helps organizations understand, assess, prioritize, and communicate cybersecurity risks.

The framework can support:

* Cybersecurity Risk Management
* IT Risk Management
* Security Operations
* Control Assessments
* Incident Management
* Vulnerability Management
* RCSA
* Cybersecurity Governance

---

# 2. NIST CSF 2.0 Core Functions

NIST CSF 2.0 organizes cybersecurity activities into six functions:

1. **Govern**
2. **Identify**
3. **Protect**
4. **Detect**
5. **Respond**
6. **Recover**

The addition of **Govern** in CSF 2.0 makes the framework more useful for connecting cybersecurity activities to enterprise risk management and governance.

```text
                         NIST CSF 2.0
                              |
       ┌──────────────────────┼──────────────────────┐
       ↓                      ↓                      ↓
     GOVERN                IDENTIFY                PROTECT
       |                      |                      |
       └──────────────┬───────┴──────────────┬───────┘
                      ↓                      ↓
                    DETECT                RESPOND
                                             |
                                             ↓
                                          RECOVER
```

---

# 3. GOVERN

## Purpose

Establish and monitor the organization's cybersecurity risk-management strategy, expectations, and policies.

Governance provides the foundation for the other cybersecurity functions.

## Typical Activities

* Cybersecurity strategy
* Cybersecurity policies
* Risk management strategy
* Risk appetite
* Roles and responsibilities
* Legal and regulatory requirements
* Third-party risk management
* Cybersecurity oversight

## Example Risk

Cybersecurity responsibilities are not clearly defined.

## Example Controls

* Cybersecurity governance framework
* Defined security roles
* Security policies
* Risk management framework
* Management reporting
* Cybersecurity committees

## Evidence

* Cybersecurity policies
* Governance committee minutes
* Risk registers
* Organizational charts
* Management reports

---

# 4. IDENTIFY

## Purpose

Understand cybersecurity risks to the organization's assets, systems, data, people, and business environment.

## Typical Activities

* Asset management
* Risk assessment
* Vulnerability identification
* Business environment assessment
* Supply-chain risk assessment

## Example Risk

The organization cannot identify all devices connected to its network.

## Controls

* IT asset inventory
* Network discovery
* CMDB
* Endpoint management
* Asset ownership
* Periodic asset reconciliation

## Evidence

* Asset register
* Network discovery reports
* GLPI records
* Endpoint management reports
* CMDB

## Testing

1. Obtain the asset inventory.
2. Compare it against network discovery results.
3. Identify unknown devices.
4. Verify asset ownership.
5. Document discrepancies.

---

# 5. PROTECT

## Purpose

Implement safeguards that reduce the likelihood or impact of cybersecurity incidents.

## Typical Activities

* Identity management
* Access control
* Awareness training
* Data security
* Platform security
* Technology infrastructure resilience

## Example Risk

Unauthorized users may access critical systems.

## Controls

* MFA
* Least privilege
* RBAC
* PAM
* Access reviews
* Password controls
* Network segmentation

## Evidence

* Active Directory reports
* PAM reports
* MFA reports
* Access review records
* Network configurations

## Testing

1. Obtain user access listings.
2. Identify privileged users.
3. Verify MFA.
4. Review access approvals.
5. Review periodic access reviews.
6. Identify inappropriate access.

---

# 6. DETECT

## Purpose

Discover and analyze possible cybersecurity attacks and other potentially adverse events.

## Typical Activities

* Continuous monitoring
* Security event analysis
* Anomaly detection
* Threat detection
* Security alert management

## Example Risk

Security events may not be detected because critical systems are not adequately monitored.

## Controls

* SIEM
* EDR
* Network monitoring
* IDS/IPS
* Log management
* Security alerting
* Threat intelligence

## Evidence

* SIEM dashboards
* EDR reports
* Security alerts
* Network monitoring reports
* Incident tickets

## Testing

1. Identify critical systems.
2. Verify logging.
3. Verify integration with SIEM.
4. Select security alerts.
5. Trace alerts to investigation records.
6. Check whether incidents were appropriately escalated.

---

# 7. RESPOND

## Purpose

Take action regarding detected cybersecurity incidents.

## Typical Activities

* Incident management
* Incident analysis
* Incident reporting
* Incident containment
* Incident mitigation
* Stakeholder communication

## Example Risk

Cybersecurity incidents may not be contained promptly.

## Controls

* Incident response plan
* Incident classification
* Escalation procedures
* Containment procedures
* Communication plans
* Incident response exercises

## Evidence

* Incident tickets
* Incident response plans
* Investigation records
* Escalation records
* Incident reports

## Testing

1. Select security incidents.
2. Review detection time.
3. Review response time.
4. Verify containment actions.
5. Review escalation.
6. Verify closure and lessons learned.

---

# 8. RECOVER

## Purpose

Restore affected assets and operations after a cybersecurity incident.

## Typical Activities

* Recovery planning
* System restoration
* Recovery communication
* Recovery verification
* Improvement activities

## Example Risk

A ransomware attack may result in prolonged system downtime because recovery capabilities are inadequate.

## Controls

* Backups
* Disaster recovery plans
* System restoration procedures
* Recovery testing
* Business continuity plans
* Recovery objectives

## Evidence

* Backup reports
* DR plans
* DR test reports
* Recovery test results
* RTO/RPO documentation

## Testing

1. Identify critical systems.
2. Review backup arrangements.
3. Verify backup success.
4. Review restoration testing.
5. Compare recovery results against RTO/RPO.
6. Document recovery gaps.

---

# 9. NIST CSF and IT Risk

NIST CSF can be incorporated into an IT Risk assessment as follows:

```text
Risk
 ↓
Identify
 ↓
Protect
 ↓
Detect
 ↓
Respond
 ↓
Recover
 ↓
Continuous Improvement
```

However, the six functions should not be viewed as a simple linear process. They work together as part of an ongoing cybersecurity risk-management lifecycle.

---

# 10. Example Risk Mapping

### Risk

Critical vulnerabilities remain unpatched beyond the defined remediation period.

### Govern

Establish vulnerability-management policy and risk appetite.

### Identify

Identify vulnerable systems and assess vulnerability severity.

### Protect

Deploy patches and implement compensating controls.

### Detect

Monitor systems for exploitation attempts.

### Respond

Investigate and contain any resulting security incidents.

### Recover

Restore affected systems and validate security after remediation.

---

# 11. NIST CSF and RCSA

NIST CSF can support RCSA by organizing cybersecurity controls according to the type of security activity they support.

Example:

| Risk                      | NIST Function  | Control                   | Evidence              |
| ------------------------- | -------------- | ------------------------- | --------------------- |
| Unknown devices           | Identify       | Asset inventory           | Asset register        |
| Unauthorized access       | Protect        | MFA/RBAC                  | Access reports        |
| Malware                   | Protect/Detect | EDR                       | EDR reports           |
| Missed security events    | Detect         | SIEM                      | SIEM reports          |
| Delayed incident response | Respond        | Incident response process | Incident tickets      |
| Data loss                 | Recover        | Backup/DR                 | Backup and DR reports |

---

# 12. NIST CSF and IT Risk Tracker

A NIST CSF mapping field can be added to the IT Risk Tracker.

Example:

| Risk                      | Risk Rating | Control                | NIST Function    | Effectiveness       | Treatment |
| ------------------------- | ----------- | ---------------------- | ---------------- | ------------------- | --------- |
| Shared admin accounts     | Major       | Named accounts/PAM     | Protect          | Partially Effective | Mitigate  |
| Unpatched vulnerabilities | Major       | Patch management       | Identify/Protect | Partially Effective | Mitigate  |
| SIEM monitoring gaps      | Major       | Centralized monitoring | Detect           | Ineffective         | Mitigate  |
| Delayed incident response | Moderate    | Incident management    | Respond          | Partially Effective | Mitigate  |
| Inadequate backups        | Critical    | Backup/DR              | Recover          | Effective           | Accept    |

---

# 13. NIST CSF vs COBIT vs ISO/IEC 27001

| Area              | COBIT         | ISO/IEC 27001        | NIST CSF           |
| ----------------- | ------------- | -------------------- | ------------------ |
| Primary Focus     | IT Governance | Information Security | Cybersecurity Risk |
| Governance        | Strong        | Yes                  | Strong in CSF 2.0  |
| IT Risk           | Strong        | Strong               | Strong             |
| Cybersecurity     | Supporting    | Strong               | Strong             |
| ISMS              | No            | Yes                  | No                 |
| Control Testing   | Yes           | Yes                  | Yes                |
| Incident Response | Yes           | Yes                  | Strong             |
| Asset Management  | Yes           | Yes                  | Strong             |
| RCSA              | Strong        | Strong               | Strong             |

### Simple distinction

**COBIT:**

> How should enterprise IT be governed and managed?

**ISO/IEC 27001:**

> How should information-security risks be managed through an ISMS?

**NIST CSF:**

> How should cybersecurity risks be governed, identified, protected, detected, responded to, and recovered from?

---

# 14. Key Takeaway

NIST CSF is particularly useful for translating cybersecurity risks into practical security activities.

The six functions provide a useful structure:

```text
GOVERN
   ↓
IDENTIFY
   ↓
PROTECT
   ↓
DETECT
   ↓
RESPOND
   ↓
RECOVER
```

For IT Risk purposes, the framework becomes especially powerful when combined with COBIT and ISO/IEC 27001.

The eventual objective of this repository is to create a cross-framework mapping that allows one IT Risk or control to be mapped to multiple frameworks without duplicating the underlying control work.
