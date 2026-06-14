# Part B — Design Intent

## B1 — Focal Event

Amber Jenkins is reviewing household expense records to determine which recurring-service obligations have been paid, which remain outstanding, and whether any recordkeeping discrepancies exist.

The task requires reconciliation across invoices, billing notices, payment confirmations, transaction records, account statements, screenshots, and an expense tracker.

The final objective is to produce an evidence-backed discrepancy report.

---

## B2 — Scope Boundary

### In Scope

- Household utility bills
- Internet service bills
- Mobile service bills
- Insurance premium payments
- Payment confirmations
- Billing notices
- Payment transactions
- Expense tracker entries

### Out of Scope

- Community activities
- School events
- Travel planning
- Membership registrations
- General household lifestyle content
- Non-financial records

---

## B3 — Trap Design Summary

### Trap T1
Cross-source contradiction involving electricity payment status.

### Trap T2
Cross-source contradiction involving insurance payment status.

### Trap T3
Missing payment evidence for the internet bill.

### Trap T4
Amount mismatch between mobile invoice and payment transaction.

### Trap T5
Noise artifacts designed to appear plausible while contributing no evidence.

### Expected Reasoning Behavior

- Reconcile records across multiple sources.
- Prioritize payment evidence over tracker entries.
- Distinguish outstanding obligations from completed payments.
- Compare billed amounts against paid amounts.
- Ignore irrelevant artifacts.
