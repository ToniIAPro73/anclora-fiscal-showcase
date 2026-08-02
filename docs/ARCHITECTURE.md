# Architecture

## Architectural objective

Anclora Fiscal separates source-specific ingestion from fiscal-domain decisions.

This prevents platform-specific formats from leaking directly into invoicing,
tax-period or regulatory workflows.

## Conceptual layers

### Presentation

Responsible for operator workflows, previews, review screens and evidence status.

### Application services

Coordinates imports, reconciliation, document issuance and period preparation.

### Connectors

Translates external files into normalised records without making fiscal decisions.

### Domain

Contains deterministic rules for matching, invoicing, evidence and readiness.

### Persistence

Stores traceable entities, relationships, audit events and idempotency keys.

### External services

Represents storage, email, commerce platforms and regulatory endpoints behind
replaceable interfaces.

## Design principles

- Explicit boundaries.
- Idempotent mutations.
- Immutable source evidence.
- Human review for ambiguity.
- Auditability.
- Least privilege.
- Conservative regulatory claims.
