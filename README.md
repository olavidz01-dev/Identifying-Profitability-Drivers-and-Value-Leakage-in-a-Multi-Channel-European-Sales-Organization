# Identifying-Profitability-Drivers-and-Value-Leakage-in-a-Multi-Channel-European-Sales-Organization
<p align="center">
  <img src="assets/Overview.png" width="1000" />
</p>


---


## Business Overview
**Choco de Luxe** is a premium artisanal chocolate brand headquartered in Brussels, Belgium, specializing in high-quality chocolate bars, bites, and confections. The company operates across multiple European cities and distributes its products through a diversified mix of retail boutiques, online platforms, and supermarket partnerships. As Choco de Luxe continues to expand its product portfolio and geographic footprint, the brand focuses on preserving artisanal quality standards while driving market share growth. To support sustainable expansion, the company adapts its product offerings and sales strategies based on regional performance insights and evolving customer preferences across European markets.


---


## Business Problem 
Despite strong product quality and a growing presence across Europe, Choco de Luxe lacks a unified, data-driven understanding of its commercial and operational performance. 

The key challenges include:

  1. Revenue & Profit Visibility Gaps
  2. Regional Underperformance Masked by Averages
  3. Unclear Sales Channel ROI
  4. Sales Agent Performance Imbalance
  5. Delivery Performance Not Driving Sales or Profitability Outcomes
  6. Product Mix Diluting Profitability


---


## Project Objectives
The objective of this project is to deliver a comprehensive, data-driven assessment of Choco de Luxe’s commercial performance across Europe, enabling leadership to identify value leakage, optimize execution, and support profitable growth.

Specifically, the project aims to:

**1. Evaluate Sales & Profit Performance Holistically**

Analyze revenue, profit, and volume trends across time, regions, and channels to uncover seasonality, growth patterns, and periods of underperformance.

**2. Identify Regional & City-Level Performance Gaps**

Compare sales volume, profitability, and delivery success across European locations to pinpoint underperforming markets masked by strong overall operational performance.

**3. Assess Sales Channel Effectiveness & ROI**

Measure the relative contribution of Website, Warehouse, and Social Media channels to revenue, profit, and quantity sold, including the impact of organic versus inorganic sales.

**4. Analyze Sales Agent Productivity & Profitability**

Evaluate individual agent performance using revenue, profit, transaction volume, delivery success rate, and average revenue/profit per agent to identify top performers, underperformers, and value leakage.

**5. Examine Delivery Performance as a Commercial Enabler**

Assess whether delivery reliability drives or limits sales performance by linking delivery success rates to revenue and agent productivity across regions.

**6. Optimize Product Mix & Margin Contribution**

Analyze profitability across product categories and lines to distinguish high-margin, value-driving products from high-volume, low-margin items that dilute overall performance.

**7. Enable Executive Decision-Making Through Interactive Dashboards**

Develop intuitive, interactive Tableau dashboards that allow business leaders to dynamically explore performance drivers, drill into problem areas, and support strategic decisions on pricing, product mix, channel investment, and salesforce management.


---


## Data Dictionary and Modelling
The dataset contains four different tables with multiple columns. The tables include: Sales Fact Table, LocationDim Table, SalesPersonDim Table, and ProductDim Table. 

**Sales Fact Table**
- TransactionID: A unique identifier assigned to each sales transaction
- Date: The date when the transaction occurred
- SalesPersonID: identifies who made the sale
- LocationID: indicating where the sale was made
- ProductID: the identifier of chocolate product sold
- Boxes Shipped: The number of boxes of chocolate shipped for the transaction
- Sales Channel: The platform or medium through which the product was sold, e.g., website, In-store
- Delivery Status: The state of delivery for the order, e.g., completed, cancelled

**LocationDim Table**
- LocationID: Unique identifier for each location
- Country: Country where the sale took place.
- City: Specific city of the sale/distribution center
- Region: geographical area or grouping of the city

