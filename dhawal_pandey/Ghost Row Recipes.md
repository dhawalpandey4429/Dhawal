\#\# Section 5 — Ghost Row Recipes

\#\#\# GR-01 Previous Billing Cycle

Purpose:  
Introduce historical billing activity.

Implementation:  
Add an electricity bill from the previous month.

Rules:  
\- Different billing period.  
\- Different due date.  
\- Fully paid.  
\- Must not affect current-month findings.

\---

\#\#\# GR-02 Closed Service Record

Purpose:  
Introduce a completed obligation.

Implementation:  
Add a historical household service payment.

Rules:  
\- Status \= Completed.  
\- Service not referenced by current GTFA.  
\- No outstanding balance.

\---

\#\#\# GR-03 Duplicate-Looking Notice

Purpose:  
Create review noise.

Implementation:  
Add an older billing notice for Internet service.

Rules:  
\- Earlier date.  
\- Different notice identifier.  
\- Must not override current overdue notice.

\---

\#\#\# GR-04 Historical Payment Confirmation

Purpose:  
Increase transaction volume.

Implementation:  
Add an older payment confirmation record.

Rules:  
\- Different billing period.  
\- Different confirmation identifier.  
\- No impact on current discrepancies.

\---

\#\#\# GR-05 Archived Expense Entry

Purpose:  
Add spreadsheet noise.

Implementation:  
Add a fully reconciled historical expense.

Rules:  
\- Historical date.  
\- Paid status.  
\- No linkage to current findings.  
