# Performance Standards

# Philosophy

Performance is a core engineering responsibility.

Systems generated from this platform SHOULD remain performant by default, not by later optimization efforts.

---

# Core Principles

Prefer:

- explicit behavior
- predictable execution
- low allocation patterns
- efficient queries
- batching
- projections
- async I/O
- streaming where appropriate

Avoid:

- N+1 queries
- unnecessary abstraction layers
- reflection-heavy execution
- hidden allocations
- repeated enumeration
- synchronous blocking
- excessive serialization
- large object graphs

---

# Complexity Rules

Engineers MUST consider:

- time complexity
- space complexity
- database query complexity
- network overhead
- memory allocations

Avoid unnecessary:

- nested loops
- repeated scans
- redundant transformations
- repeated materialization
- unnecessary LINQ chaining in hot paths

---

# Persistence Performance

Persistence layers SHOULD:

- use explicit queries
- load only required data
- use projections intentionally
- batch operations where possible
- avoid chatty database access

N+1 query patterns are forbidden.

---

# API Performance

APIs SHOULD:

- support pagination
- support filtering
- avoid oversized payloads
- avoid excessive serialization depth
- support cancellation tokens where applicable

Streaming SHOULD be considered for large datasets.

---

# Benchmarking

Performance-sensitive workflows SHOULD support benchmarking.

Systems SHOULD provide:

- request timing visibility
- query timing visibility
- profiling support
- endpoint performance metrics
- tracing

Performance regressions SHOULD be measurable.

---

# Observability

Performance metrics SHOULD be observable through:

- structured logs
- tracing
- metrics
- dashboards
- profiling tools

---

# Final Principle

Readable systems are important.

Predictably performant systems are mandatory.