
# End-to-End Healthcare Data Science Pipeline: NTPF Ireland

![R](https://img.shields.io/badge/R-4.2+-blue.svg)
![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📌 Project Overview

**A complete Data Science workflow transforming raw waiting list data into actionable insights.**

This project analyzes outpatient waiting lists from the **National Treatment Purchase Fund (NTPF)** in Ireland (Jan - Aug 2025). The goal is to move beyond simple reporting and apply statistical rigor to detect operational bottlenecks, measure system volatility, and identify "stress points" in the healthcare system.

The pipeline spans from raw data ingestion and cleaning in **R**, through hypothesis testing, to a production-ready **Power BI** dashboard.

## 🚀 Key Features

* **Data Engineering (R/Tidyverse):** Robust cleaning pipeline, handling missing values, string manipulation, and type conversion for over 2.7M patient records.
* **Statistical Analysis:**
    * **Normality Testing:** Shapiro-Wilk tests on wait time distributions.
    * **Hypothesis Testing:** Welch Two Sample t-test (Adult vs. Child wait times) and Chi-squared tests for independence.
    * **Time Series Analysis:** Measuring "System Stress" (volatility) and monthly fluctuations.
* **Business Intelligence (Power BI):** Interactive dashboard allowing drill-down by specialty, age profile, and time bands.

## 📂 Repository Structure

```text
├── data/               # Raw and processed CSV files
│   └── OpenData_OPNational02_2025.csv
├── src/                # R Source codes and Quarto documents
│   └── Report.qmd      # Main analysis notebook
├── dashboard/          # Power BI files
│   └── Dashboard.pbix
├── output/             # Generated HTML/PDF reports and images
│   ├── Report.html
│   └── Report.pdf
└── README.md           # Project documentation

```

## 📊 Key Insights & Results

> *See `output/Report.html` for the full statistical breakdown.*

1. **Top Bottleneck:** **Orthopaedics** is the most critical specialty with the highest volume (536K+ patients) and high volatility.
2. **System Stress:** The system experienced peak stress in **July 2025** (+8.1K patient net increase), indicating a seasonal surge in demand or reduced capacity.
3. **Demographics:** Adult patients make up **54.5%** of the total volume.
4. **Statistical Significance:** Hypothesis testing confirmed a statistically significant difference in waiting list behaviors between Adult and Child cohorts ().

## 📸 Dashboard Preview

| Executive Overview | Volatility Analysis |
| --- | --- |
| <img src="output/screenshot_dashboard_1.png" width="400" alt="Dashboard Overview"> | <img src="output/screenshot_dashboard_2.png" width="400" alt="Volatility Charts"> |

*(Note: Screenshots are available in the `output/` folder)*

## 🛠️ Tech Stack

* **Language:** R (Quarto)
* **Libraries:** `tidyverse`, `janitor`, `ggplot2`, `scales`, `lubridate`
* **Visualization:** Power BI & ggplot2
* **Version Control:** Git & GitHub

## 💻 How to Run

1. **Clone the repository:**
```bash
git clone [https://github.com/your-username/ntpf-waiting-list-analysis.git](https://github.com/your-username/ntpf-waiting-list-analysis.git)

```


2. **R Analysis:**
* Open `src/Report.qmd` in RStudio.
* Ensure the `tidyverse` and `janitor` packages are installed.
* Render the file to generate the HTML report.


3. **Power BI:**
* Open `dashboard/Dashboard_HealthBeacon.pbix`.
* *Note: You may need to repoint the data source to the `/data` folder on your local machine if the path changes.*



## 👤 Author

**Iván Villar Naredo**

* [LinkedIn Profile](https://www.google.com/search?q=https://www.linkedin.com/in/ivan-villar-naredo/)
* [Portfolio](https://www.google.com/search?q=https://ivanvillarnaredo.com)

---

*Data Source: National Treatment Purchase Fund (NTPF) Open Data.*

```

```
