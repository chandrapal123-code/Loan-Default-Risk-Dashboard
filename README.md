# Loan-Default-Risk-Dashboard
SQL + Power BI credit-risk analytics project identifying high-risk customer segments and loan types and prioritizing loan applications for manual review using historical default patterns.
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

### Data Preparation
  * The selected loan fields were loaded into SQLite using Python and Pandas.
  * The project first created a raw table:

        loans_raw

* Data quality checks were performed for:
   * Missing values
   * Duplicate loan IDs
   * Loan status distribution
   * Missing risk variables
   * Invalid or incomplete records

## Portfolio Analysis
 
    The dashboard provides portfolio-level KPIs:
    Total Loans
    Total number of loan applications.
    Total Loan Amount
    Total amount of loans in the portfolio.
    Defaulted Loans
    Number of loans classified as historically defaulted.
    Observed Historical Default Rate
                    Defaulted Loans
                    ---------------- × 100
                    Total Loans
    Average Loan Amount
    Average amount per loan.
    Average Interest Rate
    Average interest rate across the portfolio.
    
## Key Business Insights
 * 1. Customer Segment Risk
      * Low-income borrowers had the highest observed historical default rate at 14.22%.
 * 2. Loan Type Risk
      * Small Business loans had an observed historical default rate of 18.55%, making them one of the higher-risk loan categories in the analysis.
 * 3. Grade Risk
      * Grades E, F and G had substantially higher historical default rates than lower-risk grades.
 * 4. Credit Score Risk
      * Lower FICO segments had higher historical default rates.
 * 5. Debt Burden
      * Very-high DTI loans had a 15.26% historical default rate.
 * 6. Interest Rate Risk
      * Loans with interest rates of 20%+ had a 24.07% historical default rate.
 * 7. Manual Review
      * Approximately 44,856 applications were identified for manual review using the project-defined risk-screening framework.
