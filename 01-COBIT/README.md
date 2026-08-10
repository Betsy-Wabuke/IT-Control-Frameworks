# COBIT

## 1. Overview

COBIT (Control Objectives for Information and Related Technologies) is an IT governance and management framework developed by ISACA.

It provides a structured approach for organizations to ensure that information and technology support business objectives while managing IT-related risks.

COBIT can be used to support:

* IT Governance
* IT Risk Management
* Internal Controls
* IT Audit
* Compliance
* Cybersecurity Governance
* RCSA
* Control Assessment

## 2. Why COBIT Matters in IT Risk

COBIT helps organizations establish a relationship between:

**Business Objectives → IT Objectives → Risks → Controls → Evidence → Assurance**

For example:

```text
Business Objective
       ↓
Protect Critical Business Information
       ↓
IT Risk
       ↓
Unauthorized access to critical systems
       ↓
Control
       ↓
Periodic user access reviews
       ↓
Evidence
       ↓
Access review reports
       ↓
Control Testing
       ↓
Effectiveness Assessment
```

## 3. COBIT Governance and Management

A key concept in COBIT is the distinction between **Governance** and **Management**.

### Governance

Governance ensures that stakeholder needs, conditions, and options are evaluated to determine:

* Business objectives
* Priorities
* Direction
* Monitoring requirements

In simple terms:

> **Governance determines what should be achieved and provides oversight.**

### Management

Management involves planning, building, running, and monitoring activities in accordance with the direction established through governance.

In simple terms:

> **Management determines how the objectives will be achieved.**

## 4. COBIT Core Model

COBIT organizes governance and management activities into five domains.

### Governance

**EDM — Evaluate, Direct and Monitor**

This domain focuses on governance activities such as:

* Evaluating stakeholder needs
* Establishing direction
* Monitoring performance
* Monitoring risk
* Monitoring compliance

### Management

**APO — Align, Plan and Organize**

Focuses on:

* Strategy
* Enterprise architecture
* Risk management
* Security
* Data
* Human resources
* Vendors

**BAI — Build, Acquire and Implement**

Focuses on:

* Change management
* Solutions development
* Implementation
* IT assets
* Configuration
* Knowledge management

**DSS — Deliver, Service and Support**

Focuses on:

* Operations
* Service requests
* Incidents
* Problems
* Continuity
* Security services

**MEA — Monitor, Evaluate and Assess**

Focuses on:

* Performance monitoring
* Internal control monitoring
* Compliance
* Assurance

### COBIT Structure

```text
                    COBIT
                      │
        ┌─────────────┴─────────────┐
        │                           │
   GOVERNANCE                  MANAGEMENT
        │                           │
       EDM                ┌─────────┼─────────┐
                          │         │         │
                         APO       BAI       DSS
                                    │
                                   MEA
```

## 5. COBIT and IT Risk

COBIT can be used to structure an IT Risk assessment.

For example:

### Risk

> Unauthorized users may gain access to critical applications.

### Risk Cause

* Poor user provisioning
* Delayed account deactivation
* Excessive privileges
* Lack of periodic access reviews

### Potential Impact

* Unauthorized transactions
* Data exposure
* Fraud
* Regulatory breaches
* Loss of accountability

### Control Objective

Ensure that access to IT systems is authorized, appropriate, and periodically reviewed.

### Example Controls

* User access approval
* Role-based access control
* Privileged access management
* Joiner-Mover-Leaver process
* Periodic access reviews
* Segregation of duties
* Account deactivation procedures

## 6. Example COBIT Control Assessment

| Risk                   | Control                       | Evidence             | Testing                                   | Effectiveness       |
| ---------------------- | ----------------------------- | -------------------- | ----------------------------------------- | ------------------- |
| Unauthorized access    | Quarterly user access review  | Access review report | Sample users and verify approval          | Effective           |
| Excessive privileges   | Role-based access             | User-role matrix     | Compare user roles against approved roles | Partially Effective |
| Shared admin accounts  | Named privileged accounts     | PAM report           | Identify shared accounts                  | Ineffective         |
| Unauthorized changes   | Change approval process       | Change tickets       | Sample changes and verify approvals       | Effective           |
| Poor incident response | Incident management procedure | Incident records     | Review sample incidents                   | Partially Effective |

## 7. COBIT in RCSA

COBIT can support the RCSA process by helping identify:

* IT processes
* Risks
* Control objectives
* Controls
* Control owners
* Evidence
* Control effectiveness
* Remediation actions

A practical RCSA structure can therefore be:

```text
Process
   ↓
Sub-Process
   ↓
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
Residual Risk
   ↓
Action Plan
```

## 8. Example

### Process

Access Control

### Sub-Process

Privileged Access Management

### Risk

Shared administrative accounts may be used to perform activities on critical systems without sufficient accountability.

### Control Objective

Ensure privileged activities can be uniquely attributed to authorized individuals.

### Controls

* Named administrator accounts
* PAM implementation
* MFA
* Privileged access approval
* Session monitoring
* Audit logging
* Periodic privileged access review

### Evidence

* PAM reports
* Active Directory reports
* Application user listings
* Audit logs
* Access approval records
* Access review reports

### Control Testing

1. Obtain the privileged account listing.
2. Identify shared administrative accounts.
3. Verify whether each privileged account is assigned to a named individual.
4. Review PAM configuration.
5. Check whether privileged sessions are logged.
6. Review evidence of periodic access reviews.
7. Document exceptions.
8. Assess control effectiveness.

### Possible Assessment

**Control Effectiveness: Partially Effective**

**Reason:**

PAM has been implemented; however, shared administrative accounts remain in use, reducing individual accountability and traceability.

### Recommended Action

> Ensure all privileged activities are performed using uniquely assigned named accounts and eliminate shared administrative accounts where technically feasible.

## 9. Key Takeaway

COBIT should not be viewed simply as a list of controls.

It provides a framework for connecting:

**Business Objectives → IT Governance → IT Processes → Risks → Controls → Performance → Assurance**

This makes COBIT particularly useful for IT Risk, RCSA, IT Audit, IT Governance, and control assessment activities.
