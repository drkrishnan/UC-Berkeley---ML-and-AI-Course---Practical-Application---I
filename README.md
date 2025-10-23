# Coupon Data Analysis Project

## Overview
This project performs a comprehensive analysis of coupon usage patterns from a dataset containing multiple coupon types. The analysis identifies acceptance rates for each coupon type and highlights characteristics of customers who are more likely to accept or reject coupons.

The workflow includes:
- Performing generic exploratory data analysis (EDA) on the dataset.
- Analyzing specific coupon types, including Bar coupons.
- Generating visualizations for acceptance vs rejection, overall coupon summaries, and heatmaps.

---

## 🛠 Code Functionality

1. **Exploratory Data Analysis**
   - Answers four generic questions about the dataset.
   - Generates two graphs:
     - `KR_number_of_coupons.png` – Distribution of coupon types.
     - `KR_temparature_distribution.png` – Distribution of temperature data.

2. **Coupon-specific Analysis**
   - Analyzes Bar coupons for six specific conditions.
   - Generates visualizations for each condition, saved in the `images` folder:
     - `KR_Bar_Acceptance_vs_Rejection.png` (example pattern for other coupons: `KR_<coupon name>_Acceptance_vs_Rejection.png`)
   - Coupon insights are manually generated and stored in "coupon_insights.json" in the configs folder . The insights are generated based on the result from EDA and individual coupon data analysis and used in visualizations.

3. **Overall Coupon Summary**
   - Generates a bar chart summarizing total acceptance rates for each coupon type:
     - `KR_Overall_Coupon_Summary.png`

4. **Acceptance Rate Heatmap**
   - Generates a heatmap summarizing acceptance rates across all coupon types:
     - `KR_Acceptance_Heatmap.png`

5. **Output Files**
   - Complete analysis results for all coupons are saved in:
     - `KR_PA1_coupon_data_analysis_output.txt` (delimited by `|`)

---

## 👥 Customer Insights

This analysis identifies general differences between customers who accepted coupons and those who did not:

- **Customers more likely to accept coupons:**
  - Visit the relevant establishments more frequently.
  - Are typically younger adults.
  - Travel without children.
  - Have occupations not tied to farming, fishing, or forestry.
  - Engage more often with restaurants or services targeted by the coupon.

- **Customers less likely to accept coupons:**
  - Visit the establishments infrequently.
  - May include very young or older adults.
  - Travel with children.
  - Have occupations in farming, fishing, or forestry.
  - Show lower engagement with the targeted services or establishments.

These patterns help understand **which customer groups respond positively to different types of coupons**, providing insights for marketing strategies.

---

## 📂 File Structure

├── data/
│ └── KR_PA1_coupon_data_analysis_output.txt
├── images/
│ ├── KR_<coupon_name>_Acceptance_vs_Rejection.png
│ ├── KR_number_of_coupons.png
│ ├── KR_temparature_distribution.png
│ ├── KR_Overall_Coupon_Summary.png
│ └── KR_Acceptance_Heatmap.png
├── configs/
│ └── coupon_insights.json
├── module_5_practical_application_1.ipynb
└── README.md