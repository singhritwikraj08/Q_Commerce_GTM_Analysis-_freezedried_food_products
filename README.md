# Q_Commerce_GTM_Analysis-_freezedried_food_products
# Omnichannel Pricing & Operations Strategy: E-Commerce vs. Quick Commerce

## 📌 Project Overview
This repository contains an end-to-end data science and operations research project designed to build a Go-To-Market (GTM) strategy for an FMCG brand (Hamps Bio). The project mathematically maps consumer purchasing behavior across traditional e-commerce (Amazon) and 10-minute Quick Commerce delivery platforms (Blinkit, Zepto). 

**Objective:** To define strict, data-backed manufacturing constraints (Weight, Maximum Retail Price, and Promotional Discount thresholds) to maximize per-unit profit margins and bypass algorithmically enforced "bulk penalties" on fast-delivery platforms.

---

## 🛠️ Tech Stack & Tools
* **Languages & Libraries:** Python (Pandas, NumPy, Scikit-Learn, XGBoost)
* **Unsupervised Learning:** K-Means Clustering, Normalized Euclidean Distance Mapping
* **Supervised Learning:** XGBoost Regressor, Decision Tree Classifier
* **Business Intelligence:** Power BI (Pareto Analysis, KPI Dashboards)

---

## 📊 Phase 1: Analytical Methodology & Key Findings

### 1. Market Segmentation & Omnichannel Matching
* **K-Means Clustering:** Segmented a highly saturated market dataset to find the optimal balance between mathematical separation (Silhouette Score) and business utility (Elbow Method), ultimately defining 4 distinct purchasing tiers.
* **Euclidean Distance Mapping:** Mathematically cross-referenced clusters between standard e-commerce and Q-Commerce platforms to eliminate human bias and identify exact cross-platform consumer overlaps.
* **Strategic Insight:** Identified a severe "Bulk Penalty" on Q-commerce where heavy items (>400g) require margin-destroying discounts (~42%) to sell. Consequently, bulk inventory must be routed exclusively to traditional e-commerce.

### 2. Operational Threshold Extraction (Decision Trees)
* Built a Decision Tree Classifier to transition from unsupervised clusters to hard, supervised logic rules.
* Extracted specific manufacturing constraints required to win the "Impulse Buy" market: **Weight ≤ 130g** and **Price ≤ ₹199**. These thresholds have been delivered to the procurement and packaging teams for upcoming production runs.

### 3. Demand Forecasting (XGBoost)
* Deployed an XGBoost Regressor to predict Amazon market velocity (Rating Counts) using Quick Commerce behavioral data.
* **Model Performance:** Achieved an **$R^2$ score of 82.04%** with an RMSE of 2594.80, successfully proving that future product market traction can be predicted with high accuracy based solely on configured weight and price combinations.

### 4. Demand Density & Product Prioritization (80/20 Rule)
* Built an executive Power BI Dashboard tracking ₹13.97L in total revenue.
* **Product Pareto:** Isolated the exact 20% of SKUs driving 80% of total revenue.
* **Geographic Pareto:** Filtered postal codes by >2 daily average orders to pinpoint high-profit, high-density delivery zones for the upcoming pilot launch.

---

## 🚀 Phase 2: Hyper-Local Pilot Launch (Next Steps)
Using the insights generated in Phase 1, Phase 2 will execute a Lean GTM market validation:
1. **Targeted Deployment:** Launching trial inventory strictly in the top 2-3 high-density postal codes identified in the Pareto analysis.
2. **Platform Sandbox:** Utilizing Amazon Same-Day and Flipkart Minutes to test the 130g/₹199 packaging thresholds in a live environment, bypassing the high entry barriers of dedicated Q-commerce dark stores.
3. **Data Acquisition:** Gathering empirical Customer Acquisition Cost (CAC) and true logistics overheads to calibrate the Phase 3 Pan-India scale-up.

---