**SalesPersonDim Table**
- SalesPersonID: Unique identifier for each salesperson
- SalesPerson Name: Full name of the salesperson
- Email: The official company email of the salesperson.
- Hire_Date: The date the salesperson joined the company.

**ProductDim Table**
- ProductID: A unique identifier for each product
- Product Name: The name of the chocolate product (e.g., 85% Dark Bars, Caramel Stuffed Bars)
- Category: The classification of the product based on its type (e.g., Dark Chocolate, Milk Chocolate)
- Cocoa Percent (%): The percentage of cocoa content in the chocolate product
- Cost per unit: The internal cost to produce one unit (box) of the product
- Price Per box: The selling price per box of the product
- Is_Organic: Indicates whether the product is made with organic ingredients (Yes/No)
<p align="center">
  <img src="assets/dataMod.png" width="1000" />
</p>


---


## Approach & Methodology
This project was developed using **Microsoft Excel** and **Tableau**, covering the full analytics workflow from data cleaning and transformation to modeling, analysis, and visualization. The objective was to analyze Choco de Luxe’s sales performance across locations, sales channels, and product lines to identify performance patterns, operational inefficiencies, workforce and growth opportunities, and to deliver interactive Tableau dashboards that enable business leaders to make informed decisions on product positioning and channel strategy.

### 1. Data Cleaning & Transformation (Microsoft Excel)
- Imported raw customer data into **Excel**
- Performed data cleaning and transformation:
  - removed duplicates and filtered invalid or missing entries
  - renamed columns and standardized field formats (e.g., text, numeric, dates)
  - created **calculated columns** using VLOOKUP, XLOOKUP, IF, SUMIF, addition, subtraction, and multiplication   
- Ensured consistency and data quality for downstream modeling

### 2. DAX Measures (Tableau)
- Created **calculated fields** to support key metrics and business logic
- Applied dimensions and calculated measures to support dynamic and filter-aware analysis across sales, agents, and location segments

### 3. Interactive Visualization & Dashboard Design (Tableau)
Developed a comprehensive suite of interactive dashboards using **Tableau Dashboard**

### 4. Insight Generation & Business Alignment
- Identified key customer behavior patterns
- Translated findings into **actionable business recommendations**


---

## Live Dashboard
You can interact with the fully published Tableau dashboard here: 

