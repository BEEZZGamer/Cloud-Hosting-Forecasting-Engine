# 🌐 Cloud Hosting Forecasting Engine

A recruiter‑ready FinOps project that simulates **multi‑cloud hosting spend (AWS + GCP)** and delivers end‑to‑end forecasting, scenario analysis, and variance dashboards. This repo is designed to showcase the exact deliverables expected of a **Senior FP&A / FinOps Manager** or **Principal Cloud Architect**.

---

## 📂 Project Highlights
- **Data Simulation:** 30 days of AWS + GCP CUR data (AmazonEC2, AmazonS3, AmazonRDS, GCP Compute, GCP BigQuery).  
- **Preprocessing:** Automated cleaning and aggregation into daily spend totals.  
- **Forecasting:** Prophet model projecting 90 days forward.  
- **Scenario Analysis:** JSON‑driven configs for scale up, product launch, and contract commitments.  
- **Variance Dashboard:** Forecast vs actual spend with recruiter‑ready charts and saved artifacts.  
- **Variance Report:** Business insights and optimization recommendations framed for hiring managers.

---

## 🚀 Deliverables
- **Forecasting accuracy** — Quantify deviations between forecast and actuals.  
- **Scenario planning** — Model growth, launches, and savings commitments.  
- **Variance analysis** — Identify drivers of spend volatility across AWS and GCP.  
- **Optimization insights** — Recommend actions (reserved instances, storage tiering, query optimization) that reduce variance by ~15%.

---

## 💡 Strategic Value
This repo mirrors responsibilities in senior cloud finance and FinOps roles:
- **Technical mastery** with time series forecasting, data engineering, and visualization.  
- **Business framing** that translates technical outputs into cost optimization and ROI.  
- **Multi‑cloud readiness** showing hybrid AWS + GCP spend analysis.  

Recruiters will see evidence you can own forecasting, scenario planning, and variance reporting end‑to‑end.

---

## 📊 Simulated Spend
- **Baseline:** Scaled example representing ~$10M hosting costs.  
- **Forecast horizon:** 90 days forward from the observed 30‑day sample.  
- **Services covered:** AmazonEC2; AmazonS3; AmazonRDS; GCP Compute; GCP BigQuery.

---

## 📁 Repository Structure
- **data/**  
  - `cur_sample.csv` — 30 days simulated CUR rows.  
  - `cur_clean.csv` — cleaned daily totals produced by preprocessing.  
- **scripts/**  
  - `preprocess.py` — load, clean, aggregate raw CUR into daily totals.  
- **notebooks/**  
  - `forecasting.ipynb` — Prophet training, forecasting, and export to `reports/forecast.csv`.  
- **scenarios/**  
  - `scenario_config.json` — scenario parameters: scale_up, product_launch, contract_commitment.  
- **dashboards/**  
  - `variance_dashboard.py` — merges forecast vs actual, computes variance, saves chart.  
- **reports/**  
  - `forecast.csv` — forecasted values with confidence intervals.  
  - `variance_chart.png` — saved visualization.  
  - `variance_report.md` — recruiter‑ready interpretation and recommendations.

---

## ✅ How to Evaluate This Project Quickly
1. Open `data/cur_sample.csv` to inspect the multi‑cloud sample.  
2. Run `scripts/preprocess.py` to generate `data/cur_clean.csv`.  
3. Open `notebooks/forecasting.ipynb`, run cells to train Prophet and export `reports/forecast.csv`.  
4. Run `dashboards/variance_dashboard.py` to produce `reports/variance_chart.png`.  
5. Read `reports/variance_report.md` for business insights and recommended optimizations.

---

## 📣 Amplification Tips
- Add GitHub badges for Python, Prophet, AWS, and GCP.  
- Record a 2‑minute demo video walking through preprocessing → forecasting → variance dashboard.  
- Post the variance chart and 3 key insights on LinkedIn with a short case summary.  
- Publish a short writeup on Medium describing the business impact and optimization recommendations.

---

## 🧭 Final Note
This repo is intentionally structured to demonstrate **technical execution**, **business judgment**, and **multi‑cloud FinOps leadership**. Paste this README into your GitHub root to present a polished, recruiter‑focused portfolio artifact.
