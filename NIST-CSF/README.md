# NIST Cybersecurity Framework (CSF)

## 1. Overview

The NIST Cybersecurity Framework (CSF) is a cybersecurity risk-management framework developed by the National Institute of Standards and Technology (NIST).

It provides organizations with a structured approach to managing cybersecurity risks and improving their ability to:

* Identify cybersecurity risks
* Protect systems and information
* Detect cybersecurity events
* Respond to incidents
* Recover from cybersecurity disruptions

The current NIST CSF 2.0 is organized around six core Functions:

**Govern → Identify → Protect → Detect → Respond → Recover**

---

## 2. Purpose

The NIST CSF can be used to:

* Establish cybersecurity governance
* Identify cybersecurity risks
* Assess existing security controls
* Identify control gaps
* Prioritize security improvements
* Support risk assessments
* Support RCSA activities
* Improve incident response
* Support cybersecurity audits
* Measure cybersecurity maturity

---

## 3. The Six NIST CSF Functions

| Function | Purpose                                                                       |
| -------- | ----------------------------------------------------------------------------- |
| Govern   | Establish and monitor cybersecurity risk management strategy and expectations |
| Identify | Understand cybersecurity risks, assets, and organizational context            |
| Protect  | Implement safeguards to manage cybersecurity risks                            |
| Detect   | Discover and analyze potential cybersecurity attacks and compromises          |
| Respond  | Take action regarding detected cybersecurity incidents                        |
| Recover  | Restore affected assets and operations                                        |

### High-Level Model

```text
                    NIST CSF 2.0
                         |
    ┌────────────────────┼────────────────────┐
    ↓                    ↓                    ↓
 GOVERN              IDENTIFY              PROTECT
    ↓                    ↓                    ↓
Cybersecurity       Understand           Safeguards
Governance          Cyber Risk           & Controls
    │
    └────────────────────┬────────────────────┘
                         ↓
                      DETECT
                         ↓
                  Security Events
                         ↓
                      RESPOND
                         ↓
                    Incidents
                         ↓
                      RECOVER
                         ↓
                  Restore & Improve
```

---

## 4. NIST CSF and IT Risk

NIST CSF provides a practical way of connecting cybersecurity risks with security controls.

```text
Cybersecurity Risk
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
Risk Reduction
```

---

## 5. NIST CSF and RCSA

NIST CSF can support an RCSA by helping organizations identify:

* Cybersecurity risks
* Security control objectives
* Existing controls
* Control gaps
* Control evidence
* Control effectiveness
* Remediation actions

Example:

**Risk:** Unauthorized access to critical systems

**Identify:** Identify critical systems and privileged users.

**Protect:** Implement MFA and least privilege.

**Detect:** Monitor authentication and privileged activity.

**Respond:** Investigate unauthorized access alerts.

**Recover:** Restore affected systems and review lessons learned.

---

## 6. NIST CSF and IT Risk Tracker

NIST CSF Functions can be added as a framework-mapping field in an IT Risk Tracker.

Example:

| Risk                      | Control                | NIST Function | Effectiveness       | Treatment |
| ------------------------- | ---------------------- | ------------- | ------------------- | --------- |
| Unauthorized access       | MFA                    | Protect       | Effective           | Accept    |
| Unknown IT assets         | Asset inventory        | Identify      | Partially Effective | Mitigate  |
| Missed security alerts    | SIEM monitoring        | Detect        | Partially Effective | Mitigate  |
| Delayed incident response | Incident response plan | Respond       | Effective           | Accept    |
| Data loss                 | Backup and recovery    | Recover       | Effective           | Accept    |

---

## 7. NIST CSF Implementation Approach

A practical implementation can follow these steps:

1. Establish cybersecurity governance.
2. Identify organizational assets and risks.
3. Determine current cybersecurity capabilities.
4. Define target cybersecurity outcomes.
5. Identify gaps.
6. Prioritize remediation.
7. Implement controls.
8. Monitor performance.
9. Review and improve continuously.

---

## 8. NIST CSF Profiles

NIST CSF can be used to develop organizational Profiles.

### Current Profile

Describes the organization's current cybersecurity posture.

### Target Profile

Describes the desired cybersecurity outcomes.

The gap between the two can be used to prioritize improvement activities.

```text
Current Profile
       ↓
Gap Analysis
       ↓
Risk Prioritization
       ↓
Target Profile
       ↓
Remediation
       ↓
Continuous Improvement
```

---

## 9. NIST CSF and Other Frameworks

NIST CSF can be used alongside other frameworks.

```text
                 IT GOVERNANCE
                      |
                    COBIT
                      |
        ┌─────────────┼─────────────┐
        ↓             ↓             ↓
   ISO 27001       NIST CSF      ITGC
        ↓             ↓             ↓
 Information      Cybersecurity   IT General
  Security           Risk         Controls
```

NIST CSF can therefore serve as the cybersecurity risk-management layer while COBIT provides broader IT governance and ISO/IEC 27001 provides an information-security management framework.

---

## 10. Key Takeaway

The NIST CSF provides a simple way to understand cybersecurity risk management:

> **Govern → Identify → Protect → Detect → Respond → Recover**

For IT Risk professionals, the framework is particularly useful for connecting cybersecurity risks to practical controls, control testing, remediation, and continuous improvement.
