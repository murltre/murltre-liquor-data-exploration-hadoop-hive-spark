# 🧊 Liquor Sales Data Exploration Using Hadoop, Hive, and Spark

This project explores large-scale liquor sales data from Iowa (2021–2022) to uncover actionable business insights using a big data analytics pipeline. Leveraging **Hadoop**, **Hive**, **Spark**, and **Tableau**, we addressed three business questions around store performance, pricing strategies, and vendor profitability using over **over 3 million records**.

---

##  Dataset Overview

- **Source**: [Kaggle - Iowa Liquor Sales](https://www.kaggle.com/)
- **Size**: ~1 GB (3 million+ records, 24 columns)
- **Time Period**: January 2021 to January 2022
- **Fields Included**:
  - Store name, product type, vendor, brand, alcohol content
  - Volume sold, unit price, total sales, purchase date


![image](https://github.com/user-attachments/assets/a189bc04-2cac-48fb-b1da-22b0b2dcf882)

![image](https://github.com/user-attachments/assets/2bc4af8b-3da4-4f7b-9ff3-baec1b2dfa27)

---

## Business Questions

1. **Stores & Categories Performance**  
   How do store volumes and product sales correlate with total dollar sales?

2. **Pricing Strategy**  
   How does pricing affect sales volume and profitability across categories?

3. **Vendor & Category Profitability**  
   Which vendors and products contribute most to profitability, and how can this inform inventory and negotiation strategies?

---

## Tools & Technologies

- **Apache Hadoop** (HDFS)
- **Apache Hive** (SQL-based querying)
- **Apache Spark** (Data processing & transformation)
- **Tableau** (Data visualization)
- **HiveQL / SQL**

---

## Data Processing Workflow

1. Loaded CSV dataset into Hadoop Distributed File System (HDFS)
2. Processed data with **Apache Spark** to clean, format, and prepare for analysis
3. Queried datasets using **HiveQL** to compute key metrics
4. Visualized insights using **Tableau dashboards**

---

## Key Insights & Results

### 1️⃣ Store & Category Performance
- **Hy-Vee #3 / Des Moines** and **Central City 2** led in total sales
- **Central City Liquor, Inc.** had a **high profitability ratio** of `$104.55 per gallon` on `$2.8M` revenue
- **Top Categories by Revenue**:
  - **American Vodkas**: `$65M` (highest sales)
- **Top Categories by Profitability**:
  - **Imported Brandies**: `$184 per gallon`
  - **100% Agave Tequila**: `$147.38 per gallon`



💡 *Recommendation*: Increase premium product stock in high-ratio stores (e.g., Central City, Urbandale) to improve margins.

---

### 2️⃣ Pricing Strategy & Elasticity
- Calculated price elasticity using % change in quantity vs. price
- **High Elasticity Categories** (very price-sensitive):
  - American Cordials & Liqueurs, Coffee Liqueurs, RTD Cocktails
- **Low Elasticity Categories**: More stable in price

💡 *Recommendation*:  
  - **Lower prices** slightly for high-elasticity products to boost volume  
  - **Raise prices** for low-elasticity products without losing sales volume

---

### 3️⃣ Vendor Profitability
- **Top Vendor**: **DIAGEO AMERICAS**
  - Dominant in **Canadian Whiskies** and **Spiced Rum**
- **Sazerac Company** showed balanced volume & profitability in Whiskey Liqueur

💡 *Recommendation*:  
  - Partner with DIAGEO for **joint promotions** and **exclusive access**  
  - Use **competitive pricing** to grow Sazerac sales volume

---

## Visualizations

- ## Top 20 Liquor Stores based on Total Revenues

![image](https://github.com/user-attachments/assets/d8b344be-79ec-4e1d-b9fb-118a8c4f1fe0)

Despite its strong sales, Costco Wholesale #788 / WDM has a lower dollar-to-volume ratio of $55.6, indicating a strategy that prioritizes volume over higher profit margins per unit

- ## Liquor Stores ranked based on the dollar/volume ratio
![image](https://github.com/user-attachments/assets/95598765-5ad8-4c8c-a5e4-9af579a82f6c)



- ## Top 20 Liquor Categories ranked by revenues
![image](https://github.com/user-attachments/assets/e592059a-2bb1-4dd3-84bf-77845ef41ad0)

Even though with the highest revenue of $65M, American Vodkas yet exhibit a lower profitability ratio at $41, ranked 7th

---

## Conclusions

- Big data tools like **Hadoop**, **Hive**, and **Spark** allow for scalable analysis of multi-million-row datasets  
- **Dollar-to-volume ratio** and **price elasticity** are powerful profitability indicators
- Business recommendations included **optimizing inventory**, **revising pricing strategies**, and **targeting vendor relationships** based on data

---


*Big Data Analytics conducted on a virtual machine using Hadoop and Spark*

