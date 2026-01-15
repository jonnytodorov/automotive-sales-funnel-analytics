# Automotive Sales Funnel Analytics
An analytics project investigating marketing campaign performance across the automotive sales funnel, from lead to final purchase. This dashboard was built using SQL and Power BI to assess attribution sensitivity, conversion behaviour, and financial performance metrics.

### Dashboard walkthrough
A short video walkthrough explaining the dashboard structure, key metrics and insights: 
[Watch on Loom](https://www.loom.com/share/8e0274750cb64996bb33c546a800fc14)

---

## Problem Statement
The automotive industry is one of the largest globally, with marketing investments spread across multiple channels. Accurately identifying the most profitable campaigns is challenging without analyzing attribution assumptions throughout the entire sales funnel.

<i>This portfolio addresses three main questions:</i>
1. How effectively do leads progress through the sales funnel, and how do conversion rates vary over time and across locations?
2. Which marketing channels deliver the strongest financial results, and how sensitive are metrics like ROI and CPA to attribution assumptions?
3. How do campaign results based on descriptive measures (e.g. ROAS) compare to insights from statistical methods such as linear regression?

The goal is to support data-driven marketing budget decisions by identifying the most profitable channels through descriptive and statistical analyses, backed by well-structured data models, clearly defined KPIs, and insightful analytics.

---
## Data & Tools
<b>Data:</b>
* Synthetic CSV datasets simulating the full customer journey from initial lead to final purchase. 
* Fact tables include leads, test drives, and sales; dimension tables contain campaigns, customers, and dealerships. Table sizes range from 8 rows (campaigns) up to 8,000 (leads).

<b>Tools:</b>
* PostgreSQL was used for data cleaning, date handling, and statistical preparation. 
* Power BI managed data shaping and dashboard development, with Power Query (M) for transformations and DAX for KPI calculations and analysis.

---
## Dashboard Overview
The dashboard has five pages covering key areas of the automotive sales funnel and campaign performance.

<b>1. Funnel Overview:</b> National sales funnel over two years. KPIs: leads, test drives, sales, conversion rates, and average days to purchase. Slicers by province and month.

<b>2. Campaign Performance:</b> Table with leads, sales, and profit. Visuals include spend vs. revenue scatter plot with a trend line, plus bar chart for ROI, ROAS, and CPA by campaign.

<b>3. Dealership Map:</b> Interactive map of Canada showing dealership sales volume (bubble size), with revenue and average sales price on hover. Filters by campaign and month.

<b>4. Customer Cohorts:</b> Two heatmaps of lead-to-customer conversion and purchase timing by cohort month over six months.

<b>5. Advanced analytics:</b> Statistical insights including attribution sensitivity, linear regression (R²), outlier detection via z-scores, and a two-sample t-test of commercial vs. private customers.

---
### Key Insights

* Most sales occur months after lead creation, explaining why short attribution windows miss many sales. Lead-to-sale rates remain stable across regions despite volume differences.

* Campaign performance varies by metric: Search Ads lead in volume and revenue; SMS has highest ROI due to very low CPA despite lower revenue, showing high ROI alone doesn’t guarantee overall success.

* Some sales can’t be directly linked to campaigns; accounting for these unassigned conversions is crucial when evaluating campaign performance. 

* Large dealerships drive most sales; average sale prices are consistent across locations. Smaller dealers show more extreme averages due to fewer transactions, and campaign choice minimally impacts dealership results.

* Cohort analysis reveals most lead-to-customer conversions happen within six months, with timing varying by cohort; purchases usually follow quickly after conversion.

* Statistical analysis adds depth: Z-scores show Search Ads as top and Email as worst performer; low R² suggests campaign spend explains little revenue variation, indicating other factors play key roles.

---
## Dashboard & Schema Screenshots

### Page 1: Funnel Overview

<p align="center">
<img src="page_1_funnel.png" width="775">
</p>

### Page 2: Campaign Performance

<p align="center">
<img src="page_2_campaigns.png" width="775">
</p>

### Page 3: Dealership Map

<p align="center">
<img src="page_3_map.png" width="775">
</p>

### Page 4: Customer Cohorts

<p align="center">
<img src="page_4_cohort.png" width="775">
</p>

### Page 5: Advanced Analytics

<p align="center">
<img src="page_5_analytics.png" width="775">
</p>

### Snowflake Schema 

<p align="center">
<img src="snowflake_schema.png" width="775">
</p>

---
<p align="center">
<strong> 🇩🇪 Deutsche Version verfügbar:</strong>
   <a 
href="https://github.com/jonnytodorov/automobil-verkaufsfunnel-analyse">Hier klicken</a>
</p>

---
<p align="center">
  <em>Automotive Sales Funnel & Campaign Anaytics Dashboard</em><br>
<strong>Jonathan Todorov, MA</strong> Business Analytics Portfolio 2026 EN</p>


