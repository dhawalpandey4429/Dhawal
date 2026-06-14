# **trap\_ledger.md**

## **T1 — Cross-Source Contradiction**

Trap Type:  
Cross-Source Contradiction

Location:

* household\_expense\_tracker.xlsx  
* payment\_confirmations.csv  
* transactions.csv

Planted Conflict:  
Electricity is marked "Unpaid" in the expense tracker.

Ground Truth:  
Electricity payment was completed.

Evidence:

* payment\_confirmations.csv  
* transactions.csv

Expected Resolution:  
Trust payment confirmation records and transaction records over the tracker entry.

---

## **T2 — Cross-Source Contradiction**

Trap Type:  
Cross-Source Contradiction

Location:

* household\_expense\_tracker.xlsx  
* payment\_confirmations.csv  
* transactions.csv

Planted Conflict:  
Insurance is marked "Unpaid" in the expense tracker.

Ground Truth:  
Insurance payment was completed.

Evidence:

* payment\_confirmations.csv  
* transactions.csv

Expected Resolution:  
Trust payment confirmation records and transaction records over the tracker entry.

---

## **T3 — Missing Payment Evidence**

Trap Type:  
Outstanding Obligation

Location:

* internet\_invoice.pdf  
* billing\_notices.csv  
* transactions.csv

Planted Conflict:  
Internet invoice exists.  
Internet overdue notice exists.

Ground Truth:  
No payment transaction exists.

Evidence:

* internet\_invoice.pdf  
* billing\_notices.csv

Expected Resolution:  
Classify the internet bill as outstanding.

---

## **T4 — Amount Reconciliation**

Trap Type:  
Multi-Source Reconciliation

Location:

* mobile\_bill.pdf  
* transactions.csv

Planted Conflict:  
Mobile invoice amount \= $68.  
Mobile payment amount \= $60.

Ground Truth:  
Payment amount does not match billed amount.

Evidence:

* mobile\_bill.pdf  
* transactions.csv

Expected Resolution:  
Identify an $8 payment discrepancy.

---

## **T5 — Decoy Evidence**

Trap Type:  
Noise Artifact

Location:

* family\_trip\_itinerary.pdf  
* school\_activity\_schedule.pdf  
* community\_fair\_flyer.pdf

Planted Conflict:  
Documents appear legitimate.

Ground Truth:  
Documents contain no billing evidence.

Evidence:  
None.

Expected Resolution:  
Exclude these files from discrepancy analysis.

