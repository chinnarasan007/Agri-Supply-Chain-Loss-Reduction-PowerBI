# 🌾 Agri Supply Chain Loss Reduction Dashboard

> A unified Power BI analytics platform to identify, quantify, and reduce post-harvest agricultural losses across India's supply chain.

---

## 📌 Problem Statement

India is the world's second-largest food producer, yet loses an estimated **₹92,000 Crore worth of agricultural produce annually** due to post-harvest inefficiencies. Despite record harvests, a significant portion of food never reaches the consumer — it rots in farms, spoils in transit, deteriorates in poorly maintained warehouses, or gets rejected at markets.

**The core challenge is not production — it is preservation, logistics, and market access.**

Agricultural stakeholders operate in **information silos** with no unified visibility into:
- **Where** losses are happening (state, district, supply chain stage)
- **What** is being lost (crop, category, cause)
- **Why** losses occur (cold chain gaps, poor roads, bad packaging, pest attacks)
- **How much** it costs (loss value in ₹ Crore)
- **Which interventions** are working (program effectiveness vs. budget spent)

---

## 💡 The Solution

The **Agri Supply Chain Loss Reduction Dashboard** is a multi-dimensional Power BI platform integrating data from **6 operational sources**:

| Data Source | Description |
|---|---|
| Supply Chain Transactions | Loss records by crop, stage, state, and cause |
| Warehouse Infrastructure | Condition, capacity & utilization of 300 warehouses |
| Transport & Logistics | Vehicle type, road condition, packaging impact |
| Market Price Trends | MSP → Wholesale → Retail price chain by crop |
| Farmer Profiles | Demographics, certifications, market channels |
| Government Intervention Programs | 200 schemes with budget, beneficiaries & outcomes |

---

## 🎯 Primary Objective

> **To reduce post-harvest agricultural losses by enabling data-driven decisions at every level of the supply chain — from farm gate to consumer plate.**

---

## 📊 Dashboard Pages

| Page | Title | Key Insight |
|---|---|---|
| 1 | Cold Chain Gap Analysis | Loss 22.15% without cold chain vs. 13.67% with — 8.49% gap |
| 2 | Crop & Stage Loss Breakdown | Fruits (1,260K MT) and Vegetables (1,019K MT) lose the most |
| 3 | Warehouse Infrastructure | 111 of 300 warehouses are Poor/Dilapidated; 99 below 40% utilization |
| 4 | Transport & Logistics | Poor rural roads cause 963.6 loss units; bamboo baskets 53% worse than PP bags |
| 5 | Market Price Intelligence | Black Pepper: farmer gets only 45.7% of consumer price |
| 6 | Government Intervention Effectiveness | Training programs deliver 26.8% loss reduction vs. 20.9% for infrastructure |

---

## 📁 Repository Structure

```
agri-supply-chain-loss-reduction/
│
├── 📊 Dashboard/
│   └── Agri_Supply_Chain_Dashboard.pbix                          
│
├── 📂 Dataset/
│   └── Agri_Supply_Chain_Loss_Reduction.xlsx  
├── 📄 Documentation/
│   └── Power_BI_Problem_Statement.docx       
│
├── 📸 Screenshots/                           
│   ├── page1_cold_chain.png
│   ├── page2_crops_stages.png
│   ├── page3_infrastructure.png
│   ├── page4_transport.png
│   ├── page5_market_prices.png
│   └── page6_interventions.png
│
└── README.md
```

---

## 📂 Dataset Overview

**File:** `Agri_Supply_Chain_Loss_Reduction.xlsx`

The dataset contains **5,000+ supply chain records** across India (2020–2023) with the following fields:

| Field | Description |
|---|---|
| `Record_ID` | Unique transaction identifier |
| `Date / Year / Quarter` | Temporal dimensions |
| `State / District` | Geographic dimensions |
| `Crop / Crop_Category` | 30+ crops across Grains, Fruits, Vegetables, Spices, Cash Crops |
| `Stage` | Supply chain stage (Harvesting → Transport → Storage → Retail) |
| `Production_Qty_MT` | Total production in metric tons |
| `Loss_Qty_MT` | Loss quantity in metric tons |
| `Loss_Percentage` | Percentage loss at that stage |
| `Loss_Value_INR` | Monetary value of loss in INR |
| `Cause_of_Loss` | Root cause (e.g., Moisture & Rot, Road Condition, Lack of Cold Chain) |
| `Storage_Type` | FCI Warehouse, Cold Storage, Open Yard, NABARD Warehouse, etc. |
| `Transport_Mode` | Road-Truck, Rail-Goods, Water Barge, etc. |
| `Cold_Chain_Available` | Yes / No |
| `Market_Channel` | APMC Mandi, E-NAM, Direct to Retailer, Export, FPO/Cooperative |
| `Market_Price_INR_per_MT` | Prevailing market price |
| `MSP_INR_per_MT` | Minimum Support Price |

