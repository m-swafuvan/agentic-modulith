# AGENTS.md

# AI Governance Entry Point

This repository is an AI-governed software engineering platform designed for building scalable, maintainable, modular, and multitenant systems.

AGENTS.md is the canonical entry point for all AI agents, assistants, copilots, generators, and contributors working inside this repository.

All implementations MUST follow the standards and governance documents referenced below.

---

# Core Responsibilities

All generated systems MUST prioritize:

- architecture consistency
- modularity
- maintainability
- tenant isolation
- security
- observability
- scalability
- developer velocity
- explicitness over hidden behavior

Avoid unnecessary complexity and speculative abstractions.

---

# Required Reading Order

Before making changes, AI agents MUST read the following documents in order.

## 1. Architecture Standards

Read:

```txt
docs/standards/architecture.md
```

Defines:

- architectural philosophy
- module boundaries
- layering rules
- vertical slice expectations
- coupling restrictions
- implementation patterns

---

## 2. Module Ownership Standards

Read:

```txt
docs/standards/modules.md
```

Defines:

- module responsibilities
- ownership boundaries
- allowed communication patterns
- dependency rules
- cross-module interaction constraints

---

## 3. Feature Implementation Workflow

Read:

```txt
docs/standards/workflow.md
```

Defines:

- feature implementation lifecycle
- implementation expectations
- review expectations
- definition of done
- required engineering discipline

---

## 4. Multitenancy Standards

Read:

```txt
docs/standards/multitenancy.md
```

Defines:

- tenant isolation rules
- tenant resolution
- tenancy models
- tenant-safe implementation expectations
- cross-tenant access restrictions

---

## 5. Authorization Standards

Read:

```txt
docs/standards/authorization.md
```

Defines:

- RBAC rules
- permission models
- authorization enforcement expectations
- tenant-aware authorization
- security boundaries

---

## 6. Validation Standards

Read:

```txt
docs/standards/validation.md
```

Defines:

- validation philosophy
- validation structure
- error handling expectations
- framework independence rules

---

## 7. Persistence Standards

Read:

```txt
docs/standards/persistence.md
```

Defines:

- persistence ownership
- query expectations
- migration rules
- repository rules
- database conventions

---

## 8. API Standards

Read:

```txt
docs/standards/api.md
```

Defines:

- API conventions
- response contracts
- pagination rules
- versioning expectations
- error response standards

---

## 9. Frontend Standards

Read:

```txt
docs/standards/frontend.md
```

Defines:

- frontend architecture
- module-oriented UI rules
- state management expectations
- component structure
- frontend implementation conventions

---

## 10. Observability Standards

Read:

```txt
docs/standards/observability.md
```

Defines:

- logging expectations
- tracing expectations
- metrics
- auditability
- structured logging conventions

---

## 11. Testing Standards

Read:

```txt
docs/standards/testing.md
```

Defines:

- testing strategy
- architecture testing expectations
- tenant isolation testing
- authorization testing
- integration testing expectations

---

## 12. Naming Standards

Read:

```txt
docs/standards/naming.md
```

Defines:

- naming conventions
- terminology consistency
- forbidden naming patterns
- domain naming expectations

---

# Architecture Governance Rules

All generated features MUST:

- preserve module boundaries
- remain tenant-safe
- enforce authorization correctly
- remain observable
- remain testable
- follow existing conventions
- avoid hidden coupling
- avoid architecture drift

AI agents MUST:

- inspect existing patterns before generating code
- reuse established conventions
- avoid introducing unnecessary frameworks
- avoid speculative abstractions
- keep implementations focused and maintainable

---

# Decision Hierarchy

When making implementation decisions, prioritize:

1. Security
2. Tenant isolation
3. Architecture consistency
4. Maintainability
5. Readability
6. Simplicity
7. Scalability
8. Performance
9. Developer velocity

Prefer explicit implementations over hidden magic.

---

# Forbidden Patterns

Do NOT introduce:

- premature microservices
- distributed complexity without operational need
- generic repositories
- service locator patterns
- god classes
- hidden framework behavior
- architecture bypasses
- cross-module database access
- speculative abstractions
- tightly coupled modules
- shared mutable global state

---

# AI Contribution Expectations

Before implementing a feature:

1. Identify the owning module
2. Read the relevant standards
3. Follow existing patterns
4. Preserve architecture consistency
5. Keep changes isolated
6. Add required validation
7. Add authorization enforcement
8. Add tests
9. Preserve tenant safety

Before finalizing changes:

- verify architecture boundaries
- verify tenant isolation
- verify authorization enforcement
- run tests
- check formatting
- avoid unrelated refactors

---

# Documentation Expectations

When introducing:

- new architectural patterns
- new infrastructure capabilities
- new module communication patterns
- new tenancy strategies
- new authorization behaviors

AI agents SHOULD update:

```txt
docs/standards/
docs/architecture/
docs/decisions/
```

where appropriate.

---

# ADR Expectations

Architectural decisions SHOULD be documented inside:

```txt
docs/decisions/
```

Especially for:

- major framework changes
- infrastructure changes
- persistence strategy changes
- multitenancy strategy changes
- authorization model changes
- communication pattern changes

---

# Final Principle

This repository exists to ensure that AI-generated systems remain:

- maintainable
- modular
- secure
- scalable
- observable
- predictable
- production-ready

The objective is disciplined engineering through AI-assisted development.