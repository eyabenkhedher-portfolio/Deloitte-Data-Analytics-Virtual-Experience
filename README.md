# Deloitte Data Analytics Virtual Experience

This repository contains my solutions for the **Deloitte Data Analytics Virtual Experience Program** offered through Forage. The program simulates real-world data analytics projects, focusing on data visualization, condition logic, and forensic technology.

---

## 📂 Project Structure

### 🔹 Task 1: Telemetry Data Analysis & Troubleshooting (Tableau)
* **Goal:** Identify factories and machine types with the highest downtime (unhealthy status) using telemetry JSON data.
* **Tools Used:** Tableau Desktop
* **Key Steps:**
  1. Built a Calculated Field (`Unhealthy`) to convert `unhealthy` status logs into 10-minute downtime metrics (`IF [Status] = "unhealthy" THEN 10 ELSE 0 END`).
  2. Created interactive bar charts analyzing total downtime per factory and per device type.
  3. Integrated interactive filters in a unified Tableau Dashboard to isolate critical failure points.
* **Insights:** Isolated `daikibo-factory-seiko` as the primary downtime contributor, driven mainly by failures in `LaserWelder` and `LaserCutter` devices.

---

## 🔹 Task 2: Gender Pay Gap & Equality Classification (Excel)
* **Goal:** Classify employee compensation metrics into actionable equality categories.
* **Tools Used:** Microsoft Excel
* **Key Steps:**
  1. Applied absolute logic using `IF` and `ABS()` functions to categorize equality scores ($100$ to $-100$).
  2. Created the `Equality class` logic:
     * **Fair:** Score between $-10$ and $+10$
     * **Unfair:** Score between $-10$ and $-20$, or $+10$ and $+20$
     * **Highly Discriminative:** Score $< -20$ or $> +20$
* **Formula Used:** 
  `=IF(ABS(C2)<=10, "Fair", IF(ABS(C2)<=20, "Unfair", "Highly Discriminative"))`

---

## 🎖️ Certificate
Completed successfully and awarded the official **Deloitte Data Analytics Certificate**.
---

## 🔗 Project Resources & Outputs

* 📊 **Tableau Interactive Dashboard / Screenshot:** [View Dashboard Image](https://github.com/eyabenkhedher-portfolio/Deloitte-Data-Analytics-Virtual-Experience/blob/main/Deloitte_Data_Analytics_Dashboard.png)
* 📁 **Completed Excel Analysis:** [Download Equality Table_Completed.xlsx](https://github.com/eyabenkhedher-portfolio/Deloitte-Data-Analytics-Virtual-Experience/blob/main/Task%205%20Equality%20Table(Sheet1).csv)
* 📜 **Official Deloitte Certificate:** [Verify Certificate on LinkedIn](https://www.theforage.com/completion-certificates/9PBTqmSxAf6zZTseP/io9DzWKe3PTsiS6GG_9PBTqmSxAf6zZTseP_6a7de03600ad9dc2bfab9ef1_1786702650048_completion_certificate.pdf)
