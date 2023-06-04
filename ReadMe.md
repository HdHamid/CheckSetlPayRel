# Credit Business settlement report

In a credit business, each customer can recorIn a credit business, each customer can register their transactions for purchasing products and services using their credit card throughout the month, and at the end of each month, the amount owed by the customer is determined, which they must repay. Each customer will have a remaining balance at the end of each month and must take action to repay it.

The amounts consumed during the month that are repaid in the same month do not affect the repayment of the end-of-month debt and remaining balance and are only presented in another column in the final report.

For this purpose, two files are provided: one named PayTran containing customer transactions and their purchases in the form of records including the customer's card ID, transaction date, transaction ID, and transaction amount, and another file named SetlTran containing customer repayment transactions including the customer's card ID, transaction date, transaction ID, and repayment transaction amount.

The desired output is as follows:
DocumentNumber | BillDate | BillAmount | SettlDate | SettlAmount | PaybackPercent | CurrentMonthsettlement
--- | --- | --- | --- |--- |--- |--- 
1 | 1401/12 | 2,191,430 | 1402/01 | 2,191,430 | 100.00% | NULL
1 | 1402/01 | 100,000,000 | NULL | 0 | 0% | 2,070,200
1 | 1402/02 | 100,000,000 | 1402/03 | 20,000,000 | 20.00% | NULL
1 | 1402/03 | 80,000,000 | NULL | 0 | 0% | NULL
