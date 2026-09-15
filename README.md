# Gorth

**Building an integrated ecosystem of digital products, platforms, and services.**

Gorth is a technology startup focused on building connected digital products
and shared technology infrastructure.

Our ecosystem brings together communication, content, productivity, social
experiences, commerce, identity, payments, discovery, and other platform
capabilities through a common technology foundation.

## Ecosystem

Gorth develops a collection of interconnected applications:

- **Gorth Video** — Video streaming and content platform.
- **Gorth Reader** — Digital reading platform for comics, manga, and novels.
- **Gorth Social** — Social networking and content-sharing platform.
- **Gorth Task** — Collaborative workspace and productivity platform.
- **Gorth Chat** — Real-time messaging platform connecting users across the Gorth ecosystem.
- **Gorth Marketplace** — Multi-vendor e-commerce marketplace.

## Platform Services

Applications share a common set of platform services:

- **Single Sign-On** — Identity, authentication, authorization, and organizations.
- **Notification Center** — Cross-platform notification delivery.
- **Resource Interaction** — Comments, reactions, bookmarks, ratings, and shared interactions.
- **Discovery Engine** — Search, suggestions, recommendations, and personalization.
- **Payment Gateway** — Payment processing and transaction infrastructure.
- **Billing & Subscription** — Plans, subscriptions, billing, and entitlements.
- **Media Processing** — Shared media storage, processing, and delivery.
- **Insight & Governance** — Analytics, reporting, auditing, moderation, and risk capabilities.

Gorth Chat also acts as the shared messaging infrastructure for applications
across the ecosystem.

## Architecture

Gorth follows a distributed, service-oriented architecture.

Each application owns its domain-specific business logic and data, while
cross-platform capabilities are provided by reusable platform services.

```text
                        Gorth Ecosystem

     ┌────────┬────────┬────────┬────────┬────────┬─────────────┐
     │ Video  │ Reader │ Social │  Task  │  Chat  │ Marketplace │
     └───┬────┴───┬────┴───┬────┴───┬────┴───┬────┴──────┬──────┘
         │        │        │        │        │           │
         └────────┴────────┴────┬───┴────────┴───────────┘
                                │
                    Shared Platform Services
                                │
        ┌───────────────────────┼────────────────────────┐
        │                       │                        │
     Identity                Discovery              Payments
     Messaging               Interaction            Billing
     Notification            Media                  Governance
