# Frontend Standards

# Philosophy

Frontend systems should preserve modular ownership and maintainability at scale.

Frontend architecture should remain framework-flexible.

---

# Rules

Frontend systems MUST:

- separate UI from business logic
- preserve module ownership
- avoid uncontrolled global state
- remain scalable and maintainable

---

# Structure

Prefer:

- feature-oriented organization
- isolated modules
- focused reusable components
- predictable state boundaries

Avoid:

- giant shared folders
- duplicated business logic
- tightly coupled screens

---

# State Management

State SHOULD remain:

- predictable
- isolated
- observable
- minimal

Avoid unnecessary global state.

---

# UX Philosophy

Prioritize:

- consistency
- responsiveness
- accessibility
- simplicity
- predictable interaction patterns