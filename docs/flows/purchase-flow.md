# Purchase Flow

This flow represents how physical goods enter the business.

The system records the acceptance of merchandise, not the commercial negotiation.

---

## Step 1 — Supplier delivers goods

A supplier arrives with a legal document (invoice).

At this moment the business decides whether to accept the merchandise.

No inventory exists yet in the system.

---

## Step 2 — Purchase confirmation

When the business accepts the goods, a purchase is confirmed.

This event authorizes inventory creation.

purchase → legal acceptance

---

## Step 3 — Batch creation

Each product is stored as a physical batch.

A batch contains:

- quantity
- unit cost
- expiration date
- branch location

stock is created only here

---

## Step 4 — Inventory movements

The system records the incoming movement:

+ quantity from supplier

The inventory history begins at this point.

---

## Result

After confirmation:

- inventory exists
- cost becomes historical
- the business may owe the supplier
- no money has moved yet
