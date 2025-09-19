# insurance
README.md
# Insurance Dataset Analysis

## 📌 Project Overview
This project analyzes the **Insurance dataset** (1,338 entries, 7 columns) to explore the relationship between demographic, lifestyle, and regional factors and the **medical insurance charges**.  

The dataset contains:
- **age**: Age of the individual  
- **sex**: Gender (male/female)  
- **bmi**: Body Mass Index (numeric)  
- **children**: Number of children covered by health insurance  
- **smoker**: Whether the individual is a smoker (yes/no)  
- **region**: Residential region (northeast, northwest, southeast, southwest)  
- **charges**: Medical insurance charges billed  

---

## 📂 Files
- `insurance.csv` – dataset used for analysis  
- `insurance new11.pdf` – exploratory data analysis (EDA) results exported from Google Colab  
- `Untitled3.ipynb` – Jupyter/Colab notebook with analysis  

---

## 🔍 Exploratory Data Analysis (EDA)
- **Data Quality**: No missing values, 1,338 rows × 7 columns  
- **Descriptive Statistics**:
  - Mean Age: ~39 years  
  - Mean BMI: ~30.66  
  - Mean Charges: ~$13,270  
- **Distribution Insights**:
  - Balanced gender ratio (676 males, 662 females)  
  - Age uniformly distributed between 18–64  
  - Charges highly skewed (some very high values for smokers)  
- **Visualizations**:
  - Histograms of age, BMI, children  
  - Count plots of sex, smoker, region  
  - Boxplots for BMI and region  
  - Pairplot with insurance charges as hue  

---

## ⚙️ Preprocessing
- Applied **Label Encoding** on categorical variables:  
  - `sex`, `smoker`, `region`  
- ⚠️ Note: At one point `bmi` was also encoded as categorical, which is incorrect since it is numerical. This should be fixed in modeling steps.  

---

## 🚀 Next Steps
- Correct preprocessing (scale numerical features, encode categorical properly).  
- Correlation analysis (check relation of charges with age, BMI, smoker).  
- Build predictive models:
  - Linear Regression  
  - Random Forest / Gradient Boosting  
- Evaluate model performance (RMSE, R²).  

---

## 🛠️ Requirements
This project uses:
- Python 3.x  
- pandas, numpy  
- seaborn, matplotlib  
- scikit-learn  

Install dependencies with:  
```bash
pip install pandas numpy seaborn matplotlib scikit-learn

📊 Example Visualization

Example: Age distribution of insured individuals.

import seaborn as sns
import matplotlib.pyplot as plt

sns.histplot(df['age'], bins=20, kde=True)
plt.title("Age Distribution")
plt.show()

👩‍💻 Author

Analysis prepared in Google Colab

Exported as PDF (insurance new11.pdf)

author-Abhishek
---