🔗 [View on Tableau Public](https://public.tableau.com/shared/7XQCHSF6M?:display_count=n&:origin=viz_share_link)


---


## Sales Performance Analysis
<p align="center">
  <img src="assets/Saledash.png" width="1000" />
</p>

### 1. Top KPIs (Key Performance Indicators)
- Total Transaction: 1094
- Total Products: 21
- No of Locations: 7
- Quantity Sold: 177,007
- Total Unit Cost: €2,873,176
- Total Revenue: €5,320,696
- Total Profit: €2,447,520
- Profit Margin%: 46%
- Delivery Success Rate%: 96%

**KPI Insights**

**Choco de Luxe** demonstrates strong overall commercial health, generating €5.32M in revenue and €2.45M in profit, resulting in a healthy 46% profit margin. The business operates efficiently at scale, evidenced by a 96% delivery success rate across 7 European locations, 21 products, and 177K+ units sold.

However, beneath these strong topline metrics lie material performance imbalances across regions, sales channels, and product profitability, which, if addressed, present a significant opportunity to unlock incremental growth without materially increasing operational complexity.


### 2. Regional & City Level Performance

<p align="center">
  <img src="assets/Map.png" width="1000" />
</p>
<p align="center">
  <img src="assets/delivery%.png" width="1000" />
</p>

**Analysis**

- Sales volume is unevenly distributed across locations
- Certain countries significantly outperform others in quantity sold
- Delivery success is uniformly high (93%–100%) across regions, meaning logistics is not the constraint

**Insight**

Underperformance in certain countries is commercial, not operational. Strong delivery execution masks weaker local demand, pricing fit, or sales coverage.

**Implication**

Leadership should not interpret high delivery success as market success. Sales strategy must be localized, not uniformly applied across regions.


### 3. Revenue & Profit Trend Analysis

**Analysis**

- Choco de Luxe recorded its highest revenue and profit at the start of the year in January, generating €821,720 in revenue and €377,987 in profit.
- Performance declined sharply in February, with revenue falling to €539,678, before recovering steadily over the following months. Revenue peaked again in June at €796,260, after which it declined gradually, closing the analyzed period in August at €622,851.
- Profit trends broadly follow revenue, but profit growth does not scale proportionally with revenue in all months.
- January shows strong revenue but relatively lower profit, suggesting early-year margin pressure (discounting, promotions, or cost inefficiencies).

<p align="center">
  <img src="assets/Pro.Rev.png" width="1000" />
</p>

**Insight**

Choco de Luxe exhibits seasonality and campaign-driven volatility, indicating that pricing, promotions, or cost structures are not consistently optimized throughout the year.

**Implication**

There is an opportunity to:
- Smooth revenue volatility
- Improve margin consistency through better campaign timing and pricing discipline

### 4. Sales Channel Effectiveness

**Channel Performance Breakdown**

**1. Website**
- Strategic Role: Primary growth engine
- Insight: Highest revenue, profit, and quantity sold

**2. Warehouse**
- Strategic Role: Stable secondary channel
- Insight: moderate revenue, lower profit efficiency

**3. Social Media**
  - Strategic Role: Emerging/support  channel
- Insight: Lowest volume but strategic brand value

<p align="center">
  <img src="assets/Org.Inorg.png" width="1000" />
</p>
<p align="center">
  <img src="assets/Pro.Qtysold.png" width="1000" />
</p>

**Key Observations**
- The Website channel dominates both revenue and profit, accounting for the largest share of units sold both in organic and inorganic produce.
- Warehouse sales deliver volume, but at lower profit efficiency
- Social Media contributes limited revenue and profit, but shows potential as a demand-generation channel

**Insight**

Not all channels are equally value-accretive. The Website channel is the core profit engine, while others should be optimized for either cost efficiency or demand stimulation.


### 5. Product Mix & Profit Margin Contribution

**Key Observations**
- Profit margin contribution varies widely across product categories
- Premium and specialty products (e.g., caramel chocolate, dark chocolate, filled chocolates, and flavored chocolate variants) contribute disproportionately higher margins of approximately 5% and above.
- Some high-volume products dilute overall margin, contributing between 3.58% and 4.66%

**Insight**

Revenue growth is currently driven by volume, but profit growth is driven by product mix quality.

**Implication**

Without deliberate product mix optimization, scaling volume alone will not maximize profitability.

<p align="center">
  <img src="assets/proMar.png" width="1000" />
</p>


---


## Agent Performance Analysis
<p align="center">
  <img src="assets/Ag-dash.png" width="1000" />
</p>

**1. Top KPIs (Key Performance Indicators)**
- Total Transaction: 1094
- Qty Sold: 177,007 units across 21 products
- Sales Coverage: 25 agents across 7 locations
- Avg Revenue/Agent: €212, 827
- Avg Profit / Agent: €97,901
- Profit Margin: 46%
- Delivery Success Rate: 96%

**KPI Insights**

Choco De Luxe demonstrates strong overall commercial health, with €212.8k average revenue per agent, 46% profit margin, and an excellent 96% delivery success rate. However, performance is highly uneven across agents, with a small group materially outperforming while several agents destroy value (negative profit contribution when the target is €100,000). The core opportunity lies not in top-line growth alone, but in performance rebalancing, capability uplift, and selective intervention among underperformers.


**2. By Balance Band**
<p align="center">
  <img src="assets/Protarg.png" width="1000" />
</p>

**Top Performers (Profit ≥ €100k target)**
- Karlen McCaffrey – €31,994 profit (clear benchmark agent)
- Beverie Moffet – €20,956
- Kelci Walkden – €19,693
- Oby Sorrel – €19,525
- Dennison Crosswaite – €18,184

➡ These five agents set the operational gold standard, delivering high revenue, strong margins, and consistent execution

**Underperformers (Profit ≥ €100k target)**

Several agents generate negative profit, despite selling measurable volumes:
- Wilone O’Kielt: –€45,497
- Rafaelia Blaksland: –€41,494
- Camilla Castle: –€26,090
- Hussein Algar: –€18,091
- Mallorie Waber: –€17,628

**Key Insight:**

Poor profitability is not driven by delivery failures (delivery success ~100%), but likely by:
- Poor product mix
- Discounting/price erosion
- High cost-to-serve customer








- High Balance (100k–150k): 3,830 customers
- Low Balance (<50k): 3,692 customers
- Medium (50k-100k): 1,509 customers
- Very High Balance (150k+): 969 customers
- Most balances are clustered at the extremes - either low or high, suggesting a bimodal distribution
<p align="center">
  <img src="assets/Saledash.png" width="1000" />
</p>








### ⚠️ Key Challenges Identified
**1. Low Active Engagement**
- With only 51.51% active customers, nearly half of the customer base is disengaged or dormant.
  - This may contribute significantly to the 20.37% churn rate.

**2. Low Cross-Sell Penetration**
- Over 95% of customers have 1–2 products
  - Suggests missed opportunities for upselling/cross-selling additional financial services (loans, credit cards, investments, etc.)

**3. Weak Credit Quality**
- With a median credit score of 652 and 5,693 customers in Fair or Poor segments, the bank may be carrying higher credit risk.
  - Could impact loan default rates and profitability if not managed


---


## 📊 Churn & Risk Overview

<p align="right">
  <img src="assets/churn1.png" width="1000" />
</p>

### Top KPIs (Key Performance Indicators)
- Churn Rate: 20.37%
- No. of Customers churned: 2.037
- Churned Balance: $186M
- High-Risk Customers: 174
- High-Value Churn Rate: 24.98%
  - Key Risk: Nearly 25% of high-value customers churned, representing a significant financial loss and a priority focus area.

### 🌍 Churn by Location

| Country         | Churn Rate   | Churned Balance    | Key Insight                               |
|-----------------|--------------|--------------------|-------------------------------------------|
| **Germany**     |     32%      |       $97.9M       | Highest churn rate and balance loss       |
| **Spain**       |     17%      |       $29.9M       | Moderate churn, lower financial exposure  |
| **France**      |     16%      |       $57.7M       | Lower churn rate, but large value impact  |

⚠ Germany is a high-risk churn zone, both in terms of volume and financial value.

### Churn by Customer Type
**1. Active vs. Inactive**
- Inactive customers account for 65% of churn, which is only 48% of the base.
- Active customer churn rate = 35%, indicating even active users aren't fully engaged.

**Actionable Insight:** Inactivity is a major churn predictor. There is a need to consider stronger lifecycle management.

<p align="right">
  <img src="assets/risk2.png" width="1000" />
</p>

### Churn by Product Usage
| No. of Products    | Churn Rate    | No. of Churned     |
|--------------------|-------------- |--------------------|
|   1                |     28%       |        1,409       | 
|   2                |     8%        |        348         |
|   3                |     83%       |        220         | 
|   4                |     100%      |        60          |

Customers with only 1 product are the largest churn group (1,409 customers).

**Caution**

The dataset shows a 100% churn rate for customers with four products. On investigation, this segment has a very small sample size, and all instances are labelled as churned. This appears to be a dataset artifact rather than a realistic banking behavior, so insights from this segment should be interpreted with caution. Strategic focus should remain on 1–3 product customers, where both volume and churn impact are material.

### Churn by Age Group
| Age Group       | Churn Rate    | No. of Churned                        |
|-----------------|-------------- |---------------------------------------|
|   45-54         |     48%       |  Extremely high churn risk            |
|   55+           |     39%       |  Aging segment disengaging            |
|   35-44         |     18%       |  Moderate risk                        | 
|   <25           |     9%        |  Lower churn, oppourtunity to grow    |
|   25-34         |     8%        |   Best-performing segment             |

**Insight:** Mid-to-senior age customers are churning at 2-5x the rate of younger ones.

### Churn by Credit Score Band
| Credit Score Band       |  Churn Rate    |
|-------------------------|----------------|
|  Poor (<580)            |     22%        |
|  Fair (580-669)         |     21%        |
|  very Good (740-799)    |     21%        |
|  Excellent (800+)       |     20%        |
|  Good (670-739)         |     19%        |

**Insight:**

Churn is fairly consistent across credit bands, and no strong correlation between score and churn.

### Churn Balance by Risk Tier

| Risk Tier       |  Churned Balance  |
|-----------------|-------------------|
|  Medium         |     $106M         |
|  low            |     $79.4M        |
|  High           |     $0.2M         |

**Insight:**
- My analysis showed that customers at the highest churn risk tend to have lower balances, meaning they contribute less to direct financial loss.
- The majority of revenue loss actually comes from medium-risk, higher-value customers.
- This highlights the need for differentiated retention strategies.


---


## Financial Performance Summary

<p align="right">
  <img src="assets/Summary.png" width="1000" />
</p>

### KPIs Overview
- Total Customers: 10,000
- Churn Rate: 20.37% (2,037 customers churned)
- Average Retain Balance: $72,745
- Average Churn Balance: $91,109
- Total Balance: $765M
- Geographies: France, Germany, Spain

**Key Insights**
**1. High Churn Rate**
- A churn rate of 20.37% is relatively high, indicating a potential issue in customer retention.
- The average balance of churned customers ($91,109) is higher than that of retained customers ($72,745), suggesting that higher-value customers are churning.

**2. Geographical Distribution**
- Majority of customers are from:
  - France: 5,014 (50.1%)
  - Germany: 2,509 (25.1%)
  - Spain: 2,477 (24.8%)

However, a filtered drill-down shows:
- In Germany, customers under 25 years old, with medium churn risk, are notably present (96 customers).
- Within this filtered segment, gender is almost equally split: 41 males, 36 females.

**3. Age Group Analysis**
- Most customers fall into 35-44 and 25-34 age groups:
  - 35-44: 3,278 retained
  - 25-34: 2,972 retained

- However, <25 age group has the lowest retention (417) and churn (40) proportionally.
- Suggests younger customers are more likely to churn.

**4. Churn Risk Tiers**
- Within the Germany/<25/Medium Risk segment:
  - Most are in Medium Risk tier (77 out of 96).
  - Low (14) and High (5) are negligible.


---


## 🎯 Strategic Recommendations

A. **Customer Retention Strategy**

1. **Prioritize high-balance churners:**
   - Since churned customers have higher average balances, create retention campaigns targeting high-value customers.
   - Consider proactive outreach, loyalty rewards, or personalized financial advice.

2. **Develop targeted interventions for medium-risk segments:**
   - The largest risk category is medium. Launch "nudge" campaigns for this group to reduce the risk of escalation.
   - Examples: financial planning tools, regular check-ins, or premium service trials.

B. **Segment-Specific Strategies**

1. **Adults (45-54 age group) and Seniors (55+ age group)**
   - High churn and low retention indicate dissatisfaction or low engagement.
   - Actions:
     - Launch adults-focused products (e.g., retirement planning consultations, health savings-linked accounts, insurance bundles (health + life + critical illness)).
     - Improve digital engagement (mobile banking, in-app "easy mode" interface).

2. **Germany Segment**
   - Customers <25 in Germany are showing churn behavior.
   - Consider localized offers and customer engagement campaigns in Germany targeting this age group.

C. **Geographic Focus**
   - France has 50% of total customers – leverage this for upselling and cross-selling.
   - Spain and Germany: Evaluate marketing ROI and retention performance to determine if higher engagement is needed.

D. **Improve Churn Prediction & Early Warning**
   - Use the existing churn risk tiers to build a predictive churn model based on:
     - Age
     - Geography
     - Gender
     - Credit Score
     - Product usage
     - Balance trends
   - Focus on medium-risk segments and monitor any increase in early warning indicators.

E. **Financial Impact Monitoring**
   - Given that high churners have higher balances:
     - Quantify potential revenue loss from churn and build a business case for investing in retention programs.
     - Use dashboards to track CLV (Customer Lifetime Value) over time by segment.

### Next Steps

1. **Deep dive into churn drivers:** Survey churned customers, analyze product usage data.

2. **Build retention models:** Use machine learning (e.g., logistic regression, random forest) to predict churn risk.

3. **Refine segmentation:** Include behavioral data (transaction volume, complaints, digital activity).

4. **Test retention offers:** A/B test targeted campaigns for high-value and medium-risk customers.

5. **Monitor KPIs monthly:** Add trend charts for churn rate, NPS, and retention by geography and age.


---

🔗 [View the Live Dashboard](https://bit.ly/UnityBank_Customer_Churn_Risk)


## Executive Summary

This Power BI analytics solution provides Unity Bank with a comprehensive, data-driven view of its customer base, financial exposure, and churn risk. By leveraging the full capabilities of Power BI from data transformation to advanced DAX measures and interactive dashboards, the project delivers actionable insights that directly support customer retention, revenue protection, and risk mitigation efforts.

This analysis reveals that Unity Bank is facing a critical customer churn challenge, with over 20% of customers exiting and a disproportionately high churn among medium-risk and high-balance clients. Inactivity, low product penetration, and regional concentration (notably in Germany) emerge as leading indicators of churn. Additionally, the bank’s current churn risk tiering underestimates the risk posed by medium-tier customers, who account for the largest share of churned balance value.

The dashboards empower stakeholders to explore these dynamics through real-time, filterable views segmented by geography, age, credit score, product usage, and churn risk. This enables business leaders to move from reactive churn tracking to proactive customer engagement and risk prevention.

## Executive Recommendation

Unity Bank should implement a **targeted, data-driven customer retention strategy** focused on the following priorities:

1. **Prioritize Medium-Risk and High-Balance Customers**  
   - Proactively monitor and engage medium-risk customers, especially those with high balances, using early-warning signals from the dashboard.

2. **Reactivate Inactive Customers**  
   - Launch re-engagement campaigns and personalized offers for inactive users, who represent a large portion of churned customers.

3. **Increase Product Penetration to Reduce Churn**  
   - Design bundled product offerings and personalized cross-sell strategies to encourage customers with only one product to deepen their relationship with the bank.

4. **Localize Retention Strategies by Region**  
   - Tailor retention and service strategies for high-churn regions like Germany, where customer behavior significantly deviates from the rest of the portfolio.

5. **Refine Risk Scoring Models**  
   - Update churn risk models to reflect actual behavioral drivers found in the data, such as inactivity, single product ownership, and regional trends, to improve prediction accuracy.

By implementing these actions, Unity Bank can significantly reduce churn, improve customer lifetime value, and drive sustainable revenue growth through smarter, insight-led decisions.


---


## Disclaimer
This project is for portfolio and educational display only.

No content may be reused without permission.


---


## Connect With Me
- 💼 **LinkedIn:** (https://www.linkedin.com/in/david-okeleye001/)
- 📧 **Email:** okeleyedavid2021@gmail.com
- 🌐 **Portfolio:** https://bit.ly/3N5c1p7
- 🐙 **GitHub:** https://github.com/olavidz01-dev
