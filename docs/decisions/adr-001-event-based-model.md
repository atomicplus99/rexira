# ADR-001: Event-Based Transactional Model

## Context

Traditional POS systems store current values such as stock and balance.

This causes inconsistencies because history cannot be reconstructed.

Retail operations require auditability and financial traceability.

## Decision

The system will store business events instead of mutable state.

Stock and balances will be reconstructed from movements.

## Consequences

### Positive

- Full auditability
- Historical reconstruction
- Real profit calculation
- No hidden corrections

### Negative

- More complex queries
- Larger data volume
- Requires strict invariants

## Status

Accepted
