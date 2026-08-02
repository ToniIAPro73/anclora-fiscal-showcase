# Security and privacy

## Core controls

- Authentication and session protection.
- Role-based access control.
- Audit events for sensitive actions.
- Encrypted import metadata.
- Input and file validation.
- Rate limiting.
- Idempotency.
- Restricted error responses.
- No production secrets in source control.
- No real customer or fiscal exports in public repositories.

## Data-handling principles

### Minimise

Only information required for the fiscal workflow should be processed.

### Separate

Source evidence, normalised operations and generated documents should remain
distinct entities.

### Trace

Every important transformation should be attributable to its source and actor.

### Restrict

Sensitive workflows should require explicit permissions and production flags.

### Retain deliberately

Retention periods must be based on operational and legal requirements rather than
indefinite storage by default.

## Public repository policy

The operational source code and infrastructure are private.

This public case study contains no credentials, customer data, fiscal exports,
production certificates or complete regulatory implementation.
