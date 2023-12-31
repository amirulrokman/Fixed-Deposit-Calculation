Fixed Deposits Aging Analysis 📊💰

As a trainee, my task was to streamline the reporting process for Bank Negara by automating the generation of weekly and monthly reports, which were previously handled manually using Excel. While I cannot provide specific code due to confidentiality, I can elaborate on the overall workflow involved.

Overview
The SQL script is designed to categorize fixed deposits into aging buckets based on their maturity dates relative to a reporting date. It then calculates the total principal and product for each aging bucket and determines the weekly interest rates for deposits older than 1 month.

SQL Query Steps
Step 1: Get the Current Date
sql

DECLARE @reporting_date DATE
SET @reporting_date = GETDATE()

Step 2: Categorize Fixed Deposits into Aging Buckets
A Common Table Expression (CTE) is used to classify fixed deposits into aging buckets based on the difference between their maturity dates and the reporting date.

Step 3: Determine Maximum Value Dates for Each Aging Bucket
Another CTE is employed to find the maximum value date for each aging bucket.

Step 4: Calculate Total Principal and Product
This CTE calculates the total principal and product for each aging bucket and value date.

Step 5: Calculate Weekly Interest Rates
The final query calculates weekly interest rates for aging buckets older than 1 month.

Fun Elements 🎉
📅 Automated reporting date usage.
🔄 Iterative aging bucket categorization.
💰 Calculation of weekly interest rates for older deposits.


