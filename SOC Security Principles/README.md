# Security Principles Overview

This document summarizes key cybersecurity principles, models, and concepts relevant to building, maintaining, and assessing secure systems. It is designed for educational purposes and to demonstrate understanding of security frameworks, concepts, and best practices.
---
## Core Security Triad: CIA & DAD
### CIA Triad
The foundational model of information security:
- **Confidentiality** – Only authorized individuals can access data.
- **Integrity** – Data remains accurate and unaltered unless modified by authorized entities.
- **Availability** – Systems and data are accessible when needed.
### DAD Triad (Opposite of CIA)
Represents attacks on the CIA triad:
- **Disclosure** – Unauthorized access to sensitive information (opposite of confidentiality).
- **Alteration** – Unauthorized modification of data (opposite of integrity).
- **Destruction/Denial** – Preventing access to systems or data (opposite of availability).

---
## Security Concepts
- **Authenticity** – Ensuring data or communications are genuine and from the claimed source.
- **Non-repudiation** – The sender cannot deny sending a message or performing an action.
- **Vulnerability** – A weakness in a system that can be exploited.
- **Threat** – A potential source of harm to assets.
- **Risk** – Likelihood and impact of a threat exploiting a vulnerability.
- **Trust but Verify** – Principle of monitoring and validating actions even for trusted users.
- **Zero Trust** – Assumes no implicit trust; verify all access requests continuously.

---
## Security Models
### Bell-LaPadula Model
- Focus: **Confidentiality**
- Rules:
  - *Simple Security Property*: No read up.
  - *Star Property*: No write down.
  - Discretionary security property: Access matrix for controlled permissions.
### Biba Integrity Model
- Focus: **Integrity**
- Rules:
  - *Simple Integrity*: No read down.
  - *Star Integrity*: No write up.

### Clark-Wilson Model
- Focus: **Integrity**
- Concepts:
  - *Constrained Data Item (CDI)*: Data whose integrity must be preserved.
  - *Unconstrained Data Item (UDI)*: User or system input.
  - *Transformation Procedures (TPs)*: Maintain integrity during operations.
  - *Integrity Verification Procedures (IVPs)*: Validate correctness of CDIs.

## ISO/IEC 19249 Security Principles
### Architectural Principles
1. **Domain Separation** – Group components with common attributes into domains.
2. **Layering** – Apply security policies across multiple system layers.
3. **Encapsulation** – Hide internal details and enforce controlled access.
4. **Redundancy** – Ensure availability and integrity through duplication.
5. **Virtualization** – Isolate workloads using shared hardware environments.
### Design Principles
1. **Least Privilege** – Give users only the access they need.
2. **Attack Surface Minimization** – Reduce exposure to vulnerabilities.
3. **Centralized Parameter Validation** – Validate user input consistently.
4. **Centralized Security Services** – Consolidate authentication, logging, and other security functions.
5. **Error & Exception Handling** – Design systems to fail safely without leaking sensitive information.
## Defense Principles
- **Defense-in-Depth** – Multiple layers of security controls to slow or prevent attacks.
- **Shared Responsibility Model** – Security responsibilities are divided between provider and customer:
  - **Hardware, network, OS, applications** – Vary depending on IaaS, PaaS, or SaaS.
- **Trust but Verify / Zero Trust** – Continuous verification of access, even for internal users.
## Threat Management Concepts
- **Threat Intelligence** – Understanding emerging threats.
- **Incident Response** – Responding quickly and efficiently to breaches.
- **Vulnerability Management** – Detecting, prioritizing, and remediating system weaknesses.
- **Risk Assessment** – Evaluating threats in terms of likelihood and impact.

## Summary
Cybersecurity requires balancing multiple principles:
- Protect confidentiality, integrity, and availability while maintaining usability.
- Apply defense-in-depth and least privilege to limit risk.
- Incorporate trust verification and zero-trust approaches to reduce insider threats.
- Understand security models (Bell-LaPadula, Biba, Clark-Wilson) for structured access and data integrity.
- Leverage ISO/IEC 19249 architectural and design principles to guide secure system design.

This summary provides a high-level reference for best practices, models, and concepts in modern cybersecurity.

---
