# Meta Ad Performance Analysis | Power BI

An interactive Power BI dashboard developed to analyze paid advertising performance across Facebook and Instagram. The dashboard provides insights into campaign reach, engagement, conversions, audience demographics, geographic performance, time-based trends, and ad-type performance.


---

## 🎯 Business Objective

The objective of this project is to develop a performance tracking dashboard for Facebook and Instagram advertising campaigns.

The dashboard enables marketing teams to:

* Monitor campaign reach and engagement
* Analyze conversion performance
* Compare Facebook and Instagram performance
* Understand audience engagement patterns
* Analyze ad performance by demographic and geographic segments
* Identify trends across time
* Support data-driven budget allocation decisions

---

## 📌 Key KPIs

The dashboard tracks the following key performance indicators:

| KPI                      | Description                                      |
| ------------------------ | ------------------------------------------------ |
| Impressions              | Number of times advertisements were displayed    |
| Clicks                   | Number of users who clicked advertisements       |
| Shares                   | Number of times advertisements were shared       |
| Comments                 | Number of user comments                          |
| Purchases                | Number of purchases attributed to advertisements |
| Engagements              | Clicks + Shares + Comments                       |
| CTR                      | Clicks ÷ Impressions × 100                       |
| Engagement Rate          | Engagements ÷ Impressions × 100                  |
| Conversion Rate          | Purchases ÷ Clicks × 100                         |
| Purchase Rate            | Purchases ÷ Impressions × 100                    |
| Total Budget             | Total campaign budget                            |
| Avg. Budget per Campaign | Total Budget ÷ Campaign Count                    |

---

## 📈 Dashboard Features

### 1. Audience Analysis

* Target Gender — Donut Chart
* Target Age Group — Bar Chart
* Dynamic metric selection

These visuals help identify audience segments contributing to selected performance metrics.

### 2. Geographic Analysis

A country-level map visualizes advertising performance geographically, allowing campaign performance to be explored across different markets.

### 3. Time-Based Analysis

The dashboard includes:

* Calendar heat map
* Weekly performance trends
* Hourly engagement trends

These visuals help identify periods of higher and lower advertising activity.

### 4. Ad Type Analysis

A matrix compares performance across different advertising formats and platforms.

Ad types include:

* Image
* Video
* Carousel
* Stories

### 5. Interactive Analysis

The dashboard uses interactive filtering and dynamic metric selection to allow users to explore campaign performance from different perspectives.

---

## 🗂️ Data Model

The dataset follows a **star schema** consisting of one fact table and multiple dimension tables.

```text
                    ┌──────────────┐
                    │  campaigns   │
                    └──────┬───────┘
                           │
                           │
┌──────────────┐     ┌─────▼──────┐     ┌──────────────┐
│     ads      │────►│ ad_events  │◄────│    users     │
└──────────────┘     └────────────┘     └──────────────┘
```

### Fact Table

**ad_events**

Contains event-level advertising interactions such as:

* Impression
* Click
* Share
* Comment
* Purchase

### Dimension Tables

**ads**

Contains:

* Ad platform
* Ad type
* Target gender
* Target age group
* Target interests
* Campaign ID

**campaigns**

Contains:

* Campaign name
* Start date
* End date
* Campaign duration
* Total budget

**users**

Contains:

* Gender
* Age
* Age group
* Country
* Location
* Interests

---

## 🔍 Key Findings

Based on the dashboard analysis:

* The campaigns generated approximately **216K impressions** and **25.4K clicks**.
* The overall CTR was approximately **11.76%**.
* Approximately **1.3K purchases** were recorded.
* The purchase rate was approximately **0.61%**, indicating a larger drop-off toward the conversion stage.
* Engagement was concentrated among younger audience segments.
* Advertising activity showed stronger engagement during afternoon and evening hours.
* Video and Stories formats showed strong engagement and conversion-related metrics within the analyzed dataset.
* Performance varied across geographic markets and audience segments.


---

## 💡 Business Recommendations

Based on the observed patterns in the dataset:

1. Investigate the conversion funnel to understand the gap between clicks and purchases.
2. Analyze landing-page and offer performance to identify potential conversion barriers.
3. Further evaluate audience segments with higher engagement and conversion rates.
4. Compare advertising formats based on both engagement and conversion metrics before reallocating budget.
5. Use time-based performance patterns to inform campaign scheduling.
6. Monitor geographic performance when evaluating future campaign targeting and budget allocation.

---

## 🛠️ Tools & Technologies

* **Power BI**
* **DAX**
* **Power Query**
* **Data Modeling**
* **Star Schema**
* **Data Visualization**
* **Business Intelligence**
* **KPI Development**
* **Interactive Dashboard Design**

---

## 👩‍💻 Author

**Imasha Buddhini**

