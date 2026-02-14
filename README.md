# 🌐 Cloud Hosting Forecasting Engine

A recruiter‑ready FinOps portfolio project that simulates **multi‑cloud hosting spend (AWS + GCP)** and delivers end‑to‑end forecasting, scenario analysis, and variance dashboards. Built to demonstrate the deliverables expected of a **Senior FP&A / FinOps Manager** or **Principal Cloud Architect**.

---

## 📌 Elevator Pitch
**Translate raw billing into business impact.** Ingest simulated CUR data, clean and aggregate daily spend, train a Prophet forecasting model, run scenario simulations, and produce variance dashboards with prioritized optimization recommendations — all framed for hiring managers who need measurable cost control and forecasting leadership.

---

## 📂 Project Highlights
- **Data Simulation** — 30 days of multi‑cloud CUR data (AmazonEC2, AmazonS3, AmazonRDS, GCP Compute, GCP BigQuery).  
- **Preprocessing** — Automated cleaning and aggregation into daily spend totals.  
- **Forecasting** — Prophet model projecting 90 days forward from a 30‑day baseline.  
- **Scenario Analysis** — JSON‑driven configs for scale up, product launch, and contract commitments.  
- **Variance Dashboard** — Forecast vs actual visualizations and saved artifacts.  
- **Variance Report** — Recruiter‑ready interpretation and prioritized optimization recommendations.

---

## 📁 Repository Structure
- **data/**  
  - `cur_sample.csv` — 30 days simulated multi‑cloud CUR rows.  
  - `cur_clean.csv` — cleaned daily totals produced by preprocessing.  
- **scripts/**  
  - `preprocess.py` — load, clean, and aggregate raw CUR into daily totals.  
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

## 🚀 How to Evaluate Quickly
1. Inspect **data/cur_sample.csv** to review the multi‑cloud sample.  
2. Run `python scripts/preprocess.py` to generate **data/cur_clean.csv**.  
3. Open and run **notebooks/forecasting.ipynb** to train Prophet and export **reports/forecast.csv**.  
4. Run `python dashboards/variance_dashboard.py` to produce **reports/variance_chart.png**.  
5. Read **reports/variance_report.md** for business insights and recommended optimizations.

---

## ✨ Hiring Manager Hooks
- **Business impact statement** at the top showing expected cost base and forecast horizon.  
- **One‑line result** in `reports/variance_report.md` summarizing the top insight (for example, “Model overforecasted mid‑month by X%; reserved instance strategy could save Y% annually”).  
- **Demo assets**: include a 2‑minute screencast and a 1‑page PDF summary for quick review.  
- **Access control**: keep the full code in a private repo and publish demo artifacts publicly; offer private invites or live demos for technical interviews.

---

## 📣 Amplification Tips
- Add GitHub badges for Python, Prophet, AWS, and GCP.  
- Record a 2‑minute demo video walking through preprocessing → forecasting → variance dashboard and link it in the repo.  
- Post the variance chart and 3 key insights on LinkedIn with a short case summary.  
- Publish a short writeup on Medium describing the business impact and optimization recommendations.

---

## 🧭 Final Note
This repo is intentionally structured to demonstrate **technical execution**, **business judgment**, and **multi‑cloud FinOps leadership**. Paste this README into your GitHub root to present a polished, recruiter‑focused portfolio artifact.
