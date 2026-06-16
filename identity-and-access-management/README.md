# Identity and Access Management (IAM) Lifecycle Model

## Purpose
This project demonstrates how enterprise identity lifecycle management works across onboarding, access changes, and offboarding.

## Lifecycle Stages

### 1. Onboarding
- HR triggers account creation
- Manager requests access
- IAM assigns role-based permissions
- MFA enforced

### 2. Access Changes
- Role changes require approval
- Least privilege enforced
- Previous access removed if not needed

### 3. Offboarding
- Account disabled immediately upon termination
- Sessions revoked
- Access removed from systems
- Logs retained for audit purposes

## Security Principles
- Least Privilege
- Separation of Duties
- Audit Logging
