<div align="center">

# -- ! Superstore Sales Analysis — Power BI Dashboard ! --
### *Interactive Sales, Profit & Discount Analysis using Power BI*

[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Dataset](https://img.shields.io/badge/Dataset-9%2C994%20Rows-4472C4?style=for-the-badge)](#-overview)
[![Analysis](https://img.shields.io/badge/Analysis-Sales%20%26%20Profit-F39C12?style=for-the-badge)](#-part-c--kpi-analysis)
[![Dashboard](https://img.shields.io/badge/Dashboard-Interactive-008C95?style=for-the-badge)](#-part-d--interactive-dashboard)

<br/>

> *"Turn raw Superstore sales data into clear, interactive insights with Power BI."*

</div>

---

## 📋 Table of Contents

- [📌 Overview](#-overview)
- [🎯 Problem Statement](#-problem-statement)
- [✨ Key Features](#-key-features)
- [🏗️ Project Structure](#️-project-structure)
- [🔄 Project Workflow](#-project-workflow)
- [🧹 Part A — Dataset Import](#-part-a--dataset-import)
- [🧽 Part B — Data Cleaning & Modeling](#-part-b--data-cleaning--modeling)
- [📊 Part C — KPI Analysis](#-part-c--kpi-analysis)
- [📈 Part D — Interactive Dashboard](#-part-d--interactive-dashboard)
- [🎥 Video Demo](#-video-demo)
- [🛠️ Tech Stack](#️-tech-stack)
- [📈 Results & Insights](#-results--insights)
- [🏆 Advantages](#-advantages)
- [📄 License](#-license)
- [👤 Author](#-author)
- [🙏 Acknowledgements](#-acknowledgements)

---

## 📌 Overview

The **Superstore Sales Analysis — Power BI Dashboard** is a Power BI project built on the Superstore dataset of **9,994 order lines** (5,009 unique orders, 793 customers, 49 states) covering **January 2014 to December 2017**.

The report takes the data through a complete analysis workflow:

- Import the Superstore CSV into Power BI
- Clean and prepare the data (data types, date hierarchy)
- Build KPI cards for **Sales, Profit, Quantity and Average Discount**
- Create visuals by **Sub-Category, Product Category and Region**
- Add interactive **Region** and **Category** slicers
- Add a **Detailed Order Data** table that supports drill-through / tooltip style exploration

### 📁 Dataset Information

| Item | Details |
|------|---------|
| Dataset | `superstore.csv` |
| Total Rows | **9,994** |
| Unique Orders | **5,009** |
| Date Range | **Jan 2014 – Dec 2017** |
| Main Measures | Sales, Quantity, Discount, Profit |
| Main Dimensions | Customer, Segment, Region, State, City, Category, Sub-Category, Product |

---

## 🎯 Problem Statement

> **Objective:** Transform the Superstore sales data into an interactive Power BI dashboard that shows where sales are strong, where profit is lost, and how discounts affect results.

| 📂 Project Area | 📄 Type | 🔍 Description |
|----------------|---------|----------------|
| Raw Data | Source Data | Superstore CSV imported into Power BI |
| Data Model | Data Preparation | Typed columns, date hierarchy (Year / Quarter / Month / Day) |
| KPI Cards | Measures | Sum of Sales, Sum of Profit, Sum of Quantity, Average of Discount |
| Charts | Visualization | Sales by Sub-Category, Sales by Category, Profit by Region |
| Slicers | Interactivity | Region and Category filters |
| Detail Table | Drill-down | Order-level data with customer, segment, product and profit |

---

## ✨ Key Features

| Feature | Description |
|--------|-------------|
| 📥 **CSV Import** | Superstore data loaded directly into Power BI |
| 🧹 **Data Preparation** | Data types fixed and date broken into Year, Quarter, Month and Day |
| 📌 **KPI Cards** | Sum of Sales, Sum of Profit, Sum of Quantity, Average of Discount |
| 📊 **Sales by Sub-Category** | Bar chart showing which sub-categories sell the most |
| 🗂️ **Sales by Product Category** | Office Supplies vs Technology vs Furniture |
| 🌍 **Profit by Region** | West, East, South and Central compared (Central shows a loss in the selected view) |
| 🎛️ **Interactive Slicers** | Region and Category checkboxes update every visual |
| 📋 **Detailed Order Data** | Order-level table with Segment, Category, Sub-Category, Sales, Quantity, Discount and Profit |
| 🔄 **Live Cross-Filtering** | Click any visual to filter the rest of the dashboard |

---

## 🏗️ Project Structure

```text
📦 PowerBI-SalesDashboard/
│
├── 📄 Sales_Dashboard.pbix        ← Main Power BI report
├── 📄 README.md                   ← Project documentation
│
├── 📁 dataset/
│   └── 📄 superstore.csv          ← Source dataset
│
└── 📁 assets/
    ├── 🖼️ 01_detailed_order_data.jpg
    └── 🖼️ 02_sales_dashboard.jpg
```

### 📚 Report Map

| Section | Purpose |
|------|---------|
| **Title & Logo** | "Superstore Sales Dashboard" header with SALES icon |
| **KPI Cards** | Four headline numbers for the current filter selection |
| **Sum of Sales by Sub-Category** | Sub-category ranking by sales |
| **Slicers (Region, Category)** | Interactive filters |
| **Total Sales by Product Category** | Category-level sales comparison |
| **Total Profit by Region** | Regional profit comparison |
| **Detailed Order Data** | Order-level table for deeper investigation |

### 🖼️ Detailed Order Data Preview

![Detailed Order Data](assets/01_detailed_order_data.jpg)

---

## 🔄 Project Workflow

```text
Project Start
      │
      ▼
┌────────────────────────────────────┐
│  Step 1 — Import Dataset          │
│  superstore.csv → Power BI        │
└───────────────┬────────────────────┘
                │
                ▼
┌────────────────────────────────────┐
│  Step 2 — Clean & Model Data      │
│  Data types + date hierarchy      │
└───────────────┬────────────────────┘
                │
                ▼
┌────────────────────────────────────┐
│  Step 3 — Create KPI Measures     │
│  Sales / Profit / Qty / Discount  │
└───────────────┬────────────────────┘
                │
                ▼
┌────────────────────────────────────┐
│  Step 4 — Build Visuals           │
│  Bar charts + detail table        │
└───────────────┬────────────────────┘
                │
                ▼
┌────────────────────────────────────┐
│  Step 5 — Add Slicers & Format    │
│  Region + Category filters        │
└───────────────┬────────────────────┘
                │
                ▼
┌────────────────────────────────────┐
│  Step 6 — Publish / Share         │
│  Final interactive dashboard      │
└────────────────────────────────────┘
```

---

## 🧹 Part A — Dataset Import

### 📝 1. Source Dataset

The project uses **`superstore.csv`** (kept in the `dataset/` folder).

The main fields include:

- Row ID, Order ID
- Order Date, Ship Date, Ship Mode
- Customer ID, Customer Name, Segment
- Country, City, State, Postal Code, Region
- Product ID, Category, Sub-Category, Product Name
- Sales, Quantity, Discount, Profit

### 📌 2. How to Load

1. Open Power BI Desktop
2. **Home → Get Data → Text/CSV**
3. Select `dataset/superstore.csv`
4. Click **Transform Data** to check types, then **Close & Apply**

---

## 🧽 Part B — Data Cleaning & Modeling

### 🔍 3. Preparation Steps

- Checked column data types (dates, whole numbers, decimals, text)
- Converted **Order Date** into a proper date column
- Used the Power BI **date hierarchy** to get **Year, Quarter, Month and Day**
- Kept Sales, Quantity, Discount and Profit as numeric measures (Sum / Average)

### 📊 4. Measures Used

| Measure | Aggregation |
|--------|-------------|
| **Sum of Sales** | Sum of `Sales` |
| **Sum of Profit** | Sum of `Profit` |
| **Sum of Quantity** | Sum of `Quantity` |
| **Average of Discount** | Average of `Discount` |

---

## 📊 Part C — KPI Analysis

The dashboard displays four KPI cards that respond to the slicers:

| KPI | Description |
|-----|-------------|
| **Sum of Sales** | Total sales for the current selection |
| **Sum of Profit** | Total profit for the current selection |
| **Sum of Quantity** | Total units sold |
| **Average of Discount** | Average discount applied |

### 📌 Full Dataset Totals (no filters)

| Metric | Value |
|-------|-------|
| Total Sales | ≈ 2.30M |
| Total Profit | ≈ 286.4K |
| Total Quantity | 37,873 |
| Average Discount | ≈ 0.16 |

> The dashboard screenshot below shows a **filtered view**, so its KPI values are lower than the full-dataset totals above.

---

## 📈 Part D — Interactive Dashboard

### 🎛️ Dashboard Filters

- **Region** — Central, East, South, West
- **Category** — Furniture, Office Supplies, Technology

Selecting any checkbox updates the KPI cards and all charts.

### 📊 Visuals

| Visual | What it shows |
|-------|---------------|
| **Sum of Sales by Sub-Category** | Binders, Accessories, Bookcases, Appliances, Art, etc. |
| **Total Sales by Product Category** | Office Supplies, Technology, Furniture |
| **Total Profit by Region** | West, East, South, Central |
| **Detailed Order Data** | Order-level rows with customer, segment, category, sales, quantity, discount and profit |

### 🖼️ Dashboard Preview

![Superstore Sales Dashboard](assets/02_sales_dashboard.jpg)

---

## 🎥 Video Demo

> 🎬 **Watch the walkthrough:**
> 
> **[▶️ Click here to watch the project demo]([https://drive.google.com/drive/u/2/folders/1ghA2Tm8vuXUYFcdI92iz-bt132rX_1c8](https://drive.google.com/file/d/1LATvE76XKB8bhNL3C5FnSFVIMWUXxQ8b/view?usp=sharing))**

---

## 🛠️ Tech Stack

| Tool / Feature | Purpose |
|----------------|---------|
| 📊 **Power BI Desktop** | Report and dashboard creation |
| 📥 **CSV Dataset** | Source data |
| 🧹 **Power Query** | Data cleaning and type conversion |
| 📐 **Measures (Sum / Average)** | KPI calculations |
| 📈 **Bar Charts** | Sales and profit comparison |
| 🎛️ **Slicers** | Region and Category filters |
| 📋 **Table Visual** | Detailed order data |
| 🎨 **Formatting & Icons** | Dashboard design |

---

## 📈 Results & Insights

- ✅ **9,994-row dataset** loaded and modeled in Power BI
- 📌 **Four KPI cards** for sales, profit, quantity and discount
- 📊 **Sub-category and category views** show which products drive sales
- 🌍 **Regional profit view** highlights strong regions (West, East) and weak spots (Central in the selected view)
- 📉 Some orders with **high discounts (0.70–0.80)** show **negative profit** in the detail table
- 🎛️ **Slicers** make it easy to analyze any Region / Category combination
- 📋 **Detailed order table** helps trace individual orders

---

## 🏆 Advantages

| Advantage | Detail |
|-----------|--------|
| 🎓 **Beginner Friendly** | Shows a complete Power BI workflow from CSV to dashboard |
| 🎛️ **Interactive** | Region and Category slicers filter all visuals |
| 📊 **Visual** | KPI cards and charts make insights quick to read |
| 🔍 **Detailed** | Order-level table allows deeper investigation |
| 🔄 **Reusable** | Works with any Superstore-style sales dataset |
| 📚 **Portfolio Ready** | Clean structure with dataset, report and screenshots |

---

## 📄 License

This project is provided for **educational and portfolio purposes**.

You may adapt the report and documentation for your own learning or portfolio use, while keeping appropriate attribution for any source material you reuse.

---

## 👤 Author

<div align="center">

### Superstore Sales Analysis — Power BI Dashboard

> *"From raw rows to meaningful insights — one measure, one visual and one dashboard at a time."*

**👩‍💻 Author:** Yashvi Jasani  
**🎓 Project Type:** Power BI Data Analysis & Dashboard  
**📊 Focus:** Sales Performance, Profit Analysis & Visualization  
**🛠️ Skills:** Power BI · Power Query · Data Cleaning · KPI Measures · Slicers · Data Visualization · Dashboard Design

</div>

---

## 🙏 Acknowledgements

This project was developed using the Superstore sales dataset and Power BI Desktop.

Key Power BI concepts demonstrated in the project include:

- Data import and cleaning
- Date hierarchy
- KPI cards
- Bar charts
- Slicers
- Table visuals
- Dashboard layout and formatting

---

<div align="center">

---

*Made with ❤️ and 📊 — Last updated: 12 October, 2026*

</div>
