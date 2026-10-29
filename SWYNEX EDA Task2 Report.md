# SWYNEX Technologies — Task 2: Exploratory Data Analysis

## Objective
Explore the cleaned Task 1 dataset to summarize amount patterns, compare countries/cities, review monthly trends, and check for unusual amount values.

## Dataset overview
- Records analyzed: 120
- Fields: Name, Email, City, Country, Date, Amount
- Date coverage: 01 Sep 2025 to 25 Jun 2026
- Countries: 9
- Cities: 12
- Data note: email addresses use the example.com domain, so results are descriptive of the provided sample dataset and should not be treated as real customer/business performance.

## Key statistics
- Total Amount: **13,613.31**
- Mean Amount: **113.44**
- Median Amount: **116.12**
- Minimum Amount: **9.11**
- Maximum Amount: **238.94**
- Standard deviation: **63.98**
- IQR boundaries: **-87.18** to **303.87**
- IQR-flagged outliers: **0**

## Key insights
1. Dataset coverage: The cleaned dataset contains 120 records across 9 countries and 12 cities, dated 01 Sep 2025 to 25 Jun 2026.
2. Overall amount: Total Amount is 13,613.31; the average record is 113.44 and the median is 116.12. The mean is slightly below/above the median by 2.68 (below), so these two measures are fairly close.
3. Country contribution: United Kingdom has the largest total (3,638.84) from 31 records, contributing 26.7% of the dataset total.
4. Monthly pattern: 2025-09 has the highest monthly total (2,204.43, 17 records), while 2026-02 has the lowest monthly total (694.76, 8 records).
5. Record volume by month: 2025-09 has the most records (17); 2026-02 has the fewest (8). Monthly totals should be interpreted alongside record counts.
6. City patterns: Manchester appears most often (19 records). Tampere has the highest average amount (149.44), while Berlin has the lowest (52.62); average amount and record volume are different measures.
7. Outlier check: Using the 1.5×IQR rule, the lower boundary is -87.18 and the upper boundary is 303.87. 0 records fall outside these boundaries, so no amount outliers are flagged by this rule.

## Visualizations included
1. Total Amount by Country (bar chart)
2. Monthly Total Amount (line chart)

The Excel workbook also contains country, month, and city summary tables and an outlier-check sheet.

## Method
- Used pandas to calculate descriptive statistics and aggregate Amount by country, city, and month.
- Used the 1.5×IQR rule to flag potential Amount outliers.
- Compared monthly totals alongside record counts to avoid interpreting totals without considering volume.

## Conclusion
The dataset shows differences in total and average amounts across countries, cities, and months. The United Kingdom contributes the highest total amount in this sample, while monthly totals vary across the observed period. The IQR check does not flag any amount outliers. Because the data is a small sample with example.com emails and no currency field, conclusions are descriptive only; no currency or real-world business meaning has been assumed.
