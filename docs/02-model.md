# Domain Model

REXIRA is not a CRUD inventory system.

The model is based on real-world business events instead of mutable state.

## Core Concepts

### Product is not Inventory
A product defines what is sold commercially.
Inventory represents physical units that exist in the real world.

Stock exists only through batches.

product → definition
stock_batch → physical existence

---

### A Sale is not Money
A sale represents a commitment from a customer.
Money exists only when a payment is registered.

sale → obligation
payment → cash movement

---

### Inventory is never edited
Stock cannot be modified directly.

It only changes through events:

- purchase (incoming stock)
- sale (outgoing stock)
- adjustment (correction)
- transfer (location change)

The current stock is reconstructed from movements.

---

### History is immutable
Past operations never change.

Prices and costs are frozen at the moment of the transaction.
Reports are generated from history, not recalculated from current values.

---

### Financial separation
The system tracks three independent flows:

1) Physical goods movement
2) Commercial obligation
3) Real money movement

They are related but never merged.
