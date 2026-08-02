<div align="center">

<img
  src="./assets/brand/anclora-fiscal-medalla-oro-transparente.png"
  alt="Anclora Fiscal"
  width="112"
/>

# Anclora Fiscal

### Traceable fiscal operations for digital commerce

A professional case study covering fiscal evidence ingestion, reconciliation,
invoicing, VAT-period preparation and regulatory-aware software architecture.

<br />

![Case study](https://img.shields.io/badge/type-case%20study-D7A957)
![Architecture](https://img.shields.io/badge/focus-software%20architecture-111827)
![Privacy](https://img.shields.io/badge/privacy-by%20design-047857)
![License](https://img.shields.io/badge/license-portfolio%20evaluation-7C3AED)

</div>

---

> [!IMPORTANT]
> This is a reduced professional portfolio repository. It does not contain the
> operational source code of Anclora Fiscal and does not provide tax, legal,
> accounting or regulatory advice.

## At a glance

| Product challenge | Engineering response |
|---|---|
| Fragmented sales evidence | Normalised ingestion workflow |
| Multiple commerce formats | Connector-based architecture |
| Duplicate and conflicting records | Idempotency and reconciliation controls |
| Fiscal-document traceability | Evidence-linked document lifecycle |
| VAT-period preparation | Readiness gates and dossier workflow |
| Regulatory-sensitive operations | Explicit limits, feature flags and auditability |

## Project context

Digital businesses frequently receive evidence from different platforms and in
different formats:

- Shopify orders;
- Shopify payment transactions;
- Amazon KDP royalty statements;
- received invoices and expenses;
- bank and settlement evidence.

Anclora Fiscal was designed to bring those sources into a controlled operational
workflow without treating raw imports as automatically trustworthy.

## What the complete product demonstrates

- defensive file ingestion;
- preview before confirmation;
- schema and business-rule validation;
- duplicate prevention;
- evidence normalisation;
- payment and settlement reconciliation;
- fiscal-document issuance and rectification;
- VAT-period readiness;
- traceable dossiers;
- authentication and role controls;
- preparation for VERI*FACTU-related workflows;
- automated quality gates.

## Architecture overview

```text
External evidence
      │
      ▼
┌──────────────────────┐
│ Import connectors    │
│ Shopify · KDP · CSV  │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ Validation and       │
│ normalisation        │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ Traceable operations │
│ and reconciliation   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ Fiscal documents,    │
│ VAT and audit output │
└──────────────────────┘
```

The complete implementation used explicit boundaries between:

| Layer | Responsibility |
|---|---|
| Web application | Operator workflows and review interfaces |
| API | Authentication, orchestration and controlled mutations |
| Connectors | Source-specific parsing and normalisation |
| Core domain | Invoicing, matching, dossiers and integrity logic |
| Tax engine | Deterministic fiscal decisions |
| Persistence | Repositories, migrations and audit evidence |
| UI system | Reusable components and visual consistency |

## Core workflow

### 1. Ingest

A source file is identified, parsed and converted into an internal representation.

### 2. Validate

Structural errors, missing evidence, unsupported values and conflicting records
are detected before confirmation.

### 3. Confirm

Only reviewed records proceed to persistent operations. Idempotency controls
prevent accidental duplication.

### 4. Reconcile

Orders, payments, fees, refunds and settlements are compared and linked.

### 5. Prepare

Validated operations are made available for invoicing, VAT review and evidence
dossier generation.

## Key engineering decisions

### Traceability before automation

The system preserves where information came from, what transformation was
performed and which operator action confirmed it.

### Preview before persistence

Imports are not trusted automatically. The user first sees a reviewable preview
with warnings and blocking issues.

### Idempotent processing

Repeated uploads or retried requests must not create duplicate fiscal operations.

### Human review for sensitive decisions

Ambiguous fiscal or reconciliation cases remain visible instead of being silently
resolved.

### Regulatory limits

Potentially sensitive functionality is isolated behind explicit readiness gates
and conservative product language.

## Security and privacy

The complete product was designed around:

- least-privilege access;
- role-based permissions;
- signed sessions;
- auditable authentication;
- protected sensitive actions;
- encrypted import metadata;
- no real commerce exports in source control;
- controlled retention;
- production feature flags;
- separation between demonstration and production environments.

See [Security and privacy](./docs/SECURITY_AND_PRIVACY.md).

## Quality strategy

The private implementation included:

- TypeScript strict mode;
- ESLint;
- unit and integration tests;
- UI tests;
- migration tests;
- production builds;
- dependency auditing;
- continuous integration;
- synthetic fixtures;
- regression coverage for import, reconciliation and invoicing workflows.

See [Quality strategy](./docs/QUALITY.md).

## Technology profile

| Area | Technologies used in the complete product |
|---|---|
| Frontend | Next.js, React, TypeScript |
| API | Fastify, Zod, OpenAPI |
| Data | PostgreSQL, Drizzle ORM |
| Local testing | PGlite |
| Architecture | pnpm workspaces, Turborepo |
| Testing | Vitest, Testing Library, Playwright |
| Deployment | Vercel-oriented web and API builds |

## Repository contents

```text
anclora-fiscal/
├── assets/
│   └── brand/
├── docs/
│   ├── ARCHITECTURE.md
│   ├── CASE_STUDY.md
│   ├── QUALITY.md
│   └── SECURITY_AND_PRIVACY.md
├── LICENSE
├── NOTICE.md
└── README.md
```

## Documentation

- [Detailed case study](./docs/CASE_STUDY.md)
- [Architecture](./docs/ARCHITECTURE.md)
- [Security and privacy](./docs/SECURITY_AND_PRIVACY.md)
- [Quality strategy](./docs/QUALITY.md)
- [Portfolio notice](./NOTICE.md)

## Scope and limitations

This public repository does not include enough implementation detail to run,
reproduce or commercially deploy Anclora Fiscal.

It demonstrates the author's approach to:

- product definition;
- complex domain modelling;
- full-stack architecture;
- financial-data traceability;
- defensive software design;
- security;
- automated testing;
- regulatory-aware engineering.

---

<div align="center">

### Antonio Ballesteros

Product-oriented developer focused on business automation, applied AI and
traceable digital systems.

[![GitHub](https://img.shields.io/badge/GitHub-ToniIAPro73-181717?logo=github)](https://github.com/ToniIAPro73)

</div>
