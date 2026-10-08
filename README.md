# Loan-Default-Risk-Dashboard
The Loan Default Risk Dashboard is an end-to-end SQL and Power BI analytics project designed to help a lending/credit team understand historical loan default patterns, identify high-risk customer segments and loan types, and prioritize loan applications for manual review.

### Project Overview
  * The Loan Default Risk Dashboard is an end-to-end SQL and Power BI analytics project designed to help a lending/credit team understand historical loan default         patterns, identify high-risk customer segments and loan types, and prioritize loan applications for manual review.
 * The project uses historical Lending Club loan data and focuses on descriptive and diagnostic analytics, not machine learning or predictive modeling.
### Business Question
* Which customer segments and loan types have the highest observed historical default rates, and which loan applications should the credit team prioritize for manual review?
* The credit team needs to understand:
    * Which customer segments have higher historical default rates?
    * Which loan types have higher historical default rates?
    * Which borrower characteristics are associated with higher historical defaults?
    * Where is the portfolio's lending exposure concentrated?
    * Which individual applications contain multiple high-risk characteristics?
    * Which applications should receive additional manual review?

* This project converts the raw loan data into a structured risk-analysis solution and an interactive Power BI dashboard.
### Project Objectives
   * Analyze overall loan portfolio risk and default performance.
   * Identify high-risk customer segments based on income, FICO, DTI, employment, and home ownership.
   * Compare historical default rates across different loan purposes.
   * Identify key factors associated with higher historical default rates.
   * Create a transparent risk-scoring framework to prioritize applications for manual review.
   * Build an interactive Power BI dashboard to support credit-risk decision-making.

### Dataset
The project uses the Lending Club accepted loan dataset covering 2007–2018.
The original dataset contains loan-level information about borrowers, loan characteristics and repayment outcomes.

* Main fields used
        id
        loan_amnt
        term
        int_rate
        grade
        sub_grade
        emp_length
        home_ownership
        annual_inc
        verification_status
        issue_d
        loan_status
        purpose
        addr_state
        dti
        delinq_2yrs
        fico_range_low
        fico_range_high
        inq_last_6mths
        revol_util
        total_acc
        application_type
