# 🎬 Movie Box Office Insights  

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)  
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)  
![Pandas](https://img.shields.io/badge/Pandas-EDA-green)  
![License](https://img.shields.io/badge/License-MIT-lightgrey)  

> Data-driven insights for launching a new movie studio 🚀  

---

## 📑 Table of Contents  
- [📌 Project Overview](#-project-overview)  
- [🗂️ Data Sources](#️-data-sources)  
- [🛠️ Methods](#️-methods)  
- [📊 Key Visualizations](#-key-visualizations)  
- [✅ Business Recommendations](#-business-recommendations)  
- [📂 Deliverables](#-deliverables)  
- [🚀 Next Steps](#-next-steps)  

---

## 📌 Project Overview  
This project explores **movie performance at the box office** using data from multiple sources:  
- **Box Office Mojo (BOM)**  
- **The Numbers (TN)**  
- **IMDb**  

The company wants to launch its **own movie studio**, but lacks insights into what makes films financially and critically successful. This analysis provides **data-driven recommendations** on which types of films to produce.  

---

## 🗂️ Data Sources  
- **Box Office Mojo (`bom.movie_gross.csv`)**  
  - Domestic & foreign gross revenues for ~3,300 films.  
- **The Numbers (`tn.movie_budgets.csv`)**  
  - Production budgets, worldwide & domestic gross for ~5,700 films.  
- **IMDb (`im.db`)**  
  - SQLite database with movie basics (title, year, genre) and ratings.  

---

## 🛠️ Methods  
1. **Data Cleaning & Preparation**  
   - Normalized titles, years, and genres for merging.  
   - Converted financials (`$425,000,000`) into numeric values.  
   - Created **derived features**:  
     - `profit = worldwide_gross - production_budget`  
     - `ROI = profit / production_budget`  

2. **Exploratory Data Analysis (EDA)**  
   - Top-grossing and most profitable films.  
   - ROI and profit trends over time.  
   - Genre-based profitability analysis.  
   - Impact of IMDb ratings and votes on financial success.  

3. **Linear Regression Models**  
   - **Budget → Revenue/Profit** (Do bigger budgets pay off?)  
   - **Budget + Ratings → ROI** (Quality + investment influence returns)  
   - **Genre + Budget → ROI** (Which genres yield better margins?)  
   - **Year Trends** (How profitability has shifted over time)  

---

## 📊 Key Visualizations  
- 📈 Top 10 most profitable movies.  
- 📉 ROI trends across years.  
- 🎭 Genre comparison by ROI and profit margin.  
- 🔗 Scatterplots of **budget vs. revenue/profit** with regression fits.  

---

## ✅ Business Recommendations  
Based on analysis:  
1. **Mid-budget films (~$30M–$80M)** often yield higher ROI than mega-budget blockbusters.  
2. **Certain genres (e.g., Horror, Animation)** deliver strong profitability relative to budget.  
3. **Quality matters** — higher IMDb ratings correlate with stronger financial success.  

---

## 📂 Deliverables  
- 📓 **Jupyter Notebook (`student.ipynb`)**: Full code, cleaning, EDA, regression.  
- 🖼️ **Presentation (`presentation.pdf`)**: Non-technical summary for stakeholders.  
- 📘 **README.md** (this file): Project documentation.  

---

## 🚀 Next Steps  
- Expand analysis with Rotten Tomatoes & TMDB datasets.  
- Build predictive models (e.g., Random Forest, Gradient Boosting) for profitability.  
- Scrape recent box office data for fresher insights.  

---

👩‍💻 *Developed as part of an Exploratory Data Analysis (EDA) project.*  
