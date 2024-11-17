# Lending Club 
> Lending Club Project details: The consumer finance company which specialises in lending various types of loans to urban customers.
>
> Lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.
>
> The main objective to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
>
> Perform an analysis to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company want to utilise this knowledge for its portfolio and risk assessment.  


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Contributors](#contributors) 

<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Project Information
- This project is a data science project. It uses Lending Club data set to predict whether a loan will be defualted or not.
### Project Background
- This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures.
- Borrowers can easily access lower interest rate loans through a fast online interface.
- Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss).
- Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed.
- In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

### Business Problem to solve
- To identify about risky loan applicants, so that such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
  
### Project dataset
- The dataset is a csv file with name: loan.csv. It is added in the repo.


## Conclusions
## Detailed Analysis of Univariate and Bivariate

Univariate Analysis

##### 1. Defaulted vs Fully Paid Loans:

The number of defaulted loans is significantly lower, approximately 6 times less than the number of fully paid loans. This suggests that a larger portion of borrowers are successfully repaying their loans, while a smaller fraction defaults.

##### 2. Loan Term Duration:

The analysis reveals that the number of loans with a 36-month term is 3.5 times higher than those with a 60-month term. This indicates that borrowers tend to prefer loans with shorter durations, potentially due to quicker repayment goals and manageable monthly installments.

##### 3. Interest Rates on Loans:

The majority of loans were taken with interest rates between 5% to 7.5% and 10% to 15%. This suggests that borrowers are most comfortable with moderate to high-interest rates, likely due to the affordability and availability of loans within these interest rate ranges.

##### 4. Employment Length:

People with 10+ years of employment constitute the largest group of borrowers, indicating that individuals with longer employment histories tend to be more reliable borrowers, possibly due to their stability and financial capability to repay loans.

##### 5. Income Group of Borrowers:

The majority of loans are taken by individuals in the lower-income group (annual income between 20k to 90k). This shows that loans are largely accessed by people with moderate financial means, which could suggest that lending companies are targeting a broader range of individuals, including those with average incomes.

##### 6. Loan Grades:

Most loans belong to Grade A and B categories, indicating that borrowers who are considered lower-risk (according to their credit grades) are more likely to take out loans.

##### 7. Home Ownership:

A significant portion of borrowers either rent or are mortgaged and do not own their homes. This suggests that individuals without property ownership are taking out loans, likely for personal or financial needs, rather than for homeownership.

##### 8. Verification Status:

More than 50% of loans are verified by the lending company or are classified as Source Verified. This indicates that the lending company ensures that the majority of loans are checked for credibility before disbursement.

##### 9. Loan Purpose:

Most loans are taken for either credit card repayment or debt consolidation. This suggests that borrowers are seeking loans primarily to manage existing debts or improve their credit situation.

##### 10. Public Records:

A majority of borrowers have no public records indicating bankruptcy or derogatory marks, implying that most loan applicants have a clean financial background, which is a positive sign for lenders.

##### 11. Debt-to-Income Ratio (DTI):

A significant portion of borrowers have a high DTI ratio ranging between 8% to 22%, indicating that many individuals are taking on more debt compared to their income. This could potentially be a red flag, as a high DTI ratio can indicate financial strain.

##### 12. Loan Trends over Time:

Loan disbursements show a tendency to increase towards the end of the year, with a progressive rise in loan counts every month, as compared to previous months. This suggests a seasonal increase in loan activity, possibly driven by year-end financial needs or holiday spending.

##### 13. Annual Loan Growth:

Loan approvals appear to be growing at an exponential rate, with year-over-year growth in the number of loans approved. This indicates that the lending company is approving more loans each year, likely due to increased demand or expanded lending operations.

# Bivariate Analysis

##### 1. Income Group and Loan Default:

Borrowers with an annual income of 50k or less are more likely to default compared to higher-income groups. This suggests that income is a strong predictor of loan repayment ability, with lower-income individuals facing greater financial strain.

##### 2. Interest Rate and Default Probability:

As the interest rate increases, the default ratio also rises. Higher interest rates may indicate that borrowers are struggling to meet loan obligations, which could lead to an increased risk of default.

##### 3. Employment Length and Loan Default:

Borrowers with 10+ years of employment are less likely to default and have a higher chance of fully repaying their loans. This finding highlights the importance of stable employment in ensuring loan repayment.

##### 4. Loan Grade and Default Rate:

Loans with a higher Grade A (and corresponding Sub Grade A categories) exhibit a higher risk of default, whereas Grade G (and its Sub Grades) demonstrate a lower default rate. This may indicate that the credit scoring model used to classify loans might show unexpected trends, with higher-grade loans having higher default rates.

##### 5. Loan Amount and Default Probability:

The probability of a loan being charged off increases with the loan amount, particularly for amounts above 50% of the loan range. This suggests that larger loans, especially those in the range of 25k and above, are at higher risk of default.

##### 6. Home Ownership and Loan Default:

Individuals who don’t own a home and are renting or mortgaged tend to have a higher chance of defaulting, particularly with smaller loan amounts (around 10k or less). Banks should be cautious when issuing loans to such individuals.

# Driving Factors for Loan Default Prediction
Key factors that can be used to predict the likelihood of loan default include:

1. Income Group – Lower-income groups are more likely to default.
2. Interest Rate – Higher interest rates increase the probability of default.
3. Sub-grade – Higher sub grades have a higher default rate.
4. Home Ownership – Renters and mortgaged individuals have a higher chance of default.
5. Debt-to-Income (DTI) Ratio – A higher DTI ratio is linked with a higher likelihood of default.

# Summary
The analysis indicates that loan defaults are influenced by multiple factors, including income level, credit grade, loan purpose, interest rate, employment length, loan term, and verification status. Loan defaults are more prevalent among applicants with lower-to-moderate incomes, high DTI ratios, moderate interest rates, and specific credit grades (e.g., B, F, G). These findings can inform risk assessment and targeted lending policies to mitigate default risks.

## Technologies Used
- Numpy - version '2.0.2'
- Pandas - version '2.2.2'
- Seaborn - version '0.13.2'
- Matplotlib - version '3.9.2'

## Acknowledgements
- This project was inspired by UpGrad(IIITB) in AI/ML Executive Post Graduate course as a case study
- This project was based on (https://learn.upgrad.com/course/5811/segment/53276/316332/957998/4783501).

## Contact
Created by [@androidev1] -- feel free to contact us!

## Contributors
- Ashish Kumar Agrawal
- Abhishek Sharma
