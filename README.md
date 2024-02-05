# An analysis of Superstore Sales Performance

### Project Overview

This data analysis project aims to provide insights into the sales performance of Superstore over the past year. By analysing various aspect of the sales data, we seek to indentify weak areas and opportunities for Superstore to boost business growth.

### Data Sources

Sales Data: The primary data set used for this analysis is the "aqilah humaira capstone project.xlsb", containing detailed information about each sales made by the company.

### Tools

- Excel - Data Cleaning
- SQL server - Data Manipulation
- Tableau - Data Visualization
  - [Tableau Public](https://public.tableau.com/app/profile/aqilah.humaira.saiful.bahri8272/viz/AqilahHumairaCapstoneProject/SuperstoreSalesPerformance?publish=yes)

### Data Cleaning/Preparation

In the initial phase of data preparation, we performed the following task:

1. Remove blanks.
2. Identified missing values using filtering options
3. Remove duplicates
4. Correct Data errors in Customer_ID Column and other typos, incorrect formats, or inconsistencies. 
5. Ensure data consistency by standardizing formats (e.g., date formats), units, and categories.
6. Transform data to suit the analysis using PivotTables' data filtering and sorting.
7. Created new columns or variables such as order year, order month, days to ship.
8. Make sure data is accurate. Used summary statistics, charts, or data visualization to validate results.
9. Saved and performed data analysis.


### Exploratory Data Analysis

- Is there consistent sales growth, and what factors contribute to it?
- Are there any noticeable seasonality patterns in sales?
- What are the top-selling product categories and sub-categories?
- Are there any geographical patterns in the sales data?
- Which customer segment contributed to the highest sales?
- Are there any patterns in shipping modes across different regions
- Are there any products with consistently low sales that may need attention?
- Which state has the highest number of sales?


### Data Analysis

```sql
SELECT ship_mode,
COUNT (*) order_per_ship_mode
FROM orders
GROUP BY 1;
```

### Results/Findings

The analysis results are summarized as follows:
1. Sales increased consistently over the year due to business growth
2. Total sales seems to spike in 4th Quarter of each year during certain seasons or holidays
3. Technology is consistently the highest selling category over the year
4. Sales is the highest in West region due to population density or economic factors
5. Consumer segment is responsible for the majority of sales growth
6. Standard class is the most preferred shipping mode
7. Chairs and Phones are consistent top-selling products while Fasteners, Labels, Art and Envelopes show consistently low sales over the year
8. The state with the highest number of sales is California

### Recommendations

Based on the analysis, we recommed the following actions:
- Capitalize on 4th Quarter sales spikes with targeted marketing and promotions aligned with specific holidays or events to maximize impact.
- Invest further in the successful Technology category by introducing new products, enhancing existing ones, and optimizing marketing strategies to maintain and expand market share.
- Tailor product offerings, promotions, and marketing strategies to meet the preferences of the Consumer segment, driving the majority of sales growth.
- Allocate additional resources and marketing efforts to the West region, understanding the factors behind its high sales. Apply insights to replicate success in other regions.
- Tailor product offerings, promotions, and marketing strategies to meet the preferences of the Consumer segment, driving the majority of sales growth.
- Streamline the Standard shipping mode to enhance customer satisfaction. Explore improvements in delivery times, cost-effective packaging, and loyalty programs tied to standard shipping.
- Evaluate the performance of product categories. Consider reallocating resources from consistently low-selling products (Fasteners, Labels, Art, Envelopes) to focus on high-performing ones like Chairs and Phones.
- Explore opportunities for expansion in California, the highest sales region. Consider opening new stores, intensifying marketing efforts, and strengthening partnerships to maximize market potential.

### Limitations

I had to remove all blanks values because they would have affected the accuracy of my conclusions from the analysis. 
