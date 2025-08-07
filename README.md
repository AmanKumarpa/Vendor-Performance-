# Vendor-Performance-
### Exploratory Data Analysis
![Summary](https://img.shields.io/badge/status-Statistics-red?style=for-the-badge)
<br>
- Previously, we examined the various tables in the database to identify key variables,understand their relationships,and determine which ones should be included in the final analysis.</br>
- In this phase of EDA, we will analyze the resultant table to gain insights into the distribution of each column. This will help us understand data patterns,identify anomalies, and ensure data quality before proceeding with further analysis.</br>
<img width="1196" height="686" alt="Screenshot 2025-08-07 145912" src="https://github.com/user-attachments/assets/7f2017c1-5e53-4bf6-8f86-592dcf9424ee" />
<img width="15000" height="10000" alt="aman" src="https://github.com/user-attachments/assets/cc21ae8b-33b9-48a6-a447-da6fe72bf8b5" />


### Negative & Zero Values:

- **Gross Profit:** Minimum value is -52,002.78, indicating losses. Some products or transactions may be selling at a loss due to high costs or selling at discounts lower than the purchase price. </br>

- **Profit Margin:** Has a minimum of -∞, which suggests cases where revenue is zero or even lower than costs.</br>

- **Total Sales Quantity & Sales Dollars:** Minimum values are 0, meaning some products were purchased but never sold. These could be slow-moving or obsolete stock.

###  Outliers Indicated by High Standard Deviations:

- **Purchase & Actual Prices:** The max values (5,681.81 & 7,499.99) are significantly higher than the mean (24.39 & 35.64), indicating potential premium products.</br>

- **Freight Cost:** Huge variation, from 0.09 to 257,032.07, suggests logistics inefficiencies or bulk shipments.</br>

- **Stock Turnover:** Ranges from 0 to 274.5, implying some products sell extremely fast while others remain in stock indefinitely. Value more than 1 indicates that sold quantity for that product is higher than purchased quantity due to either sales are being fulfilled from older stock.

![Data](https://img.shields.io/badge/status-Filtering-red?style=for-the-badge)

  - **Gross Profit ≤ 0**  (to exclude transactions leading to losses)
  - **Profit Margin ≤ 0**  (to ensure analysis focuses on profitable transactions)
  - **Total Sales Quantity = 0**  (to eliminate inventory that was never sold)
    
### Correlation Insights
<img width="12000" height="8000" alt="aman2" src="https://github.com/user-attachments/assets/3475d999-d6ed-4152-ab67-225108e98477" />



**Purchase Price vs. Total Sales Dollars & Gross Profit:** Weak correlation (-0.012* and -0.016), indicating that price variations do not significantly impact sales revenue or profit.

**Total Purchase Quantity vs. Total Sales Quantity:** Strong correlation (0.999), confirming efficient inventory turnover.

**Profit Margin vs. Total Sales Price:** Negative correlation (-0.179), suggesting increasing sales prices may lead to reduced margins, possibly due to competitive pricing pressures.

**Stock Turnover vs. Gross Profit & Profit Margin:** Weak negative correlation (-0.038 and -0.055), indicating that faster stock turnover does not necessarily equate to higher profitability.

**Purchase Price vs. Total Sales Dollars & Gross Profit:** Weak correlation (-0.012* and -0.016), indicating that price variations do not significantly impact sales revenue or profit.

**Total Purchase Quantity vs. Total Sales Quantity:** Strong correlation (0.999), confirming efficient inventory turnover.

**Profit Margin vs. Total Sales Price:** Negative correlation (-0.179), suggesting increasing sales prices may lead to reduced margins, possibly due to competitive pricing pressures.

![Research](https://img.shields.io/badge/Research-Question-red?style=for-the-badge)

##  1.Brands for Promotional or Pricing Adjustments
Brands with Low Sales but High Profit Margins:
<img width="855" height="464" alt="Screenshot 2025-08-07 152756" src="https://github.com/user-attachments/assets/058bebae-cb23-4fd3-a536-7dc13ce190c5" />

198 brands exhibit lower sales but higher profit margins, which could benefit from targeted marketing, promotions, or price optimizations to increase volume without compromising profitability.

<img width="10000" height="6000" alt="aman3" src="https://github.com/user-attachments/assets/3b07e2e7-1e3f-452c-8a71-6a7fcd4a99f7" />

##  2.Top Vendors by Sales & Purchase Contribution

-  According to industry benchmarks, the top 10 suppliers often contribute between 60% and 70% of the total value of goods and services purchased. This aligns with your case study numbers, where top vendors contribute about 65.69% of total purchases and the remaining vendors 34.31%.
-  This high concentration indicates potential supply chain risks, as over-reliance on just a few vendors can make a business vulnerable to disruptions. It suggests a need for supplier diversification and periodic vendor performance reviews to optimize cost, quality, and reliability
  
<img width="8000" height="8000" alt="aman4" src="https://github.com/user-attachments/assets/30d87df9-6f64-4397-a799-879932954485" />

##  3. Impact of Bulk Purchasing on Cost Savings
-  Vendors buying in large quantities receive a 72% lower unit cost ($10.78 per unit vs. higher unit costs in smaller orders).
-  Bulk pricing strategies encourage larger orders, increasing total sales while maintaining profitability

  <img width="317" height="187" alt="Screenshot 2025-08-07 153416" src="https://github.com/user-attachments/assets/90cb1fd1-3e5a-4cb0-bf03-5fdc5497eaff" />
  
##  4.Identifying Vendors with Low Inventory Turnover

- Unsold Inventory Capital:**$3.71M**
  
- Slow-moving inventory increases storage costs, reduces cash flow efficiency, and affects overall profitability.

- Identifying Vendors with Low Inventory Turnover: Enables better stock management, minimizing financial strain.

<img width="432" height="489" alt="Screenshot 2025-08-07 164848" src="https://github.com/user-attachments/assets/9b6352c9-2757-4edf-bd30-9fbac643d96b" />
  
<img width="492" height="414" alt="Screenshot 2025-08-07 154737" src="https://github.com/user-attachments/assets/5472c440-a69e-48c7-bee9-030bff07f3e8" />



### ![Final](https://img.shields.io/badge/Final-Recommendations-red?style=for-the-badge)

-  Re-evaluate pricing for low-sales, high-margins brands to boost sales volume without sacrificing profitability.
   
-  Diversify vendor partnerships to reduce dependency on a few suppliers and mitigate supply chain risks.
  
-  Leverage bulk purchasing advantages to maintain competitive pricing while optimizing inventory management.

-  Optimize slow-moving inventory by adjusting purchase quantities, launching clearance sales, or revising storage strategies.

-  Enhance marketing and distribution strategies for low-performing vendors to drive higher sales volumes without compromising profit margins.

-  By implementing these recommendations, the company can achieve sustainable profitability, mitigate risks, and enhance overall operational efficiency.








