\#\# Section 3 — Value Alignment Table

| GTFA Finding | Plant Field | Artifact Source | Mock Data Source | Validation Method |  
|--------------|-------------|----------------|------------------|------------------|  
| Electricity bill paid but marked unpaid | ELECTRICITY\_PAYMENT\_STATUS | household\_expense\_tracker.xlsx | payment\_confirmations.csv | Compare tracker status against confirmation status |  
| Electricity bill paid but marked unpaid | ELECTRICITY\_TRANSACTION\_STATUS | household\_expense\_tracker.xlsx | transactions.csv | Compare tracker status against transaction status |  
| Internet bill remains outstanding | INTERNET\_PAYMENT\_STATUS | internet\_invoice.pdf | billing\_notices.csv | Verify absence of payment evidence |  
| Mobile payment amount differs from billed amount | MOBILE\_BILL\_AMOUNT | mobile\_bill.pdf | transactions.csv | Compare billed amount against transaction amount |  
| Insurance premium paid but marked unpaid | INSURANCE\_PAYMENT\_STATUS | household\_expense\_tracker.xlsx | payment\_confirmations.csv | Compare tracker status against confirmation status |  
| Insurance premium paid but marked unpaid | INSURANCE\_TRANSACTION\_STATUS | household\_expense\_tracker.xlsx | transactions.csv | Compare tracker status against transaction status |  
