# 🥑 US Avocado Retail Sales Analysis (Google Data Analytics Case Study)

An end-to-end data analytics project investigating price elasticity, regional premium pricing hotspots, and seasonal demand trends for conventional and organic avocados. This case study follows the **Google Data Analytics Framework**: *Ask, Prepare, Process, Analyze, Share, and Act*.

---

## 📂 Project Structure
* `avocado_cleaned.ipynb`: The complete Jupyter Notebook containing all data cleaning, analysis, and visualization source code.
* `avocado_cleaned.csv`: The processed, clean dataset used for analysis.

---

## 📋 Phase 1: Ask
* **Business Task:** Analyze historical retail scan data to optimize inventory allocation, geographic targeting, and seasonal pricing strategies for a national grocery retail chain.
* **Core Problem:** The business needs to identify structural performance differences between higher-margin organic avocados and high-volume conventional avocados to maximize profitability.
* **Primary Stakeholders:** VP of Merchandising, Inventory Managers, and the Director of Business Intelligence.

---

## 📂 Phase 2: Prepare
* **Data Source:** Historically generated retail scan data from the Hass Avocado Board (originally compiled by Justin Kiggins, CC0 Public Domain).
* **Data Organization:** The raw dataset contains weekly transactional records across multiple years (2015–2018) mapped by unique US cities and regions.
* **Credibility Check (ROCCC):** Sourced directly from grocery register scanners, making it highly reliable and original.

---

## 🐍 Phase 3: Process & Data Integrity
Data cleaning and transformations were executed via Python in a Jupyter Notebook environment:
* Verified that the dataset contains **0 missing entries** and **0 duplicate rows**.
* Transformed generic PLU item attributes (`4046`, `4225`, `4770`) into human-readable definitions (`small_hass_sold`, `medium_hass_sold`, `large_hass_sold`).
* Parsed text objects into explicit `datetime` stamps to programmatically extract `month` and `year` trackers.

---

## 📊 Phase 4: Analyze & Share
Key programmatic aggregations and visual charts generated the following analytical findings:

### 1. Market Segmentation
* **Conventional Avocados:** Driven by high-velocity consumer demand, moving **15.09 Billion units** at a lower mean retail price of **\$1.16**.
* **Organic Avocados:** Operates as a lower-velocity premium tier, moving **0.44 Billion units** while commanding a strict **42% price premium (\$1.65)**.

### 2. Geographic Price Premium
The top 5 most expensive retail zones in the country are concentrated in dense urban clusters:
1. **Hartford / Springfield:** \$1.82
2. **San Francisco:** \$1.80
3. **New York:** \$1.73
4. **Philadelphia:** \$1.63
5. **Sacramento:** \$1.62

### 3. Chronological Seasonality & Price Elasticity
* **Seasonal Shifts:** Retail costs experience an active cyclical spike across late-summer and early-autumn market months, peaking sharply in **October (\$1.58)** and **September (\$1.57)** before hitting a baseline floor in **February (\$1.27)**.
* **Market Elasticity:** Calculated a price-to-volume correlation coefficient of **-0.1928**. This confirms standard retail price elasticity—as retail unit pricing rises, individual purchasing velocity predictably scales downward.

---

## 🚀 Phase 5: Act
Based on the data-driven insights discovered above, the following tactical implementations are recommended for the business:

* **Deploy Dynamic Seasonal Pricing:** Accept slimmer, competitive pricing margins during high-velocity Q1 periods to capture grocery market share, then aggressively expand retail markups between August and October when seasonal consumer willingness to pay peaks.
* **Optimize Geographic Allocation:** Direct higher-margin organic inventory shipments to premium-tolerant urban zones (Northeast and West Coast metros) while leaning on stable conventional arrays in standard regional distributions.
* **Incentivize Organic Volume through Bundling:** Leverage the negative correlation coefficient (-0.1928) by executing multi-buy or cross-promotional bundle frameworks for organic stock to break consumer price friction and convert mainstream conventional shoppers.

---

## 🛠️ Tools & Technologies Used
* **Language:** Python
* **Libraries:** Pandas, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab


