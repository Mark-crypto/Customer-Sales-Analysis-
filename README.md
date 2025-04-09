
# 📊 Customer Sales Analysis and Forecasting using R

This project provides a comprehensive approach to **data cleaning**, **exploratory data analysis (EDA)**, and **sales forecasting** using ARIMA models.
It is designed for analyzing customer sales data over time and predicting future sales trends using R.

---

## 📁 Dataset

The dataset used in this project is read from a local CSV file (`train.csv`). I have made it available in the repository. It includes sales-related data such as:

- `Order Date`
- `Ship Date`
- `Sales`
- `Category`
- `Region`
- `Customer ID`

> ⚠️ Ensure your CSV file path is correctly set in the script before running.

---

## 🛠️ Features & Workflow

### 1. **Library Installation and Setup**
```r
install.packages("forecast") # Install required package
library(ggplot2)
library(tidyverse)
library(readr)
library(forecast)
```

### 2. **Data Loading**
```r
sales_data <- read_csv("D:/Documents/train.csv")
```

### 3. **Data Exploration**
- Check dimensions and structure
- View column names and sample records
- Detect missing values

### 4. **Data Cleaning**
- Identify and remove incomplete rows
- Convert `Order Date` and `Ship Date` columns from character to `Date` format

### 5. **Exploratory Data Analysis (EDA)**
Includes visualizations like:
- **Boxplot**: Sales by Category
- **Line Chart**: Sales over Time
- **Bar Chart**: Top Selling Categories
- **Bar Chart**: Sales by Region
- **Line Chart**: Customer Purchase Frequency

### 6. **Forecasting**
- Convert the sales data to a time series object
- Fit an **ARIMA model** using `auto.arima()`
- Forecast sales for the next 12 months
- Visualize the forecast using `autoplot()`

---

## 📈 Sample Visuals

Here are some key visualizations generated:

- 📦 Sales per Product Category
- ⏳ Total Sales Over Time
- 🏆 Top Selling Categories
- 🌍 Sales by Region
- 👤 Customer Purchase Frequency
- 🔮 Sales Forecast (ARIMA)

---

## 🧪 Output

- Cleaned data saved to: `cleaned_customer_sales.csv`
- Visual insights and a 12-month sales forecast

---

## 💡 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Mark-crypto/sales-analysis-r.git
   cd sales-analysis-r
   ```

2. Open the `.R` or `.Rmd` file in RStudio

3. Make sure the path to `train.csv` is updated

4. Run each code chunk or Knit the R Markdown to generate the HTML report

---

## 📦 Requirements

Install the following R packages:

```r
install.packages(c("ggplot2", "tidyverse", "readr", "forecast"))
```
---

## 📬 Contact

For suggestions, questions, or collaborations, feel free to reach out via [GitHub Issues](https://github.com/Mark-crypto/Customer-Sales-Analysis/issues).

---
