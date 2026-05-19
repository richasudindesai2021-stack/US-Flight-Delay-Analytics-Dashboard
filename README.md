# ✈️ U.S. Flight Delay & Cancellation Analytics Dashboard

An interactive analytics dashboard built to explore U.S. domestic flight performance data, visualizing on-time rates, delays, and cancellations across airlines, airports, and time periods.

![Dashboard Preview](https://drive.google.com/uc?export=view&id=1utK76RCTdn9WWI0wNTPv1B7z6D1X-okE)

---

## 📊 Overview

This project analyzes **2 million+** U.S. domestic flights to uncover patterns in delays and cancellations. The dashboard provides a high-level summary of flight performance and allows exploration across multiple dimensions — airline, city, day of week, and cancellation reason.

### Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Flights | ~2M |
| On-Time Rate | 58% |
| Delayed Rate | 41% |
| Cancellation Rate | 1% |

---

## 📁 Dataset

The dataset consists of five CSV files:

| File | Description | Available |
|---|---|---|
| `flights.csv` | Core flight records — departure/arrival times, delays, cancellation flags, airline codes, origin/destination airports | [Download from Google Drive](https://drive.google.com/file/d/1Y-ACoLPmcrP_xqpdSW1_ZqyGGlnTJAZw/view?usp=sharing) |
| `airlines.csv` | Airline IATA codes mapped to full carrier names | Included in repo |
| `airports.csv` | Airport codes mapped to city, state, and coordinates | Included in repo |
| `cancellation_codes.csv` | Cancellation reason codes (Weather, Airline/Carrier, National Air System, Security) | Included in repo |

> ⚠️ `flights.csv` is too large to host on GitHub (~500MB, 2M+ rows). Download it from the Google Drive link above and place it in the `/data` folder before opening the dashboard.

**Source:** U.S. domestic flights (2015), originally published on [Kaggle](https://www.kaggle.com/datasets/usdot/flight-delays).

---

## 📈 Dashboard Highlights

### Top-Level KPIs
- Total flights, delayed flights, and canceled flights — each with a monthly trend sparkline

### Charts & Visuals
- **Total Flights by City** — Horizontal bar chart ranking the top 10 busiest departure cities (Atlanta leads)
- **% Delayed by Airline** — Comparison of delay rates across all major U.S. carriers
- **Canceled Flights by Cancellation Reason** — Donut chart breaking down weather vs. carrier vs. system vs. security causes
- **% Canceled by Day of Week** — Bar chart revealing which days see the most cancellations
- **Total Flights by Status** — Stacked bar showing the overall split between On-Time, Delayed, and Canceled flights

---

## 🛠️ Tools Used

- **Data Visualization:** Power BI Desktop
- **Data:** CSV files (no database required)

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/richasudindesai2021-stack/US-Flight-Delay-Analytics-Dashboard.git
   cd US-Flight-Delay-Analytics-Dashboard
   ```

2. Download `flights.csv` from [Google Drive](https://drive.google.com/file/d/1Y-ACoLPmcrP_xqpdSW1_ZqyGGlnTJAZw/view?usp=sharing) and place it in the `/data` folder.

3. Open `power bi/power_bi.pbix` in Power BI Desktop.

4. Refresh and explore.

---

## 💡 Key Insights

- **Atlanta, Chicago, and Dallas-Fort Worth** are the busiest departure cities by total flight volume.
- **United Airlines and Southwest** have among the highest delay rates by percentage.
- **Weather** is the leading cause of cancellations (~57%), followed by National Air System issues (~28%).
- **Monday (Day 2)** and **Sunday (Day 7)** show the highest cancellation rates by day of week.

---

## 📂 Repository Structure

```
flight-delay-dashboard/
│
├── data/
│   ├── [flights.csv](https://drive.google.com/file/d/1Y-ACoLPmcrP_xqpdSW1_ZqyGGlnTJAZw/view?usp=sharing)              # Too large for GitHub — 📁 click to view in Drive
│   ├── airlines.csv
│   ├── airports.csv
│   └── cancellation_codes.csv
│
├── power bi/
│   └── power_bi.pbix            # Power BI dashboard — open with Power BI Desktop
│
├── dashboard_preview.png
└── README.md
```

---

## 📄 License

This project is for educational and portfolio purposes. Dataset credit: [U.S. DOT / Kaggle](https://www.kaggle.com/datasets/usdot/flight-delays).
