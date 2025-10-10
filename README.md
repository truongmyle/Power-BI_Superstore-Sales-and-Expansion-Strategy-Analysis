# [Power BI] Sales & Expansion Strategy Analysis | Retail
# 📊 Project Title: Sales & Expansion Strategy Analysis  

Author:Truong My Le

Date: 2025-08-26  

Tools Used: Power BI  

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

## 📌 Background & Overview  

### Objective:
### 📖 What is this project about? 
 
This project uses Power BI to analyze global sales data from the “Global Superstore” dataset in order to:

✔️ Understand overall business performance across markets and product categories.

✔️ Identify high-performing regions and potential markets for expansion.

✔️ Determine strategic product segments that drive profit and revenue growth.

### 👤 Who is this project for?  

✔️ Senior Managers & Decision-makers seeking insights to support market expansion strategies.

✔️ Data Analysts & Business Analysts who want to visualize and evaluate global business performance using Power BI.

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  
- Source: Provided by Superstore Global Sales dataset 
- Size:
  - `Orders.csv`: 51,290 rows × 20 columns  
  - `People.csv`: 13 rows × 2 columns  
  - `Returns.csv`: 1,172 rows × 2 columns    
- Format: CSV files (.csv)

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  

The dataset contains 3 tables:
- Orders: Contains detailed transaction information.
- People: Stores information about sales representatives in each region.
- Returns: Records orders that were returned.

#### 2️⃣ Table Schema & Data Snapshot  

<details>
<summary>Table 1: Orders</summary>  
  
| Column Name   | Data Type | Description |
|---------------|----------|-------------|
| Order_ID      | INT      | Unique identifier for each transaction |
| Order_Date    | DATE     | Date the order was placed |
| Ship_Mode     | TEXT     | Delivery mode selected by the customer |
| Segment       | TEXT     | Customer segment |
| Country       | TEXT     | Country of sale |
| Region        | TEXT     | Sales region |
| Market        | TEXT     | Market group |
| Category      | TEXT     | Product category |
| Sub_Category  | TEXT     | Product subcategory |
| Sales         | FLOAT    | Sales revenue |
| Quantity      | INT      | Quantity sold |
| Profit        | FLOAT    | Profit from the transaction |
| Type          | TEXT     | Type of order (Standard, Express, etc.) |

</details>

<details>
<summary>Table 2: People</summary> 
  
| Column Name   | Data Type | Description |
|---------------|----------|-------------|
| Person        | TEXT     | Sales representative |
| Region        | TEXT     | Region assigned |

</details>

<details>
<summary>Table 3: Returns</summary>

| Column Name   | Data Type | Description |
|---------------|----------|-------------|
| Order_ID      | INT      | Returned order ID |
| Returned      | TEXT     | Yes/No flag indicating return status |

</details>

#### 3️⃣ Data Relationships:  
<img width="1017" height="605" alt="image" src="https://github.com/user-attachments/assets/0b02d0ec-5806-4bce-9b0c-a08545d8c959" />

---

## 🧠 Design Thinking Process  

### Step 1: Empathize
<img width="1854" height="574" alt="image" src="https://github.com/user-attachments/assets/a2d29cdb-8a86-463a-95e4-f1139b7674a0" />

### Step 2: Define POV
<img width="1862" height="518" alt="image" src="https://github.com/user-attachments/assets/b32098d0-5252-4f85-b8c7-e79feec06fc9" />

### Step 3: Ideate
<img width="1835" height="546" alt="image" src="https://github.com/user-attachments/assets/4400ff78-abc0-412b-bc64-32b0161a6e77" />

### Step 4: Prototype and Review
- This section is shown in Dashboard

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Business Overview  
<img width="1197" height="672" alt="image" src="https://github.com/user-attachments/assets/d1e3f9bb-0973-496c-bed4-00391f92fbf9" />

🎯Observations:  

**By Time:**
- Sales and profit **steadily increased** from 2011 to 2014, with profit margin consistently around 11–12%.
- Profit peaks toward the end of the year, especially **September** (+66.3%).
  
**By Category:**
- **Technology** ($4.7M, 13.9% margin) and **Office Supplies** ($3.8M, 13.6% margin) deliver the **highest profitability**.
- Furniture ($4.1M, 6.4% margin) generates solid sales but has the lowest profit margin.

**By Market (%Return):**

Canada, Africa, and EMEA have **very small bubbles**, meaning return rates are negligible.

#### 2️⃣ Market Analysis
<img width="1299" height="726" alt="image" src="https://github.com/user-attachments/assets/d0c89111-63de-4a41-9905-61a9f11cf401" />

🎯Observations:

- **APAC, EU, and US** are the top profit-generating markets.
- Return rates are 0% in **Africa, Canada, and EMEA**, meaning minimal risk from product returns in these regions.
- **Canada** has the highest profit margin (26.6%) but very small absolute profit.
- High-growth, profitable sub-categories include **Copiers, Phones, Bookcases.**

#### 3️⃣ Product Analysis
<img width="1299" height="736" alt="image" src="https://github.com/user-attachments/assets/9bb0c061-fc09-4bd4-83e4-51f1be35a7f7" /> 

🎯Observations:   

- **Tables, Appliances, and Fasteners** have the **highest return rates** (≈ 8–8.5%), making them key risk items.
- **Tables** show the highest growth rate (34.4%) but from a small customer base (563), remain unprofitable (-$0.06M, –8.46% margin) -> **growth without profitability**.
- **Machines** (33.3%) and **Bookcases** (25%), **Copiers** (24.6%) combine both high growth and a larger customer base (900–1000+), making them stronger drivers of expansion.

#### 4️⃣ Product Details
<img width="1281" height="733" alt="image" src="https://github.com/user-attachments/assets/cb008d8a-9e27-451a-ad22-04f989152dac" />

---

## 🔎 Final Conclusion & Recommendations  

### 1. Market Expansion 

- **Canada**: High profit margin ( 26.62%), fast customer growth ( 41.4%), and strong efficiency despite low sales volume → **priority market for expansion**.
    - Recommendation: Increase investment in **Sales, Marketing, and Logistics**.
    - Strategic products: **Copiers, Phones** (high margin, stable sales).
- **Africa**: Stable growth, high profit margin (11.3%), and good customer growth (+12.5%) with relatively low sales loss → **potential market for moderate expansion**.
    - Strategic products: Focus expansion on **Phones** (top-selling, 15.4% profit margin).

---

### 2. Current Market Optimization

- **APAC**: Top performing region → **continue heavy investment**, focus on **Technology & Furniture**.
- **EU**: Large revenue and strong growth → expand **Technology & Office Supplies**, monitor return rates.
- **US**: High profitability → boost revenue through product expansion and targeted marketing.
- **LATAM**: Strong growth but low margins → improve **cost control and Average Order Value**.
- **Africa & EMEA**: Large customer base but negative profit → **investigate root causes** or consider market withdrawal.

---

### 3. Product Performance

- **Copiers, Phones**: Strategic products with strong performance across all markets.
- **Tables**: Consistent losses → discontinue or implement new pricing strategy.
- **Canon Copier**: High return rate → investigate and address quality/operational issues.
