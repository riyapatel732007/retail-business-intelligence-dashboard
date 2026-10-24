# 🛍️ Retail Business Intelligence Dashboard

A data analysis and business intelligence project that explores customer shopping behavior using Python, Pandas, and Microsoft Power BI.

## 📌 Project Overview

The Retail Business Intelligence Dashboard project focuses on analyzing customer shopping data through data cleaning, preprocessing, and feature engineering.

Python and Pandas are used to prepare the dataset, handle missing values, and create additional features for customer analysis. The processed dataset is saved as a CSV file and is available for use in the Power BI dashboard.

This project demonstrates how raw customer shopping data can be transformed into a structured dataset for business intelligence and data-driven decision-making.

## 🎯 Objectives

* Explore customer shopping behavior.
* Clean and preprocess the dataset.
* Identify and handle missing values.
* Standardize column names.
* Create customer age groups.
* Convert purchase frequency into numerical day intervals.
* Prepare a cleaned dataset for further analysis.
* Develop a Power BI dashboard for data visualization.

## 🛠️ Technologies Used

| Technology         | Purpose                                 |
| ------------------ | --------------------------------------- |
| Python             | Data processing and analysis            |
| Pandas             | Data cleaning and manipulation          |
| Jupyter Notebook   | Writing and executing Python code       |
| CSV                | Storing original and processed datasets |
| Microsoft Power BI | Dashboard development and visualization |

## 📂 Project Structure

```text
retail-business-intelligence-dashboard/
│
├── customer_shopping_behavior.csv
├── public customer.csv
├── Untitled.ipynb
├── pds_project_dashbord.pbix
└── README.md
```

## 📊 Dataset Description

The project uses a customer shopping behavior dataset containing information about customers, purchased products, spending, and shopping preferences.

The dataset includes fields such as:

* Customer ID
* Age and gender
* Item purchased
* Product category
* Purchase amount
* Location
* Product size and color
* Season
* Review rating
* Subscription status
* Shipping type
* Discount and promotional code usage
* Previous purchases
* Payment method
* Purchase frequency

## ⚙️ Data Cleaning and Preprocessing

The Python notebook performs the following operations:

### 1. Data Loading

Loads the customer shopping dataset into a Pandas DataFrame.

### 2. Data Exploration

Uses Pandas functions to inspect the dataset, examine column information, calculate descriptive statistics, and identify missing values.

### 3. Missing-Value Handling

Fills missing review ratings using the median review rating of the corresponding product category.

### 4. Column Name Standardization

Converts column names to lowercase and replaces spaces with underscores to simplify data manipulation.

### 5. Column Renaming

Renames the purchase amount column to `purchase_amount` for easier access.

### 6. Customer Age Group Segmentation

Creates an `age_group` feature using age-based quartile segmentation.

### 7. Purchase-Frequency Transformation

Maps purchase-frequency categories to numerical day intervals and stores the results in a new column named `purchase_frequency_days`.

### 8. Redundant Column Removal

Removes the `promo_code_used` column after comparing it with `discount_applied`.

### 9. Processed Dataset Export

Exports the cleaned and transformed dataset to `public customer.csv` for further analysis and visualization.

## 📈 Power BI Dashboard

The project includes a Power BI Desktop file:

**`pds_project_dashbord.pbix`**

Open this file in Microsoft Power BI Desktop to view the dashboard.

The processed customer dataset can be used to explore customer shopping patterns and present data through visual reports.

## 🚀 How to Run the Project

### Prerequisites

* Python 3
* Jupyter Notebook
* Pandas
* Microsoft Power BI Desktop

### Step 1: Clone the Repository

```bash
git clone https://github.com/riyapatel732007/retail-business-intelligence-dashboard.git
```

### Step 2: Open the Project Folder

```bash
cd retail-business-intelligence-dashboard
```

### Step 3: Install the Required Libraries

```bash
pip install pandas jupyter
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Untitled.ipynb` and execute the notebook cells in order.

**Note:** Ensure that the notebook uses the correct CSV file path. If both files are in the same directory, a relative path such as `pd.read_csv("customer_shopping_behavior.csv")` can be used.

### Step 5: Open the Power BI Dashboard

Open `pds_project_dashbord.pbix` using Microsoft Power BI Desktop.

## 💡 Key Learning Outcomes

* Data exploration using Pandas
* Missing-value handling
* Data cleaning and transformation
* Feature engineering
* Customer segmentation
* Categorical data transformation
* CSV file handling
* Preparing data for business intelligence reporting
* Power BI dashboard development

## 🔮 Future Enhancements

* Add more customer purchasing insights.
* Develop additional business performance indicators.
* Improve dashboard interactivity.
* Explore purchasing trends across product categories.
* Enhance customer segmentation and reporting.

## 👩‍💻 Author

**Riya Patel**

GitHub: [riyapatel732007](https://github.com/riyapatel732007)

---

*This project was developed for educational purposes to demonstrate data preprocessing and business intelligence reporting.*
