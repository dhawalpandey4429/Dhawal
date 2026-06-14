\#\# Section 4 — FK Consistency Requirements

\#\#\# Service Name Consistency

The service field must use identical values across all records.

Allowed values:

\- Electricity  
\- Internet  
\- Mobile  
\- Insurance

\---

\#\#\# Electricity Relationships

billing\_notices.csv  
service \= Electricity

payment\_confirmations.csv  
service \= Electricity

transactions.csv  
service \= Electricity

household\_expense\_tracker.xlsx  
service \= Electricity

\---

\#\#\# Internet Relationships

billing\_notices.csv  
service \= Internet

internet\_invoice.pdf  
service \= Internet

household\_expense\_tracker.xlsx  
service \= Internet

\---

\#\#\# Mobile Relationships

mobile\_bill.pdf  
service \= Mobile

transactions.csv  
service \= Mobile

household\_expense\_tracker.xlsx  
service \= Mobile

\---

\#\#\# Insurance Relationships

insurance\_invoice.pdf  
service \= Insurance

payment\_confirmations.csv  
service \= Insurance

transactions.csv  
service \= Insurance

household\_expense\_tracker.xlsx  
service \= Insurance

\---

\#\#\# Amount Consistency Rules

Electricity  
Invoice Amount \= Transaction Amount \= Confirmation Amount

Internet  
Invoice Amount \= Billing Notice Amount

Mobile  
Invoice Amount ≠ Transaction Amount

Insurance  
Invoice Amount \= Transaction Amount \= Confirmation Amount  
