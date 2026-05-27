# Workflow Standards

# Feature Workflow

When implementing a feature:

1. identify the owning module
2. inspect existing patterns
3. preserve architecture consistency
4. implement the feature in isolated slices
5. add validation
6. add authorization
7. enforce tenant safety
8. add observability where needed
9. add tests
10. update documentation if necessary

---

# Change Management

Changes SHOULD remain:

- focused
- isolated
- reviewable
- predictable

Avoid unrelated refactors during feature implementation.

---

# Performance Review Requirements

All features MUST be reviewed for:

- algorithmic complexity
- database query efficiency
- allocation behavior
- serialization overhead
- network overhead
- unnecessary loops
- redundant queries
- caching opportunities

Avoid:

- O(n²) operations where unnecessary
- repeated database calls in loops
- loading unnecessary data
- blocking I/O
- excessive object mapping
- hidden query generation

Performance-sensitive paths SHOULD include benchmarking or profiling where appropriate.

---

# Definition of Done

A feature is NOT complete unless:

- boundaries are preserved
- authorization is enforced
- tenant safety is verified
- validation exists
- tests are added
- observability is considered
- naming conventions are followed
- no dead code is introduced