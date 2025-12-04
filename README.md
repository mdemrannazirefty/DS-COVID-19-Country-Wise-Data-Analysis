# DS-COVID-19-Country-Wise-Data-Analysis

This project explores and analyzes global country-wise COVID-19 data using R.  
It covers the full workflow: cleaning, transforming, visualizing, and interpreting the dataset to uncover meaningful insights about how the pandemic affected different regions worldwide.

The dataset was sourced from Kaggle and includes key attributes such as confirmed cases, deaths, recoveries, active cases, weekly changes, WHO region, and mortality/recovery ratios.

---

## 📌 Project Goals

- Clean and prepare real-world COVID-19 data  
- Handle missing values (mean, median, mode)  
- Detect and correct outliers  
- Convert numerical attributes → categorical, and back  
- Normalize numeric variables  
- Balance the dataset  
- Visualize trends using ggplot2  
- Compute descriptive and comparative statistics  
- Explore mortality patterns across countries  

---

## 📊 Dataset Information

**Dataset Name:** COVID-19 Dataset  
**Rows:** 187  
**Columns:** 15  
**Source:** Kaggle  
🔗 https://www.kaggle.com/datasets/imdevskp/corona-virus-report

The dataset includes:

- Country / Region  
- Confirmed  
- Deaths  
- Recovered  
- Active  
- New Cases / New Deaths  
- Deaths per 100 Cases  
- Confirmed last week, Weekly change  
- WHO Region  

---

## 🧹 Data Cleaning Steps

- Replaced empty strings  
- Identified and fixed missing values  
- Removed incomplete rows  
- Checked for duplicates  
- Corrected invalid region values  
- Repaired negative values  
- Treated outliers using the IQR method  

---

## ⚙️ Feature Engineering

- Converted mortality ratio into Low / Medium / High categories  
- Mapped categories back to numeric codes (1, 2, 3)  
- Applied min–max normalization  
- Balanced the dataset using undersampling  

---

## 📈 Visualizations

- Missing value heatmap  
- Boxplot for outlier detection  
- Bar chart of the top 20 countries by total deaths  
- Group-wise trend plots  
- Statistical summary charts  

These visuals highlight global COVID-19 severity and the differences between country groups.

---

## 📐 Statistical Analysis

The project computes:

- Mean & Standard Deviation  
- Range, Variance, and IQR  
- Group-wise comparison of Confirmed, Deaths, Recovered, and Active cases  

Key insight:  
Countries with higher death rates (per 100 cases) generally reported significantly larger outbreaks.

---

## 📁 Project Structure
data-> 
country_wise_latest_update.csv

report-> 
Project_Report.pdf

scripts-> 
covid_analysis.R


---

## ▶️ How to Run the Project

### Install required libraries:
```r
install.packages("dplyr")
install.packages("ggplot2")
install.packages("naniar")
```

Load the dataset:
```r
mydata <- read.csv("data/country_wise_latest_update.csv", header = TRUE)
```

Run the analysis script:
```r
source("scripts/covid_analysis.R")
```

🧑‍💻 Author

Md. Emran Nazir Efty
📧 Email: mdemrannazirefty@gmail.com

🌐 Portfolio: [linkedin](https://www.linkedin.com/in/mdemrannazirefty/)]

🌐 GitHub: [mdemrannazirefty](https://github.com/mdemrannazirefty)]

📍 Dhaka, Bangladesh

📜 License

This project is open for educational and analytical use.

---








