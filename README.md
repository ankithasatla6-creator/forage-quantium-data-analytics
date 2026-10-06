# Quantium Data Analytics Virtual Experience

## 📌 Project Overview

This project was completed as part of the **Quantium Data Analytics Virtual Experience Program on Forage**.

The project focuses on analysing customer purchasing behaviour and evaluating the performance of selected trial stores using transaction data.

I worked on **two tasks** using Python, Pandas, data analysis, and visualisation techniques.

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualisation
* **Seaborn** – Exploratory visualisation
* **SciPy** – Statistical analysis
* **Jupyter Notebook**

---

## 📂 Project Structure

```text
Quantium-Data-Analytics/
│
├── Quantium_analysis1.ipynb
├── Quantium_analysis2.ipynb
└── README.md
```

---

# 📊 Task 1 – Customer Purchase Behaviour Analysis

The first task focused on preparing the transaction data and analysing customer purchasing behaviour.

### Dataset Used

The analysis used:

* `QVI_transaction_data.xlsx`
* `QVI_purchase_behaviour.csv`

### 🔹 Data Preparation

The transaction data was inspected and prepared for analysis.

The following steps were performed:

* Loaded the transaction dataset using Pandas.
* Loaded the customer purchase behaviour dataset.
* Inspected the available columns and data structure.
* Converted the transaction `DATE` column into a proper datetime format.
* Checked for missing values.
* Analysed product quantity information.
* Examined product names and their frequency.

### 🔹 Product Analysis

Additional information was extracted from the product names.

The analysis included:

* Extracting **pack size** from product names.
* Identifying product **brands**.
* Cleaning some brand names where the initial extraction did not represent the complete brand name.
* Analysing brand frequencies.
* Calculating total sales by brand.

### 🔹 Customer Data Integration

The transaction data was merged with the customer purchase behaviour data using:

```text
LYLTY_CARD_NBR
```

This allowed transaction information to be analysed together with customer characteristics.

### 🔹 Customer Segmentation

Customer purchasing behaviour was analysed using:

* **LIFESTAGE**
* **PREMIUM_CUSTOMER**

The analysis included:

* Counting customers across different lifestages.
* Examining premium customer categories.
* Calculating total sales for combinations of lifestage and premium customer type.
* Comparing sales across customer segments.

### 🔹 Visualisations

The analysis included visualisations such as:

* Total Sales by Brand
* Total Sales by Lifestage
* Total Sales by Premium Customer category

These visualisations helped identify differences in purchasing behaviour across customer groups.

### 💡 Key Learning

This task helped me understand how raw transaction data can be cleaned, combined with customer information, and analysed to identify meaningful purchasing patterns.

---

# 🏪 Task 2 – Trial Store Analysis

The second task focused on evaluating the performance of three trial stores:

* **Store 77**
* **Store 86**
* **Store 88**

The objective was to identify suitable control stores and compare their performance with the trial stores.

### Dataset Used

```text
QVI_data.csv
```

### 🔹 Data Preparation

The dataset was inspected for:

* Shape and columns
* Data types
* Missing values
* Store numbers
* Dates

The `DATE` column was converted into a monthly format using:

```text
YEAR_MONTH
```

### 🔹 Monthly Metrics

Monthly store-level metrics were calculated, including:

* **Total Sales**
* **Total Customers**
* **Total Transactions**
* **Transactions per Customer**
* **Chips per Customer**

These metrics were used to compare store performance over time.

---

## 🔍 Identifying Control Stores

The period before the trial was used to identify suitable control stores.

The analysis considered stores with complete pre-trial monthly data.

### Correlation Analysis

**Pearson correlation** was used to compare the trial stores with potential control stores.

Correlation was calculated for:

* Store 77
* Store 86
* Store 88

Higher correlation indicated that the store's sales pattern was more similar to the corresponding trial store.

### Magnitude Analysis

Correlation alone was not used.

A magnitude measure was also calculated to compare the sales levels of potential control stores with the trial stores.

The analysis considered stores with the complete seven-month pre-trial overlap.

This helped identify control stores that were both:

* Similar in sales pattern
* Similar in sales magnitude

### Selected Control Stores

Based on the analysis performed in the notebook:

| Trial Store | Selected Control Store |
| ----------- | ---------------------: |
| Store 77    |              Store 233 |
| Store 86    |              Store 155 |
| Store 88    |              Store 237 |

---

# 📈 Trial Period Analysis

After selecting the control stores, the trial period was analysed.

For each trial store:

1. Pre-trial sales were compared with the selected control store.
2. A **scaling factor** was calculated.
3. The control store's trial-period sales were scaled using that factor.
4. Trial-store sales were compared with scaled control-store sales.

This created a more meaningful comparison because the trial and control stores could have different sales levels before the trial began.

---

## 📊 Trial vs Control Visualisation

The final analysis included comparisons between:

* **Store 77 vs Scaled Store 233**
* **Store 86 vs Scaled Store 155**
* **Store 88 vs Scaled Store 237**

Line charts were used to compare the monthly sales of the trial stores with their scaled control stores during the trial period.

---

# 🧠 Skills Demonstrated

Through this project, I practised:

### Python & Data Analysis

* Data loading
* Data cleaning
* Data inspection
* Data transformation
* Data merging
* Grouping and aggregation
* Exploratory Data Analysis

### Pandas

* `read_csv()`
* `read_excel()`
* `groupby()`
* `merge()`
* Filtering
* Aggregation
* Date conversion
* Feature extraction

### Statistical Analysis

* Pearson correlation
* Control-store comparison
* Magnitude comparison
* Scaling-factor calculation

### Data Visualisation

* Bar charts
* Line charts
* Comparing trends across stores and customer segments

---

# 📚 Key Takeaways

This project gave me practical experience working with real-world style business datasets.

The main things I learned were:

* How to inspect and clean raw data before analysis.
* How to combine datasets using a common customer identifier.
* How customer segmentation can be used to understand purchasing behaviour.
* How to calculate and compare business metrics.
* How correlation can help identify similar stores.
* Why both **correlation and magnitude** are useful when selecting control stores.
* How scaling can make trial-store and control-store comparisons more meaningful.
* How to convert analysis into business-oriented insights.

---

# 🚀 Future Improvements

Possible improvements to this project include:

* Creating an interactive dashboard using Power BI or Tableau.
* Adding more detailed statistical analysis.
* Automating the control-store selection process.
* Adding additional customer and product-level analysis.
* Presenting the final business recommendations in a dashboard/report format.

---

# 🎓 Virtual Experience

**Quantium Data Analytics Virtual Experience Program**

Completed through **Forage**.

This virtual experience provided practical exposure to data preparation, customer analytics, statistical analysis, and business-focused decision making.

---

## 👤 Author

**Ankitha**

B.Tech – Computer Science and Data Science

### Interests

* Python
* Data Analytics
* Backend Development
* Artificial Intelligence
* Generative AI
