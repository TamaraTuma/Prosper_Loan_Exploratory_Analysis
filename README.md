# Prosper_Loan_Exploratory_Analysis


# Overview

The Prosper Loan dataset contains a comprehensive collection of attributes related to loan listings on the Prosper loan platform. These listings represent individual loan opportunities made available to the public for investment and borrowing purposes. The dataset encompasses various key aspects of each loan listing, ranging from unique identifiers and borrower details to credit ratings and financial information.

# Key Attributes:
1. ListingKey: A unique identifier for each loan listing, serving as a reference to the corresponding listing object in the API.
2. ListingNumber: An identifier displayed on the Prosper website to uniquely identify each loan listing publicly.
3. ListingCreationDate: The date when the loan listing was created and made available for investors.
4. CreditGrade: Represents the credit rating assigned at the time the listing went live, applicable to listings from the pre-2009 period.
5. Term: Indicates the length of the loan in months.
6. LoanStatus: Describes the current status of the loan, such as Cancelled, Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, or PastDue.
7. ClosedDate: Applicable for specific loan statuses like Cancelled, Completed, Chargedoff, and Defaulted, indicating the date when the loan was closed.
8. BorrowerAPR: The Annual Percentage Rate (APR) for the loan, representing the borrower's interest rate.
9. BorrowerRate: The actual interest rate assigned to the borrower for the loan.
10. LenderYield: The yield received by lenders on the loan, calculated as the interest rate minus the servicing fee.
11. EstimatedEffectiveYield: An estimation of the effective yield on the loan, factoring in various components like interest rate, servicing fee, and late fees for loans originated after July 2009.
12. EstimatedLoss: The estimated principal loss on charge-offs for loans originated after July 2009.
13. EstimatedReturn: The estimated return assigned to the listing at the time of creation, calculated as the difference between the Estimated Effective Yield and the Estimated Loss Rate.
14. ProsperRating (numeric): A numeric representation of the Prosper Rating assigned to the listing at the time of creation, ranging from 0 (N/A) to 7 (AA) for loans originated after July 2009.
15. ProsperRating (Alpha): The Prosper Rating represented in alphabetic characters (AA to HR) for loans originated after July 2009.
16. ProsperScore: A custom risk score ranging from 1 to 10, with lower values indicating a better risk score, using historical Prosper data for loans originated after July 2009.
17. ListingCategory: The category chosen by the borrower when posting the loan listing, ranging from debt consolidation to various loan purposes like home improvement, personal loans, and more.
18. BorrowerState: The two-letter abbreviation of the state where the borrower resided when the listing was created.
19. Occupation: The occupation chosen by the borrower at the time of creating the listing.
20. EmploymentStatus: The employment status of the borrower when they posted the listing.
21. EmploymentStatusDuration: The duration in months of the borrower's employment status at the time of listing creation.
22. IsBorrowerHomeowner: Indicates whether the borrower is a homeowner or not, based on their credit profile or documentation provided.
23. CurrentlyInGroup: Specifies whether the borrower was associated with a group when the listing was created.
24. GroupKey: The unique key of the group to which the borrower belongs, with null values for borrowers not affiliated with any group.
25. DateCreditPulled: The date when the credit profile was pulled for loan evaluation.
26. CreditScoreRangeLower and CreditScoreRangeUpper: The lower and upper values representing the range of the borrower's

To view the complete exploratory analysis, Click [Here](http://localhost:8889/notebooks/Python%20Project%20-%20Prosper%20Loan%20Analysis.ipynb)

# Conclusion
In conclusion, the analysis of the Prosper Loan dataset reveals several key observations and insights:

1. Employment Status: The majority of borrowers are employed, with a significant portion engaged in full-time employment. However, there are also notable groups such as the self-employed, part-time workers and individuals in various other employment categories. The presence of a "Not available" category suggests missing or unreported employment status information while the "Not employed" category indicates individuals actively seeking employment.

2. Occupations: The dataset includes diverse occupations, with the largest category labeled as "Other." This suggests the presence of various occupations not explicitly listed. Additionally, there is a notable representation of professionals in fields such as computer programming, administration, teaching, sales, executive positions, electrical engineering and construction. This distribution provides an overview of the main occupational groups represented among the borrowers.

3. Loan Statuses: The loan statuses indicate the current state of loans in terms of repayment. The largest category is "Current," representing loans that are active and being repaid according to the agreed-upon terms. Other categories include "ChargeOff" for loans unlikely to be fully repaid, "Completed" for loans that have been successfully repaid and various stages of delinquency and default. This analysis helps understand the overall loan portfolio and identify potential areas of concern.

4. Borrower Rate and Lender's Yield: There is a positive correlation between borrower rates and lender's yields suggesting that higher interest rates result in higher yields for lenders. This relationship indicates a potential risk-reward tradeoff and highlights the role of the servicing fee in determining the lender's yield. The pricing strategy employed by Prosper Loan seems to adjust both the interest rate and servicing fee in combination.

5. Current Delinquencies and Borrower Rate: A weak positive correlation exists between current delinquencies and borrower rates. This suggests a potential connection between delinquency rates and the interest rates offered to borrowers, with higher delinquencies possibly leading to higher interest rates. However, the impact of current delinquencies on borrower rates appears to be limited compared to other factors such as creditworthiness and market conditions.

6. Credit Grades and Monthly Income: The box plot analysis of credit grades and monthly income indicates income levels associated with each credit grade. There are variations within certain credit grade categories but generally, lower credit grades tend to be associated with lower incomes while higher credit grades are associated with higher incomes. Some credit grades show consistent income levels while others exhibit variability and outliers.

Overall, these observations provide valuable insights into the composition of the borrowing population, their employment status, occupations, loan statuses, interest rates and income levels. They contribute to a better understanding of the Prosper Loan dataset and can inform further analysis and decision-making related to loan portfolio management, risk assessment and pricing strategies.
