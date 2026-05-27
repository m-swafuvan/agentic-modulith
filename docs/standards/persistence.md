# Persistence Standards

# Philosophy

Persistence should remain explicit, intentional, observable, and performance-oriented.

Data access should optimize for:

- maintainability
- query clarity
- predictable performance
- scalability

---

# Preferred Persistence Strategy

Preferred persistence approach:

- Dapper-first
- explicit SQL
- projection-oriented reads
- lightweight persistence abstractions

ORM-heavy architectures should be avoided for performance-sensitive systems.

---

# Rules

Persistence MUST:

- preserve ownership boundaries
- avoid hidden query generation
- remain feature-oriented
- remain testable
- optimize intentionally

Avoid:

- generic repositories
- god data services
- excessive ORM abstraction
- hidden persistence behavior
- lazy-loading-heavy architectures

---

# Query Philosophy

Prefer:

- explicit queries
- projections
- intentional indexing
- batching where appropriate
- optimized reads
- predictable execution plans

Avoid:

- N+1 queries
- unnecessary joins
- loading unused data
- repeated query execution

---

# Database Standards

Databases SHOULD:

- use explicit migrations
- remain reviewable
- use predictable naming
- include indexes intentionally

Destructive changes require explicit justification.

---

# Migration Philosophy

Migrations SHOULD:

- remain intentional
- avoid long-running locks
- remain backward-compatible where possible
- remain operationally safe

Never modify production schema manually.