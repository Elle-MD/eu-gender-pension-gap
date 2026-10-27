# 🇪🇺 Gender Pension Gap in the EU

**How does the gender pension gap vary across EU countries, and what can the data tell us about these differences?**

This exploratory data analysis project starts by examining the demographic profile of the EU's older population, before exploring gender differences in pension income across countries and over time.

The analysis draws on Eurostat data.

Follow the analysis on [LinkedIn](https://www.linkedin.com/in/elena-maria-d/?skipRedirect=true).

## 🔄 Current status

Work in progress — two stages completed.

### ✅ Completed

1. **Population by age group and sex (Eurostat demo_pjangroup)**

   - Retrieved, cleaned and explored Eurostat population data.
   - Examined the female population in older age groups, demographic trends and differences between EU countries.
   - Developed Power BI visualisations.

   *Notebooks: [population_data_familiarisation](01.demo_pjangroup_eu27_V2_familiarisation.ipynb); [population_data_cleaning](01.demo_pjangroup_eu27_V2_cleaning_process.ipynb); [population_data_analysis](01.demo_pjangroup_eu27_V2_analysis.ipynb)*

2. **Average and median gender pension gaps (Eurostat ilc_pnp13 & ilc_pnp13m)**

   - Retrieved and validated Eurostat average and median gender pension gap data for 2015–2025.
   - Compared the two indicators across all 27 EU Member States and the published EU-27 aggregate, focusing on people aged 65+.
   - Examined country rankings, differences between indicators and the evolution of the two measures in Spain.

   *Notebook: [Average and median gender pension gap analysis](02.ilc_pnp13_ilc_pnp13m_gender_pension_gaps_vp1.ipynb)*

## 🔍 Key findings so far

### Dataset 1: Population by age group and sex

The first stage explored the size and composition of the older female population in the EU, how it has evolved over time and differences between countries.

<img width="1207" height="701" alt="Main population indicators" src="https://github.com/user-attachments/assets/a748d14d-fb6c-4b0e-a1e4-91dabeb42ed0" />

*Figure 1: Main population indicators across EU-27*

<img width="1367" height="792" alt="Population trends by age category" src="https://github.com/user-attachments/assets/b83413fa-1703-4be5-b54d-8642226c27b0" />

*Figure 2: Gender gap trend by age category*

<img width="1382" height="792" alt="Population differences between countries" src="https://github.com/user-attachments/assets/6a6572f2-e526-4b7a-b429-985dc7094951" />

*Figure 3: Differences in female population aged 85+ by country*

### Datasets 2 and 3: Average and median gender pension gaps

In 2025, the EU-27 gender pension gap among people aged 65+ was **23.9% using the average** and **24.2% using the median**.

The two indicators generally show similar patterns, but important differences emerge:

- **10 of the 27 EU Member States** recorded differences exceeding 5 percentage points between their average and median pension gaps.
- The average gap was higher than the median in **19 countries**, while the median was higher in eight.
- Spain recorded the largest difference in 2025: **27.3% average versus 40.1% median**.
- Estonia recorded a slightly negative median gap (−0.9%), compared with a positive average gap (2.7%).

These findings highlight why examining both indicators can provide a more complete picture of gender pension inequality.

<img width="750" alt="Average and median gender pension gaps in 2025" src="https://github.com/user-attachments/assets/bd96b37f-1b46-4495-b67e-f584bdd5ebda" />

*Figure 4: Comparison of average and median gender pension gaps across EU countries, 2025.*

## 🛠️ Tools and methodology

Python is the main tool for data preparation, analysis and visualisation.

The demographic analysis began with CSV-based data retrieval and Power BI dashboards, including some experimentation with PostgreSQL. The pension gap analysis uses direct retrieval through the Eurostat API, with data validation and visualisations developed in Python.

## 📁 Data sources

- [Population by age group and sex (demo_pjangroup)](https://ec.europa.eu/eurostat/databrowser/view/demo_pjangroup/default/table)
- [Average gender pension gap by age group (ilc_pnp13)](https://ec.europa.eu/eurostat/databrowser/view/ilc_pnp13/default/table)
- [Median gender pension gap by age group (ilc_pnp13m)](https://ec.europa.eu/eurostat/databrowser/view/ilc_pnp13m/default/table)

## 🗂️ Next steps

- Examine trends in average and median gender pension gaps between 2015 and 2025, focusing on selected EU countries.
- Explore features of national pension systems relevant to women's retirement income for selected EU countries using OECD data.
