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

## Tools & Technologies
    SQL — Data analysis, transformations, segmentation, and risk calculations
    SQLite — Database management and SQL execution
    Python — Data loading and processing using Pandas
    Power BI — Interactive dashboards and visualizations
    DAX — Measures and default-rate calculations
    Power Query — Data preparation and transformation
    GitHub — Project documentation and version control

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
 * Key Business Insights
   * Customer income: The Low Income segment had the highest observed historical default rate at 14.22%, compared with 8.52% for the High Income segment.
   * Loan purpose: Small Business loans showed an observed historical default rate of 18.55%, followed by Renewable Energy at 15.29% and Moving at 14.37%.
   * Loan grade: Grade G had the highest observed historical default rate among the reported grades at 37.48%, followed by Grade F at 34.67%.
   * Credit score: The Low FICO segment had an observed historical default rate of 16.98%, while the Excellent FICO segment had 3.20%.
   * Debt burden: The Very High DTI segment had an observed historical default rate of 15.26%, compared with 8.97% for the Low DTI segment.
   * Manual review: A project-defined risk-scoring framework flagged approximately 44,856 applications for additional review.

These findings describe historical patterns in the analyzed dataset. They do not establish causation or predict an individual borrower's future default.
### Business Recommendations
   * Based on the analysis:
     * Prioritize high-risk applications containing multiple risk indicators for manual review.
     * Monitor high-risk loan types such as Small Business and other categories with elevated historical default rates.
     * Monitor lower-income customer segments because they showed higher historical default rates in this portfolio.
     * Use multiple risk indicators together instead of relying on a single variable.
     * Monitor portfolio exposure, not only default rates, because a large loan category can represent significant financial exposure even when its default rate         is moderate.
     * Use the dashboard as a decision-support and risk-monitoring tool, not as an automated loan approval/rejection system.
    
 ## Dashboard Preview
  screen_short:-![Loan-Default-Risk-Dashboard](Screenshot 2026-10-07 115411.png)
  screen_short:-![Loan-Default-Risk-Dashboard](Screenshot 2026-10-07 115420.png)
  screen_short:-![Loan-Default-Risk-Dashboard](Screenshot 2026-10-07 115435.png)
)
