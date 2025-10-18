# 🥗 **Healthy Eating Meal Data Analysis**

---

## 📘 **Project Overview**
This project provides a **comprehensive statistical analysis** of a healthy eating meal dataset (**Healthy_Eating.csv**) to identify the **key nutritional drivers of customer satisfaction (Rating)** and establish **data-driven strategies** for menu optimization.

The analysis goes beyond basic descriptive statistics, applying **Multiple Linear Regression** and **ANOVA** to convert raw nutritional data into **actionable business insights**.

---

## 🎯 **Key Strategic Conclusions**

### 🧬 **1. Protein-First Strategy is Paramount**
- **Protein** and **Fiber** are the strongest positive and statistically significant predictors of higher customer satisfaction.
- Focus on **increasing these two macro-nutrients** in recipe development to directly enhance ratings.

### 🍱 **2. Cuisine-Specific Calorie Benchmarking**
- The analysis found that **calorie content varies significantly by cuisine** (e.g., *Indian vs. Mexican*).
- This supports **abandoning a single calorie target** across cuisines and adopting **cuisine-specific calorie standards** for competitive meal design.

---

## ⚙️ **Methodology and Analysis Pipeline**

The project follows a **rigorous three-stage process**, fully encapsulated in the script  
`complete_healthy_eating_analysis.py`.

### **1️⃣ Data Cleansing and Preparation**
- **Missing Data Imputation:** Replaced missing numerical values with the **median** of each column.  
- **Outlier Removal:** Used the **Interquartile Range (IQR)** method to remove outliers in *calories*, *protein_g*, and *fat_g*.  
- **Data Standardization:** Cleaned and standardized categorical columns (*cuisine*, *diet_type*).

### **2️⃣ Statistical Analysis**
- **Multiple Linear Regression:** Quantified the effect (coefficient) and significance (P-value) of nutritional variables — *protein_g*, *fat_g*, *sugar_g*, and *fiber_g* — on **Rating**.  
- **ANOVA (Analysis of Variance):** Tested the hypothesis that **mean calorie content differs across cuisine types**.

### **3️⃣ Data Visualization**
Three main plots summarize the key findings:
- 📊 **Distribution of Meal Ratings**  
- 🥑 **Average Nutritional Content (Calories, Protein, Fat) by Diet Type**  
- 🍜 **Box Plot of Calorie Distribution Across Cuisines** (supports ANOVA results)

---

## 📂 **Project Structure and Files**

| **File Name** | **Type** | **Description** |
|----------------|-----------|-----------------|
| `Healthy_Eating.csv` | Data | Raw dataset containing meal info, nutritional values, and ratings. |
| `complete_healthy_eating_analysis.py` | Python Script | Core script for loading, cleaning, analyzing, and visualizing data. |
| `project_summary.md` | Report | Summary of objectives, methodology, and strategic insights. |
| `README.md` | Documentation | Main project documentation file. |

---

## 🧠 **How to Run the Analysis**

### **Requirements**
This analysis requires **Python 3.x** and the following libraries:

```bash
pandas
numpy
matplotlib
seaborn
scipy
statsmodels
Execution Steps
Ensure Healthy_Eating.csv is located in the same directory as the Python script.

Run the main analysis script from your terminal:

bash
Copy code
python complete_healthy_eating_analysis.py
Output
The script will generate:

🧾 Data cleansing logs and descriptive statistics

📈 ANOVA and Regression results (R-squared, coefficients, P-values)

🧩 Final strategic conclusion summary

📊 Three visualization windows displaying the analytical results

🏁 Conclusion
This project demonstrates how statistical modeling can drive nutritional optimization and menu innovation in the healthy eating industry.
By focusing on Protein and Fiber while using cuisine-specific calorie benchmarks, organizations can align menu design with customer satisfaction and competitive positioning.
