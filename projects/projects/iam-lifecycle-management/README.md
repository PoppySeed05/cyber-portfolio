# IAM Lifecycle Management Project

## Overview
This project models an enterprise Identity and Access Management (IAM) lifecycle, including onboarding, access changes, and offboarding. It demonstrates how organizations enforce least privilege, manage identity risk, and maintain auditability across systems.

---

## 1. Business Context

In modern organizations, improper identity management is one of the leading causes of security breaches. This model simulates how a mid-size enterprise would manage user identities across multiple systems.

---

## 2. IAM Lifecycle Stages

### 1. Onboarding (Provisioning)
- HR triggers account creation
- Manager requests system access
- IAM team assigns role-based permissions
- MFA is enforced
- Access is logged for auditing

### 2. Access Changes (Role Modification)
- User role changes require approval
- Permissions are reviewed for least privilege
- Unused or excessive permissions are removed
- Changes are logged for compliance tracking

### 3. Offboarding (Deprovisioning)
- Account is disabled immediately upon termination
- Active sessions are revoked
- Group memberships removed
- Access logs are retained for audit purposes

---

## 3. Role-Based Access Control (RBAC)

| Role | Access Level | Systems |
|------|-------------|---------|
| IT Admin | Full Access | Servers, AD, cloud systems |
| SOC Analyst | Read/Investigate | SIEM, logs, alerts |
| Employee | Limited Access | Business apps |
| Contractor | Time-bound | Specific applications only |

---

## 4. Security Principles Applied

- Least Privilege Access
- Separation of Duties
- Identity Lifecycle Management
- Audit Logging & Traceability

---

## 5. Risk Analysis

### Risk 1: Excessive Privileges
- Users may retain unnecessary access after role changes
- Impact: High
- Mitigation: Periodic access reviews

### Risk 2: Orphaned Accounts
- Accounts not disabled after termination
- Impact: Critical
- Mitigation: Automated deprovisioning workflows

### Risk 3: Weak Approval Process
- Single approver could grant excessive access
- Impact: Medium
- Mitigation: Multi-step approval (manager + security)

---

## 6. Compliance Mapping

This model aligns with:

- Identity & Access Control (NIST CSF)
- Access Control Management (ISO 27001 concepts)
- Audit & Accountability principles

---

## 7. Future Enhancements

- Integration with Active Directory (Homelab)
- Automated access request workflow
- Logging simulation in SIEM
- Policy enforcement automation

---

## 8. Summary

This project demonstrates how identity lifecycle management reduces risk, enforces governance, and ensures secure operational access across enterprise systems.
