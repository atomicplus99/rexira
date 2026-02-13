# Cash Register Flow

The cash register represents real money inside the business.

It is independent from sales and inventory.

---

## Opening

A cashier opens a cash register session.

An initial balance is declared.

open_cash → starting real money

---

## During operation

Money can move due to:

- sale payments
- manual income
- expenses
- corrections

Each operation generates a cash movement.

cash_movements → money history

---

## Closing

At the end of the shift the cashier closes the register.

The system calculates:

expected_balance = initial + incomes - expenses

The physical count must match the calculated value.

---

## Result

The system can determine:

- real money present
- discrepancies
- responsibility by user and time
