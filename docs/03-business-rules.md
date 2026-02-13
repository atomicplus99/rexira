# Business Rules (Invariants)

These rules must never be violated by the system.

They represent accounting and operational constraints, not UI behavior.

---

## Inventory

- Stock cannot be edited manually
- Every stock unit must have an origin
- Every stock output must reference a specific batch
- Current stock must be reconstructable from movements

---

## Sales

- A sale does not imply payment
- A sale can exist without money received
- Cancelling a sale does not delete it, it creates a compensating operation

---

## Payments

- Payments register money, not products
- Payments must reference a document
- A payment cannot exist without a cash movement

---

## Accounting Integrity

- Historical prices never change
- Historical costs never change
- Reports must be reproducible at any future time

---

## Auditability

The system must always answer:

- Who performed the operation
- When it happened
- What physical units were affected
- What financial impact occurred
