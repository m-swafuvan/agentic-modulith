# Multitenancy Standards

# Purpose

Tenant isolation is a core architectural concern.

All systems SHOULD assume multitenancy unless explicitly documented otherwise.

---

# Supported Models

Supported tenancy models may include:

- shared database
- row-level security
- schema-per-tenant
- database-per-tenant
- hybrid tenancy

---

# Tenant Safety Rules

Tenant isolation MUST:

- remain explicit
- never rely solely on client input
- be enforced consistently
- remain testable

Cross-tenant leakage is forbidden.

---

# Tenant Context

Every request SHOULD resolve:

```txt
Request
 → Tenant Context
 → Authorization Context
 → Persistence Context
```

Tenant scope must remain explicit throughout the request lifecycle.

---

# Authorization Scope

Authorization MUST respect tenant boundaries.

Platform-level operations require explicit authorization.

---

# Persistence Rules

Queries MUST enforce tenant isolation.

Tenant enforcement SHOULD remain centralized and observable.

---

# Final Principle

Tenant isolation failures are considered critical architectural violations.