# 🩺 Smoking Health Risk Analysis Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C94C?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-00758F?style=for-the-badge)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-00599C?style=for-the-badge)

An interactive Power BI healthcare analytics dashboard designed to evaluate, visualize, and communicate the multi-organ health impacts of smoking relative to patient demographics, cholesterol levels, and blood pressure risks.

---

## 📌 Project Overview

The **Smoking Health Risk Analysis** project provides a comprehensive healthcare analytics solution exploring how tobacco usage affects major human organ systems (Heart, Lungs, Liver, Kidneys, and Full Body). 

By combining clinical indicators (Blood Pressure Risk, Cholesterol Levels, BMI) with lifestyle metrics (Smoking Status, Cigarettes Per Day, Years of Smoking), this dashboard allows healthcare professionals and researchers to interactively analyze physiological risk profiles.

---

## 🎯 Business & Healthcare Problem

Medical analysts and healthcare providers often evaluate patient risk factors in isolation. However, tobacco exposure impacts multiple organ systems simultaneously and non-linearly across different age groups and genders. 

Without interactive data modeling, it is difficult to isolate the exact relationship between smoking intensity (Cigarettes Per Day), exposure duration (Years of Smoking), and concrete physiological damage across specific vital organs. This dashboard bridges that gap by offering an intuitive, visual diagnostic tool.

---

## 🎯 Project Objectives

- **Demographic Profiling:** Monitor average patient age, BMI, and gender distributions relative to smoking habits.
- **Exposure Analysis:** Track the correlation between smoking intensity (CPD) and duration (YOD) across age brackets.
- **Organ-Specific Assessment:** Provide interactive visual filtering across vital organs (Heart, Lungs, Kidney, Liver, and Full Body).
- **Condition Toggling:** Allow seamless comparison between **Healthy** and **Damaged** organ states.
- **Cardiovascular & Metabolic Risk:** Analyze the distribution of cholesterol levels and Blood Pressure (BP) risk classifications.

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop:** Dashboard engineering, user interface design, visual bookmarks, and slicers.
- **DAX (Data Analysis Expressions):** Dynamic measures for aggregate calculations (`DISTINCTCOUNT`, `AVERAGE`, conditional metrics).
- **Power Query:** Data extraction, transformation, normalization, and handling missing values.
- **Data Modeling:** Star schema modeling connecting patient demographics, lifestyle factors, and clinical organ assessments.

---

## 🖥️ Dashboard Architecture & Interactive Features

### 1. Dynamic Organ Navigation Panel
* **Side Slicer Bar:** Interactive navigation icons allowing stakeholders to isolate metrics specifically for the **Heart**, **Human Body**, **Kidney**, **Liver**, or **Lungs**.

### 2. Physiological Condition Toggle
* **Healthy vs. Damaged Slicer:** Dedicated toggle at the top of the canvas to switch the central visual and metric cards between healthy organ baselines and damaged pathological states.

### 3. Key Visual Modules
* **KPI Metrics:** Real-time summary cards displaying Total Patients, Average Age, and Average BMI.
* **Smoking Status (Donut Chart):** Cohort proportions across *Never*, *Current*, and *Former* smokers.
* **Smoking Status by Gender (Stream/Area Graph):** Gender-based distribution of smoking history.
* **Intensity vs. Duration (Line Chart):** Dual-axis analysis tracking Average Cigarettes Per Day (CPD) vs. Average Years of Smoking (YOD) by Age Group (10–30, 31–50, 51–100).
* **Cholesterol & BP Risk (Stacked Bar Chart):** Cholesterol volume segmented across age groups and sub-divided by Blood Pressure risk levels (*High*, *Low*, *Normal*).

---

## 🔍 Analytical Workflow

1. **Data Collection & Schema Design:** Loaded raw healthcare data containing patient IDs, demographics, lifestyle markers, and organ assessment diagnostics.
2. **Data Cleansing (Power Query):** Cleaned data fields, handled missing clinical values, and standardized age groupings (`10-30`, `31-50`, `51-100`).
3. **Data Modeling:** Structured relationships between patient demographic tables and organ diagnostic fact tables.
4. **DAX Development:** Created dynamic measures for cohort counts, average exposure levels, and conditional dashboard formatting.
5. **UI/UX Design:** Implemented a dark medical-grade visual background, intuitive icon navigation, and dynamic image state switching.

---

## 📈 Key Insights & Findings

* **Demographic Baseline:** The patient cohort exhibits an average age of **51–58 years** with an average BMI of **29–30** across organ views.
* **Smoking Habit Distribution:** Across all patient groups, approximately **40% are Former Smokers**, **30% are Current Smokers**, and **30% are Non-Smokers**.
* **Intensity vs. Duration Crossover:** Younger patients (10–30) exhibit higher daily smoking intensity (CPD), whereas older cohorts (51–100) record significantly longer smoking duration (YOD). The 31–50 age range represents the key crossover period for cumulative risk.
* **Organ Vulnerability:** When isolating **Damaged** organ states, the **Lungs** and **Heart** record the highest proportion of damaged patient entries among long-term smokers.
* **Cardiovascular Co-morbidity:** High Blood Pressure risk accounts for over **30%** of patients across all age brackets, heavily compounding cardiovascular risk in current and former smokers.

---

## 💡 Recommendations & Clinical Value

- **Targeted Early Intervention:** Prioritize smoking cessation programs for patients in the **31–50 age group** before cumulative exposure (YOD) transitions into irreversible organ degradation.
- **Dual-Risk Screening:** Patients flagged with high smoking duration should automatically undergo combined cardiovascular (BP/Cholesterol) and pulmonary evaluations.
- **Former Smoker Monitoring:** Because former smokers still represent a large percentage of damaged organ cases, post-cessation clinical tracking must remain active long-term.

---

## ⚠️ Limitations

- **Observational Data:** The observed correlations between smoking intensity and organ damage identify risk patterns but do not replace direct medical clinical diagnosis.
- **Dataset Scope:** Findings depend on the completeness, sample size, and recording accuracy of the underlying dataset.

---

## 🏁 Conclusion

This project demonstrates how Microsoft Power BI can convert complex medical and lifestyle data into an interactive, visually engaging BI solution. By providing dynamic organ filtering and condition toggling, the dashboard equips medical analysts with clear evidence to support data-informed healthcare strategies.
