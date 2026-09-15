# Gorth Architecture

## Overview

Gorth is an ecosystem of independent applications built on reusable platform
services.

The architecture separates application-specific business domains from
capabilities that are shared across the ecosystem.

## Applications

The primary Gorth applications are:

- Video
- Reader
- Social
- Task
- Chat
- Marketplace

Each application owns its business domain and application-specific data.

## Platform Services

Shared capabilities include:

- Identity and authentication
- Notifications
- Resource interactions
- Discovery and recommendation
- Messaging
- Payments
- Billing and subscriptions
- Media processing
- Analytics and governance

## Data Ownership

Each application and service owns its data.

A service must not create database foreign keys into another service's
database.

External identifiers are used when references across service boundaries are
required.

## Communication

Applications communicate with platform services through explicit APIs and
authenticated service contracts.

User authorization and application authorization are treated as separate
concerns.

## Identity

The Gorth Single Sign-On service is the global identity source of truth.

Applications may maintain local user projections when necessary for
performance, relationships, or application-specific data.

## Shared Resources

Generic interactions may reference resources through identifiers such as:

```text
resourceType
resourceId
