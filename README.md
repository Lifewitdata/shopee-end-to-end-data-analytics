<!-- Banner -->
<div align="center">

```
╔══════════════════════════════════════════════════════════════════════╗
║   🛒  SHOPEE × CUBE ASIA  —  E-COMMERCE EDA & TREND REPORT          ║
║   75,000+ SKUs · 4 Platforms · 2 Years · Python · Seaborn           ║
╚══════════════════════════════════════════════════════════════════════╝
```

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=flat-square&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C72B0?style=flat-square)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-34A853?style=flat-square)

</div>

---

## What This Is

Not another "I analyzed the Titanic dataset" project.

This is a full **e-commerce intelligence workflow** — the kind Cube Asia delivers to brand clients and private equity firms every week. Starting from raw, messy, multi-platform transaction data, this notebook surfaces the insights a brand CMO or category manager actually needs to make decisions.

> **Business question answered:** *"Which categories are growing, which platforms dominate, and where are the anomalies that signal fake reviews, rating manipulation, or viral campaign spikes?"*

---

## Dataset

| Field | Detail |
|---|---|
| **Rows** | 80,000 SKU-level transactions |
| **Period** | January 2023 – December 2024 |
| **Platforms** | Shopee, Lazada, TikTok Shop, Tokopedia |
| **Categories** | 8 (Fashion, Electronics, Beauty, FMCG, and more) |
| **Brands** | 20 leading SEA consumer brands |
| **Injected anomalies** | Rating drops (Jun–Jul 2023), review spikes (Electronics) |

> Data is synthetically generated to mirror real SEA e-commerce distribution patterns — price skew, review velocity, discount clustering, and seasonal GMV surges all reflect actual platform behavior.

---

## What the Notebook Does (15 Cells)

```
LOAD → AUDIT → CLEAN → DESCRIBE → VISUALIZE → DETECT ANOMALIES → INSIGHT
```

```
Cell 01  │  Import libraries + Cube Asia color palette
Cell 02  │  Load 80K rows — shape, date range, platform check
Cell 03  │  Schema & dtype audit
Cell 04  │  NULL analysis — bar chart, percentage breakdown
Cell 05  │  .describe() with Coefficient of Variation added
Cell 06  │  Price distribution — log scale + median by category
Cell 07  ⭐ Top categories by GMV — bar + pie chart
Cell 08  ⭐ Monthly GMV trend + seasonality heatmap
Cell 09  │  Platform breakdown — GMV, AOV, avg rating
Cell 10  ⭐ ANOMALY: Rating drops — Z-score detection, red dot flag
Cell 11  ⭐ ANOMALY: Review spikes — IQR method, boxplot
Cell 12  │  Correlation heatmap — all numeric features
Cell 13  │  Top 10 brands by GMV
Cell 14  │  Discount % vs units sold — sweet spot analysis
Cell 15  │  Client-ready insights summary table
```

---

## Key Findings

**🏆 Category GMV Ranking**
Fashion & Apparel leads (22% share) → Electronics spikes in Q4 only → Beauty consistent year-round

**📅 Seasonality**
GMV in November–December is **2.1× the monthly average** — driven by Shopee 11.11 and Lazada 12.12. Mid-year (Jun–Jul) is the weakest window.

**🚨 Anomalies Detected**
- **Rating drop** — Jun–Jul 2023 average rating fell below Z-score threshold of −1.5. Likely: product quality batch issue or platform review purge.
- **Review spikes** — 300+ Electronics SKUs exceeded IQR upper fence (Q3 + 3×IQR). Likely: viral TikTok content or boosted listings.

**🏷️ Discount Sweet Spot**
20–30% discounts maximize units sold. Beyond 50%, conversion drops — signals clearance inventory rather than demand-driven promos.

---

## Tech Stack

```python
pandas          # Data wrangling — 80K rows, multi-platform
numpy           # Outlier thresholds, Z-scores
matplotlib      # Custom multi-panel charts
seaborn         # Heatmaps, box plots, styled distributions
jupyter         # Cell-by-cell analyst workflow
```

---

## How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/shopee-eda-trend-report.git
cd shopee-eda-trend-report

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Launch notebook
jupyter notebook Shopee_EDA_Trend_Report.ipynb
```

---

## Folder Structure

```
shopee-eda-trend-report/
│
├── Shopee_EDA_Trend_Report.ipynb        ← Main notebook (run this)
├── shopee_ecommerce_data.csv            ← 80K row dataset
├── outputs/
│   ├── missing_values.png
│   ├── price_distribution.png
│   ├── gmv_by_category.png
│   ├── monthly_gmv_trend.png
│   ├── platform_analysis.png
│   ├── rating_anomaly.png
│   ├── review_spikes.png
│   ├── correlation_heatmap.png
│   ├── top_brands.png
│   └── discount_analysis.png
└── README.md
```

---

## Resume Bullet (Copy-Paste Ready)

> *Performed full EDA on 80,000+ SKU-level transactions across Shopee, Lazada, TikTok Shop, and Tokopedia — detecting rating anomalies via Z-score, review spikes via IQR, and seasonal GMV patterns that informed client promo calendars; visualized 10+ insight charts in Python (Pandas, Seaborn, Matplotlib).*

---

<div align="center">
<sub>Built as part of a Data Analyst portfolio targeting e-commerce intelligence roles in Southeast Asia.</sub>
</div>
