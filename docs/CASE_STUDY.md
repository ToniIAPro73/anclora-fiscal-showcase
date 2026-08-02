# Case study

## Problem

A digital publisher and online seller may receive separate exports for orders,
payments, refunds, fees, royalties and expenses.

Manual consolidation creates several risks:

- duplicate records;
- missing payment evidence;
- inconsistent currencies;
- incorrect links between orders and settlements;
- poor auditability;
- premature fiscal decisions.

## Product response

Anclora Fiscal introduced a staged workflow:

1. identify the evidence source;
2. parse it defensively;
3. produce a preview;
4. surface warnings and blocking issues;
5. require confirmation;
6. persist idempotently;
7. reconcile related operations;
8. prepare fiscal outputs.

## Main challenges

### Heterogeneous source formats

Each commerce platform models transactions differently.

### Partial evidence

An order, payment and settlement can arrive at different times.

### Refunds and negative movements

Negative values require correct semantic treatment rather than simple aggregation.

### Fiscal traceability

Generated documents must remain linked to their originating operations and
decisions.

### Regulatory-sensitive functionality

VERI*FACTU preparation required clear separation between technical preparation,
preproduction validation and any claim of production readiness.

## Outcome

The project demonstrates how to transform an ambiguous operational problem into a
structured, testable and auditable software product.
