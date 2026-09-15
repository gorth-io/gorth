# Governance

Gorth is developed as an integrated ecosystem of applications, platform
services, and shared technology.

## Project Ownership

Each Gorth project owns a clearly defined domain.

Application-specific functionality belongs to the application responsible for
that domain.

Capabilities required by multiple applications may be developed as reusable
platform services.

## Architecture

Major architectural changes should consider:

- Domain ownership
- Backward compatibility
- Security
- Service dependencies
- Data ownership
- Operational complexity
- Long-term maintainability

Services should not directly depend on another service's database.

Cross-service communication should occur through explicit interfaces and
stable identifiers.

## Decision Making

Project maintainers are responsible for technical decisions within their
respective projects.

Changes affecting multiple applications or platform-wide contracts require
ecosystem-level architectural review.

## Evolution

Governance may evolve as the Gorth organization, contributor community, and
engineering teams grow.
