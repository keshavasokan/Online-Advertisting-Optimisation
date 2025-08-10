# Online Advertising Optimization

**Data-Driven Budget Allocation for High-Street Fashion Retail Campaigns**  

---

## 🚀 Project Overview

This project demonstrates a complete **data analytics and optimization workflow** for maximizing the impact of an online advertising campaign.  
Starting from raw keyword-level historical data, it builds predictive models, formulates optimization problems, and delivers actionable budget allocation strategies.  

The workflow is designed for **real-world marketing analytics**, providing insights that are directly translatable into improved campaign ROI.

---

## ✨ Key Features

* **End-to-End Analysis**: From raw data exploration to optimization and recommendation generation.
* **Insight-Driven Flow**: Each stage builds on the previous, connecting data patterns to modeling and optimization decisions.
* **Predictive Modeling**: Uses linear regression to estimate CPC per keyword.
* **Optimization Engine**: Implements linear programming to allocate budget for maximum clicks.
* **Scenario Testing**: Runs diversification and sensitivity analyses to stress-test recommendations.
* **Revenue Lens**: Extends optimization from clicks to net profitability.
* **Advanced CPC Modeling**: Supports piecewise CPC curves to capture diminishing returns.

---

## 🛠️ Tech Stack

* **Python** (3.8+)
* **Pandas / Numpy**
* **Matplotlib / Seaborn**
* **scikit-learn**
* **Gurobi** (for optimization)
* **Jupyter Notebook** (analysis and reporting)

> *See `requirements.txt` for details*

---

## 🧑‍💻 How It Works

### 1. Data Exploration
* Load and inspect keyword-level ad campaign data.
* Compute and visualize CPC distributions by keyword.
* Identify trends in budget vs. clicks to spot diminishing returns.

### 2. Predictive Modeling ([Notebook](Online_Advertising_Optimization_professional.ipynb))
* Fit zero-intercept linear regression models for each keyword.
* Validate predictions against exploratory data insights.
* Build a CPC lookup table for optimization.

### 3. Budget Optimization
* Formulate a **Linear Program** to maximize clicks given budget constraints.
* Explore diversification constraints to avoid over-reliance on one keyword.
* Perform sensitivity analysis on CPC and total budget.

### 4. Revenue Optimization
* Extend the model to maximize net revenue rather than clicks.
* Identify optimal spend and break-even points.

### 5. Advanced Extension
* Introduce **piecewise CPC functions** to handle non-linear CPC behavior.
* Compare allocations under linear vs. piecewise models.

---

## 📈 Sample Insights

* **Lowest CPC Keyword:** “retail UK” emerged as the most cost-effective term.
* **Optimization Result:** Without diversification constraints, budget concentrated on cheapest CPC terms; with constraints, spend was more evenly spread.
* **Revenue Perspective:** The profit-maximizing budget was significantly below the total available spend.
* **Sensitivity:** Small changes in CPC for top keywords could materially shift optimal allocations.

---

## 🚦 Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook Online_Advertising_Optimization_professional.ipynb
