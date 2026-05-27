# Authorization Standards

# Identity Philosophy

Preferred identity foundation:

- ASP.NET Core Identity
- JWT authentication
- refresh token workflows
- claims-based identity
- permission-based authorization

Identity systems SHOULD remain extensible and tenant-aware.

---

# Authentication Expectations

Authentication SHOULD support:

- JWT access tokens
- refresh tokens
- MFA/TOTP
- OAuth providers
- device/session management
- email verification
- password reset workflows

---

# Authorization Philosophy

Authorization MUST remain permission-based.

Role-only authorization is insufficient for enterprise SaaS systems.

Preferred authorization model:

```txt
Users
Roles
Permissions
RolePermissions
UserRoles
Claims
```

Permission examples:

```txt
users.read
users.write
billing.manage
tenant.settings
```

---

# Rules

Authorization MUST:

- remain centralized
- remain explicit
- support tenant-aware enforcement
- remain testable
- avoid duplication

Authorization logic SHOULD remain close to business capabilities.

---

# Policy Rules

Authorization policies SHOULD:

- remain composable
- remain predictable
- remain testable
- avoid hidden coupling

---

# Security Principle

Security boundaries MUST remain explicit and observable.