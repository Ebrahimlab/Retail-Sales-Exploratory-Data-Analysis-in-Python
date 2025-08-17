# Retail-Sales-Exploratory-Data-Analysis-in-Python

This project analyzes a fictional but realistic retail sales dataset to uncover customer purchasing patterns, category preferences, and seasonal spending trends.
The dataset includes:
**Transaction ID, Date, Customer ID, Gender, Age, Product Category, Quantity, Price per Unit, Total Amount**

Although the data is synthetic, the analysis methods and insights are directly applicable to real-world retail data, helping businesses optimize marketing, inventory, and customer engagement strategies.


**Business Questions Addressed**
1. **Customer Demographics & Spending** — How does age and gender influence total purchase amounts?
2. **Product Category Preferences** — Which category is most purchased by each age-gender group?
3. **Time-Based Spending Trends** — How do sales vary by day and month across product categories, customer counts, and gender?


**Dataset Overview**:
- **Rows**: 1,000
- **Columns**: 9
- **Unique Transactions**: 1,000
- **Unique Customers**: 1,000
- **Unique Dates**: 345 (multiple customers purchased on the same dates)
- **Categories**: Beauty, Clothing, Electronics
- **Missing Values**: None


**Data Preparation**
- Converted Date to datetime format
- Verified column uniqueness
- Confirmed no missing values



# Analysis 1 — Spending by Age & Gender
Grouped data by **Age** and **Gender** to calculate total spending.

**Example Pattern**:

- Females aged 18 spent more than males of the same age
- Males aged 22 outspent females significantly

**Visualization**:
("C:\Users\mebrh\OneDrive\Desktop\Retail-Sales-EDA-in-Python-main\Barplot of Total Spending by Age and Gender.png" )




# Analysis 2 — Top Product Category by Age & Gender
Examined **category-level spending** for each demographic segment.

**Key Findings**:

- Younger shoppers (18–25) prefer Beauty & Clothing
- Older demographics lean towards Electronics
- Males dominate Electronics spending, females lead in Beauty purchases

The table shows from **Age 18 - Age 25**, and **Age 56 - Age 64*. See the **FULL** output.

| Age | Product Category | Female | Male |
|---|---|---|---|
| 18 | Beauty            | 3195.0 | 1765.0 |
|   | Clothing          | 2575.0 | 1510.0 |
|   | Electronics       | 2170.0 | NaN |
| 19 | Beauty            | 2225.0 | 2140.0 |
|   | Clothing          | 1200.0 | 1530.0 |
|   | Electronics       | 3910.0 | 3865.0 |
| 20 | Beauty             | 365.0 | 2160.0 |
|   | Clothing            | 80.0  | 360.0 |
|   | Electronics       | 4730.0 | 950.0 |
| 21 | Beauty            | 3300.0 | 4700.0 |
|   | Clothing          | 1200.0 | 1885.0 |
|   | Electronics        | 900.0  | 600.0 |
| 22 | Beauty            | 1300.0 | 4230.0 |
|   | Clothing          | 3275.0 | 2075.0 |
|   | Electronics        | 850.0  | 1970.0 |
| 23 | Beauty             | 475.0  | 165.0  |
|   | Clothing          | 1270.0 | 3050.0 |
|   | Electronics       | 1150.0 | 2110.0 |
| 24 | Beauty            | 1575.0 | 1310.0 |
|   | Clothing            | 25.0   | 2125.0 |
|   | Electronics        | 150.0  | 230.0  |
| 25 | Beauty            | 1000.0 | 1375.0 |
|   | Clothing          | 2200.0 | 2150.0 |
|   | Electronics        | 350.0  | 2825.0 |
| 56 | Beauty            | 1635.0 | 500.0 |
|   | Clothing          | 1790.0 | 2100.0 |
|   | Electronics       | 2600.0 | 815.0 |
| 57 | Beauty             | 425.0  | 3200.0 |
|   | Clothing          | 2895.0 | 750.0 |
|   | Electronics        | 310.0  | 1710.0 |
| 58 | Beauty            | 2800.0 | 990.0 |
|   | Clothing           | 760.0  | 1525.0 |
|   | Electronics        | 120.0  | 1200.0 |
| 59 | Beauty            | 2700.0 | NaN     |
|   | Clothing           | 525.0  | 3585.0 |
|   | Electronics        | 560.0  | 2100.0 |
| 60 | Beauty             | 490.0  | 80.0  |
|   | Clothing          | 3250.0 | 750.0 |
|   | Electronics       | 3920.0 | 3100.0 |
| 61 | Beauty               | NaN  | 1340.0 |
|   | Clothing          | 2240.0 | 250.0 |
|   | Electronics        | 600.0  | 2300.0 |
| 62 | Beauty             | 920.0  | 305.0 |
|   | Clothing           | 440.0  | 175.0 |
|   | Electronics       | 1700.0 | 4580.0 |
| 63 | Beauty             | 105.0  | 50.0  |
|   | Clothing           | 150.0  | 2320.0 |
|   | Electronics        | 950.0  | 5675.0 |
| 64 | Beauty             | 640.0  | 1690.0 |
|   | Clothing          | 4735.0 | 820.0 |
|   | Electronics        | 950.0  | 290.0 |


# Insights from Analysis 2


Analysis 2 helps to identify **Trends in Customer Spending behaviour** based on `Age`, `Gender`, and `Product Category`

The insights:

* Age Preferences: Spending habits change with Age for certain Product Categories
* Gender Differences: There are significant differences in spending patterns between Genders for specific Product Categories

For a larger Real-life dataset, using such analysis can help to refine the **Target Audience for Marketing Campaigns**. Specific Age groups and Genders have a higher propensity to spend on certain Product Categories




# Analysis 3 — Monthly Spending Patterns

Grouped transactions by month to assess seasonal and category-specific trends.

**Findings**:

1. **Spending Fluctuations**:
- Peak in May (53,150) — 42% above average
- Low in September (23,620) — seasonal dip
- Q4 surge (Oct–Dec) above 35K

2. **Category Shifts**:
- Electronics led in 8 of 12 months
- Beauty peaked in Jan & Jul
- Clothing dominated Feb–Apr

3. **Customer Traffic**:
- Highest: May (105 customers)
- Lowest: September (65 customers)

4. **Gender Trends**:
- Females outspent males in 7 months
- Males led during Electronics-heavy months

**Visualization**:

("C:\Users\mebrh\OneDrive\Desktop\Retail-Sales-EDA-in-Python-main\Lineplot of Total Monthly Spending Trend by Gender.png")




**Conclusion**
Three core findings:

1. **Gender-Driven Behavior** — clear category preferences by gender
2. **Age Influence** — younger buyers focus on Beauty/Clothing, older on Electronics
3. **Seasonality** — predictable peaks in May and Q4, dips in September



