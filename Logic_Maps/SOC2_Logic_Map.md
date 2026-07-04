# SOC 2 (TSC) Automated Audit Logic Map

This document outlines the binary audit criteria used to translate SOC 2 compliance requirements into machine-readable validations for the AI scanning engine.

### Cluster 1: Governance & Risk (Control Environment)

| Ref | Requirement | Audit Logic (Audit Criteria) |
| :--- | :--- | :--- |
| **CC1.1** | Integrity & Values | MUST show a formal Code of Conduct or Ethics Policy signed by management. If not explicitly documented, trigger FAIL. |
| **CC1.2** | Board Oversight | MUST contain evidence of an independent board or steering committee overseeing security/compliance. |
| **CC3.1** | Risk Assessment | MUST specify a formal risk assessment methodology (identifying threats, vulnerabilities, and impacts). Must be reviewed annually. |
| **CC3.2** | Fraud Risk | MUST explicitly mention the assessment of "Fraud" or "Insider Threat" in the risk register or policy. Missing the word 'fraud' = FAIL. |

### Cluster 5: Identity & Access Control

| Ref | Requirement | Audit Logic (Audit Criteria) |
| :--- | :--- | :--- |
| **CC6.1** | Logical Access | MUST define password complexity rules (e.g., 12+ chars, alphanumeric) OR mandate SSO/MFA. Must define 'Least Privilege'. |
| **CC6.2** | Access Provisioning | MUST require formal, documented approval from a manager or data owner before granting access to systems. |
| **CC6.3** | Access Revocation | MUST mandate immediate removal of access upon termination AND require periodic (e.g., annual) reviews of user access rights. |
