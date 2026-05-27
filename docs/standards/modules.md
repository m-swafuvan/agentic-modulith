# Module Standards

# Purpose

Modules are the primary unit of ownership.

Every module should represent a business capability or bounded context.

Modules MUST remain independently understandable and maintainable.

---

# Module Responsibilities

Each module owns:

- domain rules
- persistence
- contracts
- validation
- authorization
- endpoints
- workflows
- events

Modules SHOULD remain cohesive and internally consistent.

---

# Dependency Rules

Modules MUST NOT:

- directly access another module's persistence
- bypass contracts
- introduce circular dependencies
- leak internal implementation details
- depend on internal implementation behavior of another module

Shared logic belongs only in explicitly approved shared abstractions.

---

# Communication Rules

Preferred communication approaches:

- contracts
- internal events
- explicit interfaces
- messaging abstractions

Avoid hidden coupling.

---

# Structure Philosophy

Prefer:

- feature-oriented organization
- isolated slices
- focused modules
- explicit ownership
- predictable structures

Avoid:

- giant shared service layers
- highly coupled utilities
- cross-cutting god services

---

# Internal Eventing

Modules MAY communicate through:

- domain events
- integration events
- internal messaging

Messaging SHOULD reduce coupling, not introduce unnecessary complexity.