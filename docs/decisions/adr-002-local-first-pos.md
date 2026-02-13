# ADR-002: Local-First POS Operation

## Context

Retail stores cannot stop operating when internet connectivity fails.

An online-only system would block sales and cause business interruption.

## Decision

The POS must operate locally and synchronize events with a central server later.

The local database is operational.
The central system is the historical source of truth.

## Consequences

### Positive

- Continuous operation
- Fast transactions
- Network independence

### Negative

- Synchronization complexity
- Event ordering requirements
- Conflict handling

## Status

Accepted
