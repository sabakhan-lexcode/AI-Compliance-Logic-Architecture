# GDPR Automated Audit Logic Map

This document outlines the binary audit criteria used to translate GDPR requirements into machine-readable validations for the AI scanning engine.

### Cluster 1: Governance & Risk (Accountability)

| Ref | Requirement | Audit Logic (Audit Criteria) |
| :--- | :--- | :--- |
| **Art 30** | Record of Processing (RoPA) | MUST mandate a RoPA. Must specify data categories, purposes, retention, and recipients. |
| **Art 33** | Breach Notif. (Authority) | MUST explicitly report breaches to the Supervisory Authority within 72 hours. Missing metric = FAIL. |
| **Art 35** | DPIA | MUST require a Data Protection Impact Assessment (DPIA) for "high risk" processing. |

### Cluster 6: Technological Controls

| Ref | Requirement | Audit Logic (Audit Criteria) |
| :--- | :--- | :--- |
| **Art 32(1)(a)** | Encryption | MUST explicitly mandate encryption of personal data (in transit and at rest). |
| **Art 32(1)(c)** | Backups | MUST mandate the ability to restore data availability in a timely manner (Disaster Recovery). |
| **Art 32(1)(d)** | Security Testing | MUST mandate regular effectiveness testing (e.g., Penetration Testing, Vulnerability Scanning). |

### Cluster 7: Privacy Layer (Subject Rights)

| Ref | Requirement | Audit Logic (Audit Criteria) |
| :--- | :--- | :--- |
| **Art 6** | Lawful Basis | MUST map all processing activities to a specific Lawful Basis (e.g., Consent, Contract). |
| **Art 12(3)** | DSAR Response SLA | MUST respond to Data Subject Access Requests within 1 month (30 days). Missing metric = FAIL. |
| **Art 44-46** | International Transfers | MUST prohibit transfers outside EEA unless safeguarded by Adequacy, BCRs, or SCCs. |
