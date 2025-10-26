# OPERATOR-PERFORMANCE-AND-WELL-PRODUCTIVITY

# Operator Performance and Well Productivity Dashboard

## Overview
The **Operator Performance and Well Productivity Dashboard** is a data-driven analytical report developed to evaluate oil and gas well operations across Ontario fields. The project leverages **Power BI** to visualize drilling activities, operator efficiency, well outcomes, and subsurface depth dynamics spanning from **1800 to 2019**.

The analysis identifies the **top operators by total wells drilled**, showing **Dominion Natural Gas Company Ltd** and **Union Gas Limited** as the leading contributors. A **well type distribution chart** highlights that **46.3% of wells were natural gas wells**, confirming that the studied fields are predominantly gas-reserved zones.

The dashboard also reveals that **Birchfield Oil and Gas Company** achieved the **deepest drilling depth (18,625 m)** due to operating in regions where reservoirs lie deeper beneath the surface. Additionally, an **elevation–depth relationship analysis** shows that lower elevation areas require deeper drilling to reach the reservoirs.

Overall, this project provides valuable insights into **operator performance**, **well productivity**, and **geological drilling behavior**, empowering stakeholders to make **data-informed decisions** regarding licensing, field development, and future drilling investments.

## Problem Statement
Over the years, multiple operators have been drilling wells across our licensed regions, but we lack a clear and data-driven understanding of how each operator is performing.  
The goal is to identify **which operators are contributing the most productive wells** and **which ones have the highest number of dry holes or shallow completions**.  

We need visibility into their overall **drilling activity, well outcomes, and average well depths**.  
With this, we can pinpoint **high-performing operators**, evaluate **underperforming ones**, and make **data-informed decisions** on future partnerships, licensing, and operational investments.  

The end goal is to present these insights clearly and interactively through a **Power BI dashboard**.

---

## Objectives
1. Determine the total number of wells drilled by each operator.  
2. Classify and count wells by type (e.g., Natural Gas, Oil, Dry Hole) for each operator.  
3. Calculate the average and maximum total depth achieved by wells per operator.  
4. Compute the proportion of productive wells versus dry holes for each operator.  
5. Develop an interactive **Power BI dashboard** showing operator rankings, well outcomes, and depth metrics across time and regions.  

---

## Data Collection
The dataset used for this project was sourced from **Kaggle**, by searching for *oil and gas / petroleum datasets*.  
It contains data points spanning from **1800 to 2019**, providing historical insights into drilling activity and performance.  

**Dataset Link:** [Ontario Petroleum Wells – Kaggle](https://www.kaggle.com/datasets/vaishnavivenkatesan/ontario-petroleum-wells)

## Data Cleaning and Preparation
During the inspection of the dataset in **Microsoft Power BI Power Query**, a few data quality issues were identified and resolved as follows:

- **Missing Values:** Searched for and replaced missing values with mean values (for numerical columns) and modal values (for text columns).  
- **Duplicates:** Inspected the dataset for duplicate records and confirmed that none were present.  
- **Data Type Conversion:** Some columns (e.g., `well_id`) were in the wrong format (text), so they were converted to appropriate data types (e.g., integer).

---

## Feature Selection
Since the dataset contained numerous columns, only relevant fields were selected for this analysis:  
`well_id`, `well_name`, `operator`, `well_type`, `well_mode`, `latitude`, `longitude`, `ground_elevation`, `total_depth`, `county`, `township`, `spud_date`, and `total_depth_reached_date`.

---

## Exploratory Data Analysis (EDA)
A **three-page interactive Power BI dashboard** was developed to present insights effectively:
1. **Page 1:** Displays key KPIs and high-level summary metrics.  
2. **Page 2:** Visualizes trends and operator-based comparisons.  
3. **Page 3:** Shows the spatial distribution of wells on a map view.

---

## Insights

1. **Total Wells by Operator:**  
   *Dominion Natural Gas Company Ltd* drilled the most wells (2.6K), followed by *Union Gas Limited* (1.4K) and *Unknown Operators* (0.4K).  
   This dominance is attributed to the abundance of natural gas in the region, making gas extraction companies the top operators.

2. **Historical Drilling Trends:**  
   The fewest wells were drilled in **1863 (only one well)**, gradually rising to **1,293 wells in 1970**.  
   The spike in 1970 was driven by increased energy demand, technological advancements, and domestic expansion.  
   Major drilling locations included **Lambton (515)** and **Kent (603)**.

3. **Well Type Distribution:**  
   - Natural Gas Wells: **46.3%**  
   - Dry Holes: **24%**  
   - Gas Show Wells: **13.3%**  
   - Oil Wells: **10.6%**  
   - Private Gas Wells: **5.8%**  
   This confirms the region is largely gas-reserved compared to oil.

4. **Deepest Wells:**  
   *Birchfield Oil and Gas Company* achieved the deepest well at **18,625 m**, followed by *Hockley Valley Oil and Gas Co.*  
   These operators drilled in regions where reservoirs are deeper below the surface.  
   Birchfield’s record well was classified as a **gas show well** rather than productive or dry.

5. **Elevation vs. Depth Relationship:**  
   Wells drilled in **lower elevation areas** were found to be deeper.  
   This suggests that deeper drilling is required in low-lying regions to reach the target reservoirs.

---

## Recommendations

1. **Focus Future Drilling in Proven Gas-Reserve Regions**  
   With 46.3% of wells producing natural gas, exploration efforts should continue prioritizing proven gas-rich zones to maximize productivity and minimize risk.

2. **Invest in Deeper Drilling Technologies for Low-Elevation Zones**  
   Since lower-elevation wells require deeper drilling, investing in advanced drilling and subsurface mapping technologies will improve efficiency and cost management.

3. **Strengthen Operator Performance Monitoring**  
   Implement consistent benchmarking and well outcome tracking to identify high-performing operators, reduce dry holes, and guide future licensing and operational strategies.

---

## Conclusion
The analysis of over **20,000 wells drilled by 1,000+ operators** revealed vital insights into operator performance, productivity, and geological behavior.  
Gas extraction dominated the operations, led by *Dominion Natural Gas Company Ltd*, while *Birchfield Oil and Gas Company* recorded the deepest well due to deeper reservoir zones.  

This project demonstrates how **data analytics and Power BI visualization** can uncover performance patterns, support data-driven decision-making, and guide future drilling strategies for more efficient and productive operations.


