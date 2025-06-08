## Dataset Source

The original Excel file used in this analysis is based on the [Credit Card Customers dataset from Kaggle](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers/data).
I have added several columns and sheets to the workbook, including derived features such as status labels and lookup-based classifications, to support deeper analysis and visualization.

## BankChurners Excel Analysis

This project analyzes credit card customer attrition patterns using Excel. It focuses on identifying high-risk customer segments and uncovering trends using pivot tables, charts, and formulas.
**Note:** Figures and formulas used for analysis are located in the `READ_ME_Formulas_Charts` sheet of the Excel file.

## Tools Used
- Microsoft Excel
- Pivot Tables/Charts
- XLOOKUP & VLOOKUP
- Logical & conditional functions


## Key Features
- Attrition rate calculations by demographic
- Custom XLOOKUP-based status labels
- Visualizations comparing attrited vs. existing customers
- Structured summary insights to drive retention focus

## Files Included
- BankChurners_Analysis.xlsx: Main workbook with insights, charts, and data cleaning
- README.md: Project summary and insights


## Questions/Insight Summary
1. Which types of customers, based on their gender and marital status, are most likely to close out their accounts? (Excluding UNKNOWNS)

I used logical and conditional functions to create a chart to break down the count of attrited/existing accounts based on gender and marital status. Based on this chart, we can analyze that married
female customers have the highest attrition rates, making that group the prime focus group for the bank to retain in the future. Furthermore, there are more females who are married utilizing
this bank than any other group, reinforcing the important of targeting this group for retention.

2. What was the average of total transactions amount like for Attrited vs Existing? Is there a highest income area for attrited?(Figure 1)

I created a pivot table and a clustered column chart to visualize the average total transaction amount(last 12 months) vs income for attrited customers vs existing customers. Throughout all income groups, customers who have attrited their accounts had significantly less average total transactions amount when comepare to existing customers. Using this information, banks could potentially send incentives for existing customers who are below the average total transactions amount of their income group to maintain the retention rates. Banks could also notice existing customers who are getting closer to the average total transactions amount of attrited customers and send surveys in order to see how they could better serve their customers.

3. Which education levels have higher attrited rates? Are more educated or less educated customers more likely to be attrited? (Figure 2, Excluding UNKNOWNS)

I created a pivot table and a 100% stacked column chart to visualize the education level vs %of attrited customers for attrited customers vs existing customers. Interestingly, customers holding a doctorate-level education exhibit the highest attrition rate among all education levels. Banks could use this data and information to reach out to doctorate level customers who choose to close out their accounts to find out why.

4.  Are customers with certain number of dependents more likely to be attrited?(Figure 3)

I created a pivot table and a 100% stacked column chart to visualize the number of dependents vs %of attrited customers for attrited customers vs existing customers. Altough difference was minimal, customers who only had 0 or 1 dependents did have the lowest rates to close out their accounts while customers who had 3 dependents had the highest rates to close out their accounts. While further testing and analysis is needed for causation, looking at this strictly from a focus group persepective, banks could reach out to customers with larger families to see if there is anything they can do to help maintain their accounts with the bank.

5. Is a customer more likely to attrit their account based on their gender?(Figure 4)

I created a pivot table and a 100% stacked column chart to visualize gender vs %of attrited customers for attrited customers vs existing customers. Based on this chart, we can analyze that females have a higher rate to close their accounts as opposed to males. This could further support our analysis in #1 where females who are married have the highest attrition rates. 

6. Based on the XLOOKUP formula used in Total_Revolving_Bal_Status, how many customers would receive a NEEDS PAYMENT notice in their mail if they were sent out today?

I created a Sample_Table_XLOOKUP sheet where we can categorize each customer as NO PAYMENT NEEDED or NEEDS PAYMENT based on their Total_Revolving_Bal_Status. I then added a column next to Total_Revolving_Bal_Status so that each row of customers can be associated with their respective XLOOKUP chart. Finally, counting the number of customers with NEEDS PAYMENT status, there would be 7657 mails being sent out to customers at the time of this data snapshot.

7. Based on the VLOOKUP formula used in Avg_Utilization_Ratio_Status column, how many customers are in each category?

Similarly, I create a Sample_Table_VLOOKUP sheet where we can categorize each customer as Very Poor, Poor, Fair, Good, or Excellent based on their Avg_Utilization_Ratio. I then added a column next to Avg_Utilization_Ratio so that each row of customers can be associated with their respective VLOOKUP chart. Finally, I created a chart to count the number of customers in each category of Avg_Utilization_Ratio_Status and added a pie chart to show a better visualization of each category as a percentage and frequency. Based on this analysis 51% of customers in this bank have a very low utilization ratio on their credit card on average. Meanwhile, 10% of the customers in this bank have a very high utilization ratio on their credit card on average.
