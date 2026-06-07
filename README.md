# Airbnb Rental Price Prediction


---

## Project Overview

This project builds a **machine learning model to predict nightly rental prices for Airbnb listings**. 

**Dataset:** 74,111 Airbnb listings across 6 US cities (NYC, San Francisco, Los Angeles, Boston, Washington DC, Chicago)

**Features:** 29 original features including location, room type, amenities, reviews, and host information

**Objective:** Demonstrate a complete, production-ready data science workflow from data exploration to model evaluation

**Best Model:** Gradient Boosting
- **R² Score:** 0.5384 (explains ~54% of price variance)
- **RMSE:** $55.27 (average prediction error)
- **MAE:** $39.30 (typical error)

---

##  Files Included

### **Core Project Files**

| File | Type | Size | Purpose |
|------|------|------|---------|
| `airbnb_rental_price.ipynb` | Jupyter Notebook | 
| `Airbnb_Data.csv` | Dataset | 74,111 listings × 29 features |
| `Nowshin_ML_Project_Presentation.pptx` | Presentation slide |
| `README.md` | Documentation | Instructions |

---

##  Quick Start Guide

### **Step 1: Check Python Version**

Ensure you have Python 3.8 or higher:

```bash
python --version
```
---

### **Step 2: Install Required Libraries**

Run this command to install all dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**What each library does:**
- **pandas** - Load and manipulate data (CSV files)
- **numpy** - Numerical computations and arrays
- **matplotlib** - Create charts and visualizations
- **seaborn** - Enhanced statistical graphics
- **scikit-learn** - Machine learning algorithms
- **jupyter** - Run interactive notebooks

---

### **Step 3: Navigate to Project Folder**

```

Make sure `Airbnb_Data.csv` and `airbnb_rental_price.ipynb` are in this directory.

---

### **Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook airbnb_rental_price.ipynb
```
---

### **Step 5: Run All Cells**

In the Jupyter interface:
1. Click **Kernel** menu
2. Select **Restart & Run All Cells**
3. Wait for execution

---

### **Step 6: Verify Success**

The notebook will display:

✅ **Data Loading**
```
Dataset shape: (74111, 29)
```

✅ **Data Exploration**
```
Missing Values: [list of columns with nulls]
Price Statistics: mean, std, min, max
```

✅ **Visualizations**
- Price distribution histogram
- Box plot showing outliers

✅ **Data Cleaning Results**
```
Remaining rows: 70,411 (after outlier removal)
Price range: $1.00 - $425.00
```

✅ **Model Training**
```
Linear Regression: R² = 0.4987, RMSE = $57.61, MAE = $41.34
Random Forest: R² = 0.5285, RMSE = $55.87, MAE = $39.53
Gradient Boosting: R² = 0.5384, RMSE = $55.27, MAE = $39.30
```

✅ **Feature Importance**
- Top 10 features visualization
- Bar chart of importance scores

---

### **Software Required**
- **Python:** 3.8+
- **IDE:** VS Code, PyCharm (for code editing)
- **Jupyter Lab:** Enhanced notebook interface

---

## Key Project Results

### **Best Model: Gradient Boosting**

| Metric | Value | Interpretation |
|--------|-------|-----------------|
| **R² Score** | 0.5384 | Explains 54% of price variance |
| **RMSE** | $55.27 | Average prediction error |
| **MAE** | $39.30 | Typical error magnitude |

### **Dataset Summary**

| Aspect | Value |
|--------|-------|
| Original Listings | 74,111 |
| After Cleaning | 70,411 |
| Features Used | 28 |
| Price Range | $1 - $425 |
| Cities | 6 (NYC, SF, LA, Boston, DC, Chicago) |

### **Top Price Drivers**

(From feature importance analysis in notebook)

1. Number of bedrooms
2. Room type (Entire home vs Private/Shared)
3. Guest capacity (accommodates)
4. Comfort Score
5. City location

---

Both `airbnb_rental_price.ipynb` and `Airbnb_Data.csv` must be in the same folder.

---

### **Issue: Notebook runs very slowly or hangs**

**Solution:** 
- Close other applications to free RAM
- Reduce dataset size temporarily for testing
- Ensure you have at least 4 GB RAM available

---

### **Issue: "No module named 'jupyter'"**

**Solution:** Install Jupyter
```bash
pip install jupyter
```

Or launch notebook directly from Python:
```python
import notebook
notebook.notebookapp.main(['airbnb_rental_price.ipynb'])
```

---

## Understanding the Output


### **Feature Importance Output**
Top 10 features shown with importance scores (how much each influences predictions).

---
