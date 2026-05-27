# Validation Standards

# Philosophy

Validation should remain:

- explicit
- predictable
- focused
- testable

Avoid hidden framework-driven validation behavior.

---

# Rules

Validation SHOULD:

- stay close to the feature
- return predictable errors
- remain framework-independent
- avoid duplicated business rules

Validation is part of business correctness, not only API correctness.

---

# Error Handling

Validation errors SHOULD:

- remain structured
- remain predictable
- avoid leaking internal details
- remain client-consumable

---

# Final Principle

Validation should improve correctness without introducing unnecessary complexity.