# IT Control Frameworks

## Overview

This repository provides a practical reference for understanding, implementing, assessing, and testing IT controls using established IT governance, cybersecurity, and internal control frameworks.

The repository focuses on the relationship between:

**IT Risks → Control Objectives → Controls → Frameworks → Evidence → Control Testing → Effectiveness → Remediation**

## Objectives

The objectives of this repository are to:

* Understand major IT control frameworks.
* Understand IT General Controls (ITGCs).
* Map IT risks to appropriate controls.
* Map controls to relevant frameworks.
* Identify appropriate control evidence.
* Perform control testing.
* Assess control effectiveness.
* Document control gaps and remediation actions.
* Support IT Risk, RCSA, IT Audit, and cybersecurity activities.

## Frameworks Covered

| Framework     | Primary Focus                   |
| ------------- | ------------------------------- |
| COBIT         | IT Governance and Management    |
| ISO/IEC 27001 | Information Security Management |
| NIST CSF      | Cybersecurity Risk Management   |
| CIS Controls  | Cybersecurity Safeguards        |
| ITGC          | IT General Controls             |
| COSO          | Internal Control                |
| PCI DSS       | Payment Card Security           |

## Repository Structure

### 01 - COBIT

IT governance, management objectives, control objectives, and practical control examples.

### 02 - ISO 27001

Information security controls and Information Security Management Systems (ISMS).

### 03 - NIST CSF

Cybersecurity risk management using the Identify, Protect, Detect, Respond, and Recover functions.

### 04 - CIS Controls

Prioritized technical and operational cybersecurity safeguards.

### 05 - ITGC

Core IT General Controls covering:

* Access Management
* Change Management
* IT Operations
* Backup and Recovery
* Security Management

### 06 - COSO

Internal control principles and their relationship to IT controls.

### 07 - PCI DSS

Controls for protecting payment account and cardholder data.

### 08 - Control Mapping

Practical mapping of:

**Risk → Control → Framework → Evidence → Testing → Effectiveness → Remediation**

## Practical Control Assessment Model

Each control can be assessed using the following approach:

1. Identify the risk.
2. Define the control objective.
3. Identify the control.
4. Identify the control owner.
5. Determine the control frequency.
6. Identify required evidence.
7. Define the testing procedure.
8. Test the control.
9. Assess control effectiveness.
10. Document exceptions or findings.
11. Define remediation actions.
12. Track remediation to closure.

## Example

**Risk:** Unauthorized privileged access

**Control:** Privileged access is restricted to authorized named users and reviewed periodically.

**Evidence:**

* Privileged access listings
* PAM reports
* Access review records
* System audit logs

**Testing:**

* Obtain the privileged account listing.
* Verify that each account is assigned to a named user.
* Review access approval evidence.
* Check whether periodic access reviews were performed.
* Review logs for unauthorized or unexplained activities.

**Potential Frameworks:**

* COBIT
* ISO/IEC 27001
* NIST CSF
* ITGC

## Intended Use

This repository is intended as a learning and professional reference for:

* IT Risk Management
* IT Audit
* RCSA
* Cybersecurity Governance
* IT General Controls
* Internal Controls
* Control Testing
* Risk and Control Assessments

> **Note:** This repository is a practical learning and reference resource and does not replace the official publications or requirements of the respective framework owners.

