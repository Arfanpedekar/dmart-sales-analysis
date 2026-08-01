<div align="center">

# 🛒 D-Mart Sales Analysis

### An interactive Excel sales dashboard built with PivotTables, PivotCharts & Slicers

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/status-complete-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)

![Rows](https://img.shields.io/badge/rows-15%2C345-informational?style=flat-square)
![Sales](https://img.shields.io/badge/total%20sales-%2439.26M-success?style=flat-square)
![Profit](https://img.shields.io/badge/total%20profit-%246.87M-success?style=flat-square)
![Period](https://img.shields.io/badge/period-2023--2024-orange?style=flat-square)

</div>

<br>

<div align="center">

## 🖼️ Dashboard Preview

<img src="Dashboard.png" alt="D-Mart Sales Dashboard" width="100%">

</div>

<br>

## 📌 Overview

This project analyzes two years of **synthetic D-Mart retail sales data** (2023–2024) and turns it into a fully interactive, native-Excel dashboard — no Python, no Power BI, just PivotTables, PivotCharts, and slicers doing the heavy lifting.

The goal was simple: take a raw transactional dataset and build something a retail/business team could actually click through to answer questions like *"Which region is underperforming?"* or *"Are Members spending more than Regular customers?"*

<br>

## 📊 Key Metrics

<div align="center">

| 🧾 Orders | 💰 Sales | 📈 Profit | 📦 Units | 🎯 Avg Discount |
|:---:|:---:|:---:|:---:|:---:|
| **15,345** | **$39.26M** | **$6.87M** | **76,831** | **25.04%** |

</div>

<br>

## 🍩 Sales by Category

```mermaid
pie showData
    title Sales Distribution by Category ($)
    "Electronics" : 8017583
    "Home Care" : 7929347
    "Personal Care" : 7920394
    "Grocery" : 7718904
    "Clothing" : 7676650
```

<details>
<summary>📶 View as bar chart</summary>

```
Electronics     ████████████████████████ $8.02M
Home Care       ████████████████████████ $7.93M
Personal Care   ████████████████████████ $7.92M
Grocery         ███████████████████████  $7.72M
Clothing        ███████████████████████  $7.68M
```

</details>

Categories are remarkably balanced — no single category dominates, with **Electronics** edging out as the top performer.

<br>

## 🌍 Profit by Region

```
North   ████████████████████████ $1.77M
South   ███████████████████████  $1.71M
West    ███████████████████████  $1.71M
East    ███████████████████████  $1.68M
```

**North** leads in profitability, while **East** trails slightly — a ~5% spread across all four regions.

<br>

## 💳 Payment Mode & 👥 Customer Mix

<table>
<tr>
<td width="50%">

```mermaid
pie showData
    title Payment Mode
    "UPI" : 5136
    "Cash" : 5109
    "Card" : 5100
```

</td>
<td width="50%">

```mermaid
pie showData
    title Customer Type
    "New" : 5156
    "Regular" : 5144
    "Member" : 5045
```

</td>
</tr>
</table>

Both splits land almost perfectly evenly — roughly a **33/33/33** distribution across payment methods and customer segments.

<br>

## 🏙️ Top Cities by Sales

```
Chennai      ████████████████████████ $6.64M
Delhi        ████████████████████████ $6.61M
Bangalore    ████████████████████████ $6.60M
Mumbai       ████████████████████████ $6.56M
Hyderabad    ███████████████████████  $6.45M
Pune         ███████████████████████  $6.39M
```

<br>

## ⚙️ How It Was Built

```mermaid
flowchart TD
    A["🗂️ Raw Data<br>15,345 rows"] --> B["🧹 Data Cleaning<br>& Structuring"]
    B --> C["📊 PivotTables<br>region · category · customer · payment"]
    C --> D["📈 PivotCharts<br>visual trends & comparisons"]
    D --> E["🎛️ Slicers<br>interactive filtering"]
    E --> F["🖥️ Dashboard Sheet<br>single-view interactive report"]

    style A fill:#e8f5e9,stroke:#2e7d32
    style F fill:#2e7d32,stroke:#1b5e20,color:#fff
```

Everything was built **natively in Excel** — a deliberate choice to demonstrate core spreadsheet/BI fundamentals (PivotTables, calculated fields, chart design, slicer-based interactivity) without relying on external tooling.

<br>

## 🧰 Tech Stack

<div align="center">

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=flat-square&logo=microsoft-excel&logoColor=white)
![PivotTable](https://img.shields.io/badge/PivotTables-2E7D32?style=flat-square)
![PivotChart](https://img.shields.io/badge/PivotCharts-388E3C?style=flat-square)
![Slicers](https://img.shields.io/badge/Slicers-43A047?style=flat-square)

</div>

<br>

## 📁 Repository Structure

```
dmart-sales-analysis/
├── Dmart Sales Data.xlsx     # Full workbook — raw data, pivot table & dashboard
├── Dashboard.png             # Dashboard screenshot / preview
└── README.md                 # You are here
```

Inside the workbook:

| Sheet | Description |
|---|---|
| 🗂️ `Data` | 15,345 rows of raw transactional sales data |
| 📊 `Pivot Table` | Aggregated views (sales, profit, quantity) sliced by region, category, customer type, and payment mode |
| 🖥️ `Dashboard` | Interactive dashboard combining PivotCharts + Slicers into one view |

### Columns in the raw data

`order_id` · `region` · `category` · `sales` · `discount` · `net_sales` · `sales_volume` · `quantity` · `order_date` · `delivery_date` · `customer_type` · `payment_mode` · `profit` · `city`

<br>

## 🔍 What the Dashboard Lets You Explore

| | |
|---|---|
| 🌍 | **Regional performance** — compare sales & profit across North, South, East, and West |
| 🛍️ | **Category trends** — see which product categories drive the most revenue |
| 👥 | **Customer segments** — New vs Regular vs Member buying behavior |
| 💳 | **Payment preferences** — Cash vs Card vs UPI split |
| 🗓️ | **Time trends** — sales patterns across 2023–2024 |
| 🎛️ | **Live filtering** — slice everything instantly using the built-in slicers |

<br>

## 🚀 How to Use

1. 📥 Download `Dmart Sales Data.xlsx`
2. 📗 Open it in Microsoft Excel (2016 or later recommended for slicer support)
3. 🖥️ Head to the **Dashboard** sheet
4. 🎛️ Click any slicer button (region, category, customer type, etc.) to filter the entire dashboard live

<br>

## 🎯 Why This Project

This was built as part of a presentation on *"The Changing Role of a Data Analyst in the Age of GenAI"* — as a live, click-through demo showing that solid fundamentals (clean data + PivotTables + thoughtful dashboard design) are still at the core of good analysis, even as AI tools reshape the workflow around them.

> 📝 **Note:** The dataset is synthetic and was generated for practice/portfolio purposes — it does not represent real D-Mart sales figures.

---

<div align="center">

Built with 📊 in Excel · by **Arfan**

</div>
