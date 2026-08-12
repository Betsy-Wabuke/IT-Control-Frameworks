# ISO/IEC 27001

## 1. Overview

ISO/IEC 27001 is an international standard for establishing, implementing, maintaining, and continually improving an Information Security Management System (ISMS).

It provides a systematic approach for managing information-security risks and protecting the confidentiality, integrity, and availability of information.

## 2. The CIA Triad

Information security controls should protect three core properties:

### Confidentiality

Ensuring information is accessible only to authorized individuals.

**Example controls:**

* Access controls
* Encryption
* Data classification
* User authentication

### Integrity

Ensuring information remains accurate, complete, and protected from unauthorized modification.

**Example controls:**

* Change management
* Audit logs
* Data validation
* Segregation of duties

### Availability

Ensuring information and systems are available when required.

**Example controls:**

* Backups
* Disaster recovery
* High availability
* Business continuity

```text
                 INFORMATION SECURITY
                         |
              ┌──────────┼──────────┐
              ↓          ↓          ↓
       Confidentiality  Integrity  Availability
              |          |          |
          Access       Change      Backup
          Control      Control     Recovery
```

## 3. Information Security Management System (ISMS)

An ISMS is the management framework used by an organization to manage information-security risks.

It involves:

1. Understanding the organization's context.
2. Identifying information-security risks.
3. Assessing and treating those risks.
4. Establishing security controls.
5. Monitoring control performance.
6. Conducting internal audits.
7. Reviewing the ISMS.
8. Continually improving the system.

## 4. Risk-Based Approach

ISO/IEC 27001 uses a risk-based approach.

The general process can be represented as:

```text
Identify Assets
      ↓
Identify Threats
      ↓
Identify Vulnerabilities
      ↓
Identify Risks
      ↓
Assess Risk
      ↓
Treat Risk
      ↓
Implement Controls
      ↓
Monitor Controls
      ↓
Improve
```

## 5. Risk Treatment

Once an information-security risk has been identified, an organization can determine an appropriate treatment approach.

Common approaches include:

* Mitigate
* Accept
* Avoid
* Transfer

### Example

**Risk:** Shared administrative accounts are used on critical systems.

**Treatment:** Mitigate

**Control:** Implement uniquely assigned privileged accounts and PAM.

**Expected outcome:** Activities can be attributed to individual administrators.

## 6. ISO/IEC 27001 Annex A Controls

ISO/IEC 27001 includes a set of information-security controls in Annex A.

These controls cover areas such as:

* Organizational controls
* People controls
* Physical controls
* Technological controls

The controls address topics including:

* Information-security policies
* Asset management
* Access control
* Identity management
* Authentication
* Vulnerability management
* Logging and monitoring
* Backup
* Cryptography
* Incident management
* Supplier security
* Business continuity
* Secure development

## 7. ISO 27001 and IT Risk

ISO/IEC 27001 can be incorporated into an IT Risk assessment by linking risks to security controls.

Example:

```text
IT Risk
   ↓
Risk Assessment
   ↓
Risk Treatment
   ↓
Security Control
   ↓
Control Owner
   ↓
Evidence
   ↓
Control Testing
   ↓
Effectiveness
   ↓
Improvement
```

## 8. Example Risk-to-Control Mapping

| Risk                  | Security Control           | Evidence                 | Testing                          |
| --------------------- | -------------------------- | ------------------------ | -------------------------------- |
| Unauthorized access   | Access control             | Access listing           | Review user access               |
| Shared admin accounts | Identity/access management | PAM report               | Identify shared accounts         |
| Data loss             | Backup                     | Backup reports           | Verify backup success            |
| Malware infection     | Malware protection         | EDR reports              | Review endpoint coverage         |
| Unpatched systems     | Vulnerability management   | Vulnerability report     | Review overdue vulnerabilities   |
| Security incidents    | Incident management        | Incident tickets         | Review incident handling         |
| Unauthorized changes  | Change management          | Change tickets           | Verify approval and testing      |
| Data exposure         | Encryption                 | Encryption configuration | Verify encryption implementation |

## 9. ISO 27001 in RCSA

ISO/IEC 27001 can support RCSA activities by helping identify:

* Information-security risks
* Security control objectives
* Control owners
* Control evidence
* Control testing procedures
* Control weaknesses
* Remediation activities

A practical structure is:

**Risk → Control → Evidence → Test → Effectiveness → Finding → Action**

## 10. Example: Shared Administrative Accounts

### Risk

Shared administrative accounts may be used to make changes to critical systems without sufficient individual accountability.

### Control Objective

Ensure privileged access is uniquely attributable to authorized individuals.

### Controls

* Named administrator accounts
* PAM
* MFA
* Privileged access approval
* Logging
* Session monitoring
* Periodic access reviews

### Evidence

* PAM reports
* User listings
* Access approval records
* Audit logs
* Access review reports

### Testing

1. Obtain privileged account listings.
2. Identify shared accounts.
3. Verify account ownership.
4. Review privileged access approvals.
5. Review authentication controls.
6. Check logging and monitoring.
7. Document exceptions.
8. Assess effectiveness.

### Possible Assessment

**Partially Effective**

The organization has privileged-access controls in place, but shared administrative accounts remain in use, reducing accountability and traceability.

### Recommended Action

Ensure privileged activities are performed using uniquely assigned named accounts. Where shared accounts cannot technically be eliminated, implement appropriate compensating controls.

## 11. ISO 27001 vs COBIT

| Area                 | COBIT                        | ISO/IEC 27001        |
| -------------------- | ---------------------------- | -------------------- |
| Primary Focus        | IT Governance and Management | Information Security |
| Risk Management      | Yes                          | Yes                  |
| IT Governance        | Strong                       | Supporting           |
| Information Security | Yes                          | Strong               |
| IT Operations        | Strong                       | Supporting           |
| Control Assessment   | Yes                          | Yes                  |
| ISMS                 | No                           | Yes                  |
| RCSA                 | Highly applicable            | Highly applicable    |
| IT Audit             | Highly applicable            | Highly applicable    |

### Key Difference

Think of it this way:

> **COBIT helps govern and manage enterprise IT.**

> **ISO/IEC 27001 helps establish and manage an information-security management system.**

They can therefore be used together rather than treated as competing frameworks.

## 12. Repository Objective

This section will later be expanded to map ISO/IEC 27001 controls against:

* COBIT
* NIST CSF
* CIS Controls
* ITGC
* COSO
* PCI DSS

The ultimate objective is to build a practical cross-framework control mapping that can support IT Risk, RCSA, IT Audit, and cybersecurity assessments.
