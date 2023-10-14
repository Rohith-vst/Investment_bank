# Investment_bank
 Performed Exploratory Data Analysis (EDA) for a Investment Bank using NUMPY,PANDAS,MATPLOTLIB,SEABORN libraries with the main purpose to identity LOAN DEFAULTERS and concluded that there are more defaulters from debt consolidation,others,credit card and small business purpose loans from all grades.

Summary of Bivariate Observations:
Bivariate Analysis on Continuous Variables:
#Correlation Plot:

a) There were no highly negative correlation between numerical columns.

b) 0.45 correlation between term_months and interest rate(int_rate).

c) 0.47 correlation between revol_util and interest rate(int_rate).

d) No much correlation between Annual Income, DTI with other numerical columns.

#ROI vs Interest rates and Annual income:

a) There was a positive correlation between interest rates and ROI for borrowers who paid their loans, but for those who didn’t pay the ROI was negative and it shows no correlation with interest rates.
b) Borrowers with higher income has positive ROI while borrowers with lower income has negative ROI.

#Annual Income Vs Interest Rate by each grade:

By charts, it is evident that the interest rate range changes from one grade to other, and also there are few borrowers with near 6% falling in B,C,D and E grade's.

#Annual Income Vs DTI distribution by each grade:

By charts, it shows there is no DTI range constraint from one grade to other similar to interest rate which we have seen above.

Bivariate Analysis on Categorical Variables:
#ROI Bivariate Distribution plots:

1) ROI vs Grade by loan_status: From fully_paid loan, grades E,F,G have high mean ROI, this is because of high interest rates.

2) ROI vs Loan Purpose by loan_status: a) From fully_paid loans, almost all categories have nearby mean ROI. b) From Charged_off loan, small_business, other and medical have low mean ROI.

3) ROI vs Home Ownership by loan_status: From Charged_off loans, Rent and Mortgage have low mean ROI.

4) ROI vs Income Segment by loan_status: a) From fully_paid loans, ROI is bit high for upper middle and upper Income_segment. b) From Charged_off loan, ROI is very low for lower Income_segment.

#Interest Rate Bivariate Distribution Plots:

1) Interest Rate vs Term Months by loan_status: a) It is evident that 60 months term loans have more interest rate. b) There are more defaulters in both 36, 60 month terms because of high interest rates.

2) Interest Rate vs Income Segment by loan_status: a) By charts, it shows that, at every income segment, the defaulters are due to high interest rates.

#DTI Bivariate Distribution Plots:

1) DTI vs Income Segment by loan_status: a) DTI is less in lower segment, as the annual income is less and they might not have any loans and hence less DTI. If we have age details then we can predict more with borrower’s age, income and employment length. b) DTI is high in lower middle and middle segments. c) DTI is less in upper middle and upper segments, as the income is high they might have financial freedom. Note that there are some borrower’s in upper segment who have DTI more than 25.

Loan Defaulters Analysis:
1) Distribution of Loan Defaulters by Loan Purpose: a) There are more defaulters from 'debt_consolidation','other', 'credit_card' and 'small_business'. Let's check this at granular level by combining with Home Ownership and by each Grade.

2) Distribution of Loan Defaulters by Home Ownerships: a) By charts, it shows there are more defaulters in RENT and MORTGAGE.

3) Distribution of Loan Defaulters by Home Ownerships & Loan Purpose: a) There are more defaulters with 'debt_consolidation', 'credit_card' and 'small_business' purpose from Rent, Mortgage category and hence, should be carefull when borrowers don't have own house.

4) Distribution of Loan Defaulters by Grade: a) By charts, it shows there are more defaulters in B,C and D grades. b) Grades F,G(more intereste rate grades) are having less defaulters which is a good indicator.

5) Distribution of Loan Defaulters by Grade & Loan Purpose: By charts, from all grades, there are more defaulters from 'debt_consolidation', 'others', 'credit_card' and 'small_business' purpose loans.

Conclusion:
1) Number of loans issued increased steadily by every year with a slight decrease in 2008.

2) Of settled loans, 83% were Fully Paid and 14% were Charged Off.

3) Borrowers with own house and the purpose of loan with consolidate debt, 'credit_card' and 'small_business' are not at much risk, but borrower with rent,mortgage are high risk applicants.

4) Majority of loans were from A, B, and C grade.

5) There is an inverse relationship between interest rate and loan grade - lower grades(E,F,G) have higher interest rate.

6) From ROI analysis, it shows that borrowers with the best credit profiles or the lowest loan amounts will not end up being the most profitable and the borrowers who seemed to have worst credit indicators ended up being more profitable from E,F,G grades.

7) Overall, there are more defaulters from 'debt_consolidation', 'others', 'credit_card' and 'small_business' purpose loans from all grades.
