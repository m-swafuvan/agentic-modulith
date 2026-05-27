# API Standards

# Philosophy

APIs are contracts.

Contracts should remain stable, explicit, predictable, and observable.

---

# Rules

APIs MUST:

- validate inputs
- enforce authorization
- preserve tenant safety
- use explicit contracts
- return predictable responses

Avoid leaking internal persistence models directly.

---

# API Style Flexibility

The platform supports multiple API styles depending on business requirements.

Supported approaches may include:

- REST
- GraphQL
- gRPC
- WebSockets
- MQTT integration
- event-driven APIs

API style selection MUST be intentional and use-case driven.

Avoid introducing multiple API paradigms unnecessarily within the same bounded context.

---

# API Selection Guidance

Prefer:

- REST for standard business APIs
- GraphQL for aggregation-heavy querying
- gRPC for high-performance internal communication
- MQTT for lightweight event-driven device communication
- WebSockets for realtime bidirectional workflows

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

# Error Responses

Errors SHOULD:

- remain structured
- remain predictable
- avoid leaking internal details
- support observability and diagnostics