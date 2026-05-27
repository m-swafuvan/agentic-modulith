# Agentic-Modulith

AI-native modular monolith starter built with ASP.NET Core, PostgreSQL, React, and Docker.

Designed for scalable enterprise architecture, low-cost deployment, and seamless agentic coding workflows across GitHub Copilot, Claude, and Codex.

---

# Why agentic-modulith?

Modern applications often become difficult to maintain due to:

* tightly coupled architectures
* uncontrolled abstractions
* premature microservices adoption
* inconsistent AI-generated code

`agentic-modulith` solves this by providing:

* a modular monolith architecture
* strong architectural boundaries
* AI-agent friendly repository conventions
* production-grade engineering practices
* low operational complexity
* future-ready scalability

This repository is optimized for:

* AI-assisted development
* long-term maintainability
* clean architecture
* fast developer onboarding
* enterprise-grade scalability

---

# Tech Stack

## Backend

* ASP.NET Core 10
* PostgreSQL

## Frontend

* React
* JavaScript
* Vite
* React Query

## Infrastructure

* Docker
* Docker Compose
* NGINX
* OpenTelemetry

---

# Architecture

This project follows a **Modular Monolith Architecture**.

Instead of splitting systems into microservices too early, the application is organized into isolated modules with explicit boundaries while remaining deployable as a single unit.

Benefits:

* simpler deployments
* lower infrastructure cost
* faster development velocity
* easier debugging
* future microservice extraction capability

Example structure:

```txt id="53pgre"
modules/
  auth/
  users/
  billing/
  notifications/
```

Each module owns:

* business logic
* validation
* persistence
* contracts
* application workflows

---

# AI-Native Development

This repository is designed specifically for modern AI-assisted engineering workflows.

Supported tools:

* GitHub Copilot
* Claude Code
* OpenAI Codex

The repository includes:

* `AGENTS.md`
* `CLAUDE.md`
* Copilot instructions
* architecture documentation
* coding standards
* task-driven workflows

These conventions help AI agents:

* generate consistent code
* preserve architectural boundaries
* avoid unnecessary abstractions
* follow repository standards

---

# Repository Structure

```txt id="7t6v6l"
apps/
  api/
  web/

modules/
  auth/
  users/
  billing/
  notifications/

infrastructure/
  persistence/
  observability/
  caching/

docs/
  architecture.md
  coding-standards.md
  ai-workflow.md
```

---

# Getting Started

## Prerequisites

* .NET 10 SDK
* Node.js LTS
* Docker
* PostgreSQL

---

## Start Development Environment

```bash id="ns0qye"
docker compose up
```

---

## Backend

```bash id="zhny52"
cd apps/api

dotnet restore
dotnet build
dotnet run
```

---

## Frontend

```bash id="7ntiyd"
cd apps/web

npm install
npm run dev
```

---

# Development Principles

This repository prioritizes:

* modularity over complexity
* explicitness over magic
* maintainability over cleverness
* scalability over premature optimization

Guidelines:

* keep modules isolated
* prefer composition over inheritance
* keep files small and focused
* avoid speculative abstractions
* enforce consistent patterns

---

# Deployment Philosophy

The application is intentionally designed to:

* deploy as a single unit initially
* minimize operational overhead
* reduce infrastructure costs
* scale incrementally when needed

Recommended hosting:

* Hetzner
* Railway
* Fly.io
* Coolify

---

# Long-Term Vision

`agentic-modulith` aims to become a production-grade foundation for:

* enterprise applications
* SaaS platforms
* internal tooling
* AI-native engineering workflows
* scalable modular systems

without introducing unnecessary operational complexity.

---

# License

MIT
