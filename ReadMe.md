# Credit Business settlement report

In a credit business, each customer can record their transactions for purchasing products and services using their credit card during the month, and at the end of each month, the customer's debt amount is determined, which they must repay. Each customer must repay 20% of their total outstanding balance at the end of each month, regardless of whether they made any purchases that month or not.

The amounts consumed and repaid during the month have no role in the repayment of the end-of-month and outstanding debts, and are only presented in a separate column in the final report.

For this purpose, two files are provided: one named PayTran containing the transactions of customers and their purchases in the form of records consisting of the customer's card ID, transaction date, transaction ID, and transaction amount, and another file named SetlTran containing the transactions of customer repayments, including the customer's card ID, transaction date, transaction ID, and repayment transaction amount.

The desired output is as follows:
DocumentNumber | BillDate | BillAmount | SettlDate | SettlAmount | PaybackPercent | CurrentMonthsettlement
--- | --- | --- | --- |--- |--- |--- 
1 | 1401/12 | 2,191,430 | 1402/01 | 2,191,430 | 100.00% | NULL
1 | 1402/01 | 100,000,000 | NULL | 0 | 0% | 2,070,200
1 | 1402/02 | 100,000,000 | 1402/03 | 20,000,000 | 20.00% | NULL
1 | 1402/03 | 80,000,000 | NULL | 0 | 0% | NULL
