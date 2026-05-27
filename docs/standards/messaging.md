# Messaging Standards

# Philosophy

Messaging should support decoupled workflows without introducing unnecessary distributed complexity.

The platform primarily targets modular monolith architectures.

Messaging inside the monolith SHOULD remain lightweight and observable.

---

# Supported Patterns

Supported messaging approaches may include:

- in-process domain events
- integration events
- background processing
- message queues
- publish/subscribe workflows

---

# MQTT Guidance

MQTT MAY be used for:

- IoT communication
- realtime telemetry
- device messaging
- lightweight event streaming
- low-bandwidth communication

MQTT usage SHOULD remain:

- event-oriented
- asynchronous
- observable
- resilient

---

# Event Design

Events SHOULD:

- remain immutable
- remain explicit
- avoid leaking internal persistence models
- contain only required data

Avoid tightly coupling modules through event contracts.

---

# Reliability

Messaging workflows SHOULD consider:

- retries
- idempotency
- dead-letter handling
- observability
- delivery guarantees

---

# Final Principle

Use messaging to reduce coupling, not to introduce unnecessary distributed architecture complexity.