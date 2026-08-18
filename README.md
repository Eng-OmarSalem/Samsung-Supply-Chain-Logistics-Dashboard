[README.md](https://github.com/user-attachments/files/31187424/README.md)
<div align="center">

<img src="assets/dashboard-home.png" alt="Samsung Supply Chain & Logistics Dashboard" width="100%"/>

# 📱 Samsung Supply Chain & Logistics Dashboard

### End-to-End Power BI Analytics — From Raw Materials to the Customer's Door

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-4B5563?style=for-the-badge)
![Star Schema](https://img.shields.io/badge/Star%20Schema-Data%20Model-orange?style=for-the-badge)

</div>

---

## 📌 Overview

This project is a full **supply chain and logistics intelligence dashboard** built in **Power BI** for a Samsung Electronics business scenario. It follows a single product — from **supplier → production → inventory → shipment → sale** — and turns that journey into a connected, interactive story across six dedicated pages.

The model is built on a proper **star schema**: 5 dimension tables and 5 fact tables, so every KPI on every page slices cleanly by product, facility, supplier, customer, and date — with no duplicated logic and no broken relationships.

---

## 🖼️ Dashboard Preview

### 🏠 Home
A clean landing page with brand identity and navigation into every section of the report.

![Home Page](assets/dashboard-home.png)

### 👥 Customer
A deep dive into revenue performance, sold by channel and category.

![Customer Page](assets/dashboard-customer.png)

**Highlights from the Customer page:**

| Metric | Value |
|---|---|
| Gross Revenue | **186.86M** |
| Total Revenue | **176.95M** |
| Profit | **48.56M** |
| Profit Margin | **27.44%** |
| Perfect Order % | **75%** |
| Discount Amount | **9.92M** |

The page also breaks revenue down by **channel type** (Online, Retailer, Direct), by **product category** (Smartphone, Tablet, Television, Wearable, Appliance), and highlights the top-discounted products, month by month.

---

## 🧭 Report Pages

| Page | Focus |
|---|---|
| **Home** | Brand landing page & navigation |
| **Overview** | High-level KPIs across the entire supply chain |
| **Supplier** | Supplier performance, quality scores, and tiering |
| **Inventory** | Stock levels vs. safety stock and reorder points |
| **Shipment** | Carrier performance, delivery status, and delays |
| **Customer** | Revenue, profit, discounts, and channel performance |

---

## 🗃️ Data Model

Built as a star schema for fast, accurate cross-filtering across every page.

**Dimension tables**
| Table | Description |
|---|---|
| `dim_product` | 16 SKUs across Smartphones (Galaxy S & Z series), Tablets (Tab S & A), Televisions (Neo QLED, OLED, Crystal UHD), Appliances, and Wearables — with price, cost, weight, and image |
| `dim_customer` | Key accounts: Amazon.com, Best Buy, MediaMarkt Saturn, Flipkart, Samsung Direct Store — with channel type and annual volume |
| `dim_supplier` | 7 suppliers (Samsung Electronics, SK Hynix, TSMC, Sony Semiconductor, BOE Technology...) tiered as Tier 1 / Tier 2 with quality scores |
| `dim_facility` | Manufacturing plants (South Korea, Vietnam) and distribution warehouses (USA, Poland, India) with type, specialization, and capacity |
| `dim_date` | Full calendar table (2023 onward) with year, quarter, month, week, and weekend flags |

**Fact tables**
| Table | Description |
|---|---|
| `fact_procurement` | Purchase orders — quantity, unit cost, lead time, and delivered quality score |
| `fact_production` | Units produced per batch, defective units, and defect rate |
| `fact_inventory` | Stock level vs. safety stock level and reorder point, by product and facility |
| `fact_shipment` | Shipments by carrier, status, delay reason, shipping cost, and weight |
| `fact_sales` | Orders — quantity, discount, gross/net revenue, cost, profit, and profit margin |

---

## 🛠️ Tools & Techniques

- **Power BI Desktop** — data modeling, DAX measures, and report design
- **Star Schema Modeling** — 5 dimensions × 5 facts, connected on surrogate keys
- **DAX Measures** — revenue, profit margin, discount %, defect rate, perfect order %, and month-over-month growth
- **Power Query** — data shaping and relationship building from raw CSV extracts

---

## 🚀 How to Use

1. Download `Samsung_Dashboard.pbix` and all `dim_*.csv` / `fact_*.csv` files from this repository.
2. Open `Samsung_Dashboard.pbix` in **Power BI Desktop**.
3. If prompted, repoint the data source to the folder containing the CSV files on your machine.
4. Explore the six pages via the navigation bar on the Home page.

---

## 📬 Contact Me

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Eng-OmarSalem)
[![Portfolio](https://img.shields.io/badge/Portfolio-4B5563?style=for-the-badge)](https://gamma.app/docs/Copy-of-Brand-Partnership-Proposal-lrp9yrhau9gdpj1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/eng-omarsalem)

</div>

---

<div align="center">

Made with 📱 and Power BI

</div>
