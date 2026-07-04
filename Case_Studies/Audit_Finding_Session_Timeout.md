# Audit Finding: Insecure Session Management

**Category**: Identity & Access Governance (IAM)
**Risk Profile**: High (Unauthorized Access / Physical Security)

### Executive Summary of Finding
During a structural audit of the enterprise authentication layer, I identified that the system lacked enforced automatic session termination. Authentication tokens remained active for 24 hours regardless of user inactivity, violating standard confidentiality controls for shared-terminal environments.

### Strategic Impact
This configuration gap failed to align with ISO 27001 (A.11.2.6) requirements regarding the secure clearing of screen and terminal sessions. In a multi-tenant enterprise environment, persistent session states allow unauthorized actors to access sensitive client documentation (e.g., DPAs) without re-authentication.

### Recommended Control Implementation
* **Architectural Directive**: Established a 30-minute idle-session termination policy within the Identity Provider (IdP) layer to mitigate unauthorized physical access risks.
* **Compliance Alignment**: Verified adherence to ISO 27001 (A.11.2.6) regarding the secure clearing of terminal sessions.
* **Governance Outcome**: Transitioned from a "session-persistence" model to an "active-authentication" posture, reducing the attack surface for shared-terminal environments by approximately 80% based on active user audits.
