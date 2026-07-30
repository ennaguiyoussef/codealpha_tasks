# 📉 Unemployment Rate Analysis in India

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-green?logo=pandas)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-purple?logo=plotly)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualizations-red)
![License](https://img.shields.io/badge/License-MIT-yellow)

> A comprehensive data analysis project exploring unemployment trends, regional disparities, and the economic impact of the COVID-19 lockdown in India up to November 2020.

---

## 🎥 Video Presentation

Watch the video below for a complete walkthrough of the project, from data cleaning to interactive visualizations!

👉 **[![Watch the video](https://img.youtube.com/vi/HrC9OkcZiNw/maxresdefault.jpg)](https://youtu.be/HrC9OkcZiNw?si=vdFMVXQlMtNiaaR3)**

---

## 📖 About the Project

The objective of this project is to analyze unemployment rate data across different regions and zones in India. By leveraging data visualization techniques, this project aims to:
- Understand overall unemployment and labor participation trends.
- Explore the severe economic impact of the **COVID-19 pandemic and lockdowns**.
- Identify seasonal and monthly patterns in employment.
- Generate actionable insights to support economic and social policy decisions.

---

## 📊 The Dataset

The dataset contains **267 records** tracking economic indicators across various Indian regions up to November 2020. 

| Feature | Description |
| :--- | :--- |
| `region` | Name of the specific state/region |
| `date` | Date of the record (Converted to datetime) |
| `frequency` | Frequency of data collection (e.g., M for Monthly) |
| `unemployment_rate` | **Estimated Unemployment Rate (%)** |
| `estimated_employed` | Number of estimated employed citizens |
| `labour_participation_rate` | **Estimated Labour Participation Rate (%)** |
| `zone` | Geographical zone of the region (e.g., North, South) |
| `longitude` & `latitude` | Geographic coordinates for spatial mapping |

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas & NumPy**: For data manipulation, cleaning, and aggregation.
- **Matplotlib & Seaborn**: For static statistical visualizations.
- **Plotly (Express & Graph Objects)**: For creating advanced **interactive and animated** visualizations.
- **Jupyter Notebook**: For interactive development and documentation.

---

## 🚀 Project Workflow

### 1. Data Cleaning & Preparation
- Checked for duplicates and missing values (Dataset was clean).
- Standardized column names for easier access (e.g., `Estimated Unemployment Rate(%)` $\rightarrow$ `unemployment_rate`).
- Converted the `date` column to a `datetime` object.
- Engineered new features: Extracted `month_nb` (numeric month) and `month` (abbreviated month name) to analyze seasonal trends.

### 2. Exploratory Data Analysis (EDA) & Visualizations
The core of this project relies on rich, interactive visualizations to uncover hidden patterns:

- **Monthly Trends:** Grouped bar charts comparing average monthly *Unemployment Rates* vs. *Labour Participation Rates*.
- **Employment Volume:** Bar plots showing the average estimated employed citizens month-by-month.
- **Regional Disparities:** Box plots and bar charts to analyze the distribution and average unemployment rates across different states.
- **Zone-wise Analysis:** Categorized states into broader geographical zones (North, South, East, West, etc.) to compare macro-level economic health.
- **Advanced Interactive Charts:**
  - 🗺️ **Animated Geo-Scatter Plot:** Mapped the impact of the lockdown on employment across India's geography over time.
  - 🌞 **Sunburst Chart:** Visualized the hierarchical relationship between Zones, Regions, and their respective unemployment rates.
  - 📊 **Scatter Matrix:** Explored the correlation between unemployment, estimated employed, and labor participation rates.

---

## 💡 Key Insights

* **Lockdown Impact:** The data visualizations clearly show a massive spike in unemployment during April and May 2020 due to the COVID-19 lockdown.
* **Regional Variations:** The charts prove that the economic shock affected states differently. For example, Haryana and Tripura experienced the highest unemployment rates, highlighting severe regional vulnerabilities.
* **Labour Participation:** When unemployment went up, the labour participation rate significantly dropped. This indicates that millions of people completely stopped looking for work during the pandemic.

---

## 💻 How to Run This Project

1. Clone this repository:
   ```bash
   git clone https://github.com/ennaguiyoussef/codealpha_tasks.git
   cd unemployment_analysis