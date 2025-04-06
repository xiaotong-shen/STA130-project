# Wellspring Member Engagement Analysis

This project explores factors influencing member engagement at **Wellspring**, with a focus on user background characteristics (such as POC status and age), program interest, and the impact of a new registration system.

## 📊 Objective

Our goal is to answer three key questions:

1. **How do age and program interests influence average monthly attendance?**
2. **Does POC (Person of Color) status impact a member’s total service attendance?**
3. **Can registration date, mailing province, and cancer risk predict recent engagement?**

The target population is all potential and current Wellspring members in Canada, and the audience for this report is **Wellspring staff and program planners**.

---

## 🔍 Research Questions & Methodology

### 1. Age, Program Interests, and Attendance

- **Method:** Linear Regression  
- **Variables Used:** Age, program interest count, total services attended, join month/year  
- **Approach:**  
  - Categorized members by number of program interests  
  - Calculated average monthly attendance  
  - Built a linear model with age and program interest count as predictors

**Key Findings:**

- **Age:**
  - Older members (ages 30–80) attend more frequently.
  - Most attendance is clustered between 0–10 visits per month.
  
- **Program Interests:**
  - Members with 5–7 interests have the highest engagement.
  - Attendance sharply drops with fewer interests.
  - No program interest correlates with the lowest participation.

---

### 2. POC Status and Total Attendance

- **Method:** Randomization Test  
- **Variables Used:** Member ID, POC status, attendance records  
- **Hypotheses:**
  - H₀: POC status does not affect attendance.
  - H₁: POC status does affect attendance.

**Summary of Results:**

- **Boxplot & Histogram:**
  - Both POC and non-POC members have low median attendance.
  - High concentration of low-attendance users in both groups.
  - Outliers exist, but don’t affect the overall trend.
  
- **Statistical Results:**
  - **Test Statistic:** 1.716  
  - **P-Value:** 0.636  
  - **Conclusion:** No statistically significant difference in attendance based on POC status.

---

### 3. Predicting Engagement from Registration Info

- **Goal:** Predict whether a member attended any services in the past 3 months  
- **Variables Used:**  
  - Registration Date (pre-/post-March 2024)  
  - Mailing Province (East/West)  
  - Cancer Risk (High/Low)

- **Model Used:** Classification Tree  
- **Key Insights:**
  - **Registration date** is the most significant predictor.
  - Tree model had only one level — other predictors were not significant.
  - **Accuracy:** 82.5%

**Conclusion:**  
The **new registration system is effective**, strongly associated with recent engagement.

---

## ⚠️ Limitations

- **Demographic data** is incomplete — income, education, and cultural background were not considered.
- **POC status** is self-reported and may lack nuance.
- **Cancer-specific data** (type, stage) was excluded.
- **Geographic data** was generalized by region.
- **Statistical limitations:**
  - Linear regression assumes linearity.
  - Randomization test does not account for confounders.
  - Classification trees may miss variable interactions.

---

## ✅ Conclusions & Recommendations

- The **new registration system** boosted engagement, especially among:
  - Members aged 30–80  
  - Members with multiple program interests

- **Minimal impact** observed from:
  - POC status  
  - Cancer risk  
  - Mailing location

### Recommendations for Wellspring:

- Develop **targeted programs** for younger members.
- **Encourage multi-program participation** to boost engagement.
- Address broader barriers such as **accessibility** and **program relevance**.

---

## 📁 Files

This repository includes:
- `TUT0202-B-Final-Project.qmd` — Final Quarto report
- `Service_Deliveries.csv, Service_Deliveries.csv` - Data

---

## 👥 Contributors

- Xiaotong Shen  
- Carrie Lam  
- Danni Luo
- Xinyue Pu

---

## 📅 Project Timeline

- **Start Date:** March 16th, 2025
- **Completion Date:** April 4th, 2025
- **Institution:** University of Toronto

---

## 📌 Acknowledgments

Special thanks to Wellspring for providing the data and to our course instructors for their guidance.

