

# 📊 Mobile Price Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project presents a **complete Exploratory Data Analysis (EDA)** of a mobile phone dataset containing specifications such as **price, battery, display size, RAM, ROM, camera, ratings, reviews, brand, and warranty**.

The objective of this analysis is to understand:

* How different mobile specifications are distributed
* Which features influence mobile phone pricing
* How brands position their products across price segments

This project focuses on **data understanding and insights**, not model building.

---

## 🎯 Objectives

* Perform structured and systematic EDA
* Clean and transform real-world messy data
* Analyze feature distributions (univariate analysis)
* Study relationships between features and price (bivariate analysis)
* Validate findings using correlation analysis
* Draw meaningful, business-relevant insights

---

## 🗂️ Dataset Description

The dataset includes the following types of features:

* **Numeric:**
  Price, Rating, Battery Capacity, Display Size, RAM, ROM, Camera Megapixels, Reviews

* **Categorical:**
  Brand, Processor, Warranty

Some numeric features were initially stored as text due to units (e.g., `"5000 mAh"`, `"6.5 inches"`) and were cleaned during EDA.

---

## 🛠️ Tools & Libraries Used

* **Python**
* **Pandas** – data manipulation
* **NumPy** – numerical operations
* **Matplotlib & Seaborn** – data visualization
* **Jupyter Notebook** – analysis & documentation

---

## 🔍 EDA Workflow

### 1️⃣ Data Understanding

* Inspected dataset structure, columns, and data types
* Identified `price` as the primary variable of interest

---

### 2️⃣ Data Cleaning & Feature Extraction

* Handled missing values using logical, non-biased strategies
* Converted text-based numeric features into numeric format:

  * Battery → mAh
  * Display size → numeric
  * Reviews → numeric count
  * Memory → split into `RAM_GB` and `ROM_GB`
  * Camera → primary rear camera megapixels

---

### 3️⃣ Univariate Analysis

* Studied individual feature distributions
* Identified skewness patterns:

  * Price → Right-skewed
  * Rating → Left-skewed
  * Reviews → Highly right-skewed
  * Battery & Display → Near symmetric / left-skewed
  * RAM & ROM → Right-skewed

---

### 4️⃣ Bivariate Analysis

* Analyzed relationships using **price** as the anchor variable:

  * Price vs Battery
  * Price vs Display
  * Price vs Rating
  * Price vs RAM
  * Price vs ROM
  * Price vs Camera
  * Brand vs Price

Key insight:

* Hardware specs alone do not determine price.
* Higher specs allow **pricing flexibility**, not fixed pricing.

---

### 5️⃣ Correlation Analysis

* Used correlation heatmap to quantify relationships

**Key findings:**

* ROM shows the strongest positive correlation with price (~0.66)
* Display, camera, and rating show moderate correlation
* Battery shows weak correlation
* RAM and reviews show negligible linear correlation
* Brand plays a major role in explaining pricing outliers

---

## ✅ Key Insights

* **ROM (storage capacity)** is the strongest numeric predictor of price
* **Brand positioning** significantly impacts pricing
* High-end specs do not guarantee higher prices
* User ratings are largely independent of price
* Smartphone pricing is influenced by **multiple combined factors**, not a single feature

---

## 📁 Project Files

* `Mobile_Price_EDA_Full.ipynb` → Complete EDA notebook with explanations and code
* `README.md` → Project documentation

---

## 🚀 Future Work

* Feature encoding and scaling
* Price prediction using machine learning
* Feature selection or PCA
* Dashboard or interactive visualization

---

## 👤 Author

**Ashish Prajapati**
BCA Student | Aspiring Data Scientist / Python Developer

---

## 📌 Note

This project focuses on **EDA best practices** and analytical thinking.
It is suitable for:

* GitHub portfolio
* College projects
* Internship / job interviews