---

## 🧑‍💼 Use Cases

### 🔴 Use Case 1 — Government Policy Maker
*"Where should we invest next year's cold chain budget?"*

The dashboard's Cold Chain Gap Analysis and State Loss Map help the Ministry allocate ₹500 Crore optimally. Bihar and Andhra Pradesh + Fruits/Vegetables is the highest-priority combination — projected to save **₹800+ Crore annually**.

---

### 🔴 Use Case 2 — Warehouse Infrastructure Planner
*"Which warehouses are failing and where do we need new ones?"*

Page 3 reveals 111 poor/dilapidated warehouses and 99 underutilized ones. **No new construction needed** — renovating existing + incentivizing utilization solves the problem.

---

### 🔴 Use Case 3 — Logistics & Transport Company
*"How do we reduce transit losses?"*

Switching from Bamboo Baskets to PP Bags alone yields a **53% loss reduction** with zero infrastructure cost. Poor rural roads cause 17% more loss than national highways.

---

### 🔴 Use Case 4 — FPO / Farmer Producer Organization
*"Which crops and market channels give the best return?"*

E-NAM and Direct-to-Retailer channels have consistently lower losses than Contract Farming. Harvesting + Transport stages account for **40%+ of all losses** — prime intervention points.

---

### 🔴 Use Case 5 — Government Scheme Monitoring
*"Are intervention programs actually reducing losses?"*

Training programs deliver **26.8% loss reduction** with modest budget, while Infrastructure programs spend more (₹13,163 Cr) but achieve only **20.9%** — lowest efficiency. 53 programs are currently Paused.

---

### 🔴 Use Case 6 — APMC Market Intelligence
*"Are farmers getting a fair price?"*

Black Pepper: Retail ₹83,601/MT vs. MSP ₹38,197 — **farmer receives only 45.7% of consumer price**. The dashboard instantly highlights which crops have excessive middleman margins.

---

## 🏆 Expected Outcomes

| Outcome | Current → Target |
|---|---|
| Post-harvest loss % | 19.51% → below 12% |
| Cold chain coverage | 31.1% → 60%+ |
| Annual monetary savings | — → ₹3,000–4,000 Crore |
| Warehouse utilization | avg 57% → 80%+ |
| Farmer income increase | — → 15–20% |
| Program efficiency | — → 30% more beneficiaries per crore |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard development & publishing |
| **Microsoft Excel** | Data source (`.xlsx`) |
| **DAX** | Custom measures and KPIs |
| **Power Query** | Data transformation & modeling |

---

## 🚀 How to Use

1. **(https://github.com/chinnarasan007/Agri-Supply-Chain-Loss-Reduction-PowerBI) or download** this repository
2. Open **`Dataset/Agri_Supply_Chain_Loss_Reduction.xlsx`** to explore the raw data
3. Open **`Dashboard/Agri_Supply_Chain_Dashboard.pbix`** in **Power BI Desktop** (free download from Microsoft)
4. The dashboard will automatically load with all 6 pages
5. Use **slicers** (State, Crop, Year, Season) to filter and explore
6. Use **cross-filtering** — clicking any visual filters all others on the page

> 💡 **Tip:** Power BI Desktop is free. Download from [microsoft.com/power-bi](https://powerbi.microsoft.com/desktop/)

---

## 📸 Dashboard Screenshots

> *(Add screenshots of each dashboard page here after export from Power BI)*

| Page | Preview |
|---|---|
| Cold Chain Analysis | *(screenshot)* |
| Crop & Stage Breakdown | *(screenshot)* |
| Warehouse Infrastructure | *(screenshot)* |
| Transport Analysis | *(screenshot)* |
| Market Prices | *(screenshot)* |
| Intervention Effectiveness | *(screenshot)* |

---

## 👤 Author

**Chinnarajan M** — Aspiring Data Scientist
---

## 📜 License

This project is for educational and portfolio purposes.
Dataset is synthetically generated for analysis and visualization practice.

---

## ⭐ If you found this useful, give the repo a star!
