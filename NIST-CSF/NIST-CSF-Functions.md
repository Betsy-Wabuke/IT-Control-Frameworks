# NIST CSF Functions

## 1. Overview

NIST CSF 2.0 organizes cybersecurity outcomes into six Functions:

1. Govern
2. Identify
3. Protect
4. Detect
5. Respond
6. Recover

The Functions provide a high-level structure for managing cybersecurity risk.

---

# 2. GOVERN

## Purpose

The Govern Function establishes and monitors the organization's cybersecurity risk-management strategy, expectations, and policies.

It provides the foundation for the other five Functions.

## Key Areas

* Cybersecurity strategy
* Risk management strategy
* Organizational policies
* Roles and responsibilities
* Oversight
* Supply-chain risk management
* Legal and regulatory requirements
* Cybersecurity performance measurement

## Example

**Risk:** Cybersecurity responsibilities are unclear.

**Control:**

* Define cybersecurity roles.
* Establish accountability.
* Document responsibilities.
* Establish governance committees.
* Monitor cybersecurity performance.

## Evidence

* Cybersecurity policies
* Governance structures
* Committee minutes
* Risk appetite statements
* Security responsibilities
* Management reports

---

# 3. IDENTIFY

## Purpose

The Identify Function helps the organization understand:

* Assets
* Data
* Business environment
* Cybersecurity risks
* Vulnerabilities
* Dependencies

## Key Areas

* Asset management
* Risk assessment
* Risk management strategy
* Improvement activities

## Example

**Risk:** Unknown devices may connect to the corporate network.

**Control:**

Maintain an accurate inventory of:

* Servers
* Workstations
* Network devices
* Applications
* Cloud resources
* Critical data

## Evidence

* Asset register
* CMDB
* GLPI records
* Network discovery reports
* Vulnerability scanning reports

---

# 4. PROTECT

## Purpose

The Protect Function focuses on implementing safeguards that reduce cybersecurity risks.

## Key Areas

* Identity management
* Authentication
* Access control
* Awareness and training
* Data security
* Platform security
* Technology infrastructure resilience

## Example

**Risk:** Unauthorized users may access critical applications.

**Controls:**

* MFA
* Least privilege
* Role-based access
* Access approval
* Privileged Access Management
* Periodic access reviews

## Evidence

* Access listings
* MFA reports
* PAM reports
* User access reviews
* Training records

---

# 5. DETECT

## Purpose

The Detect Function focuses on finding and analyzing possible cybersecurity attacks and compromises.

## Key Areas

* Continuous monitoring
* Adverse event analysis
* Detection processes
* Security event monitoring

## Example

**Risk:** A compromised endpoint may not be detected promptly.

**Controls:**

* EDR
* Antivirus
* SIEM
* Network monitoring
* Security alerts
* Threat detection

## Evidence

* SIEM reports
* EDR alerts
* Antivirus reports
* Security monitoring dashboards
* Incident tickets

---

# 6. RESPOND

## Purpose

The Respond Function focuses on actions taken after a cybersecurity incident has been detected.

## Key Areas

* Incident management
* Incident analysis
* Incident reporting
* Incident response
* Communication
* Mitigation

## Example

**Risk:** Security incidents may not be contained promptly.

**Controls:**

* Incident response plan
* Incident classification
* Escalation procedures
* Containment procedures
* Investigation procedures
* Communication plans

## Evidence

* Incident tickets
* Investigation reports
* Escalation records
* Incident response plans
* Root cause analysis

---

# 7. RECOVER

## Purpose

The Recover Function focuses on restoring affected assets and operations after a cybersecurity incident.

## Key Areas

* Recovery planning
* Recovery execution
* Communication
* Improvements

## Example

**Risk:** A ransomware incident may result in prolonged service disruption.

**Controls:**

* Tested backups
* Disaster recovery plan
* Business continuity plan
* Recovery procedures
* Restoration testing
* Lessons learned

## Evidence

* Backup reports
* DR test results
* Recovery plans
* Restoration records
* Post-incident review reports

---

# 8. Functions Working Together

The six Functions should not be treated as isolated activities.

Example:

```text
GOVERN
Establish cybersecurity strategy
        ↓
IDENTIFY
Identify critical assets and risks
        ↓
PROTECT
Implement security controls
        ↓
DETECT
Monitor for suspicious activity
        ↓
RESPOND
Contain and investigate incidents
        ↓
RECOVER
Restore systems and improve controls
        ↓
GOVERN
Review lessons learned and adjust strategy
```

This creates a continuous cybersecurity risk-management cycle.

---

# 9. Example: Ransomware Risk

### Govern

Establish ransomware risk-management requirements.

### Identify

Identify critical systems, data, dependencies, and vulnerabilities.

### Protect

Implement:

* EDR
* MFA
* Patch management
* Least privilege
* Security awareness
* Backups

### Detect

Monitor:

* Endpoint alerts
* SIEM events
* Network traffic
* Suspicious authentication

### Respond

* Isolate affected systems.
* Investigate the incident.
* Escalate appropriately.
* Contain the threat.
* Eradicate malware.

### Recover

* Restore systems.
* Validate backups.
* Resume operations.
* Conduct lessons learned.
* Improve controls.

---

# 10. Summary

| Function | Key Question                                    |
| -------- | ----------------------------------------------- |
| Govern   | How should cybersecurity risk be governed?      |
| Identify | What assets and cybersecurity risks do we have? |
| Protect  | What safeguards reduce those risks?             |
| Detect   | How will we know something has gone wrong?      |
| Respond  | What will we do when an incident occurs?        |
| Recover  | How will we restore operations and improve?     |

## Key Takeaway

NIST CSF should be viewed as a continuous cybersecurity lifecycle rather than a one-time checklist.
