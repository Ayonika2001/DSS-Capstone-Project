
# 📊 SBI Customer Churn Analysis Project

This repository contains a comprehensive customer churn analysis project using **Python**, **Power BI**, **Excel**, and **PowerPoint**, focused on SBI (State Bank of India) customer data. The project is designed to identify key churn factors, visualize business insights, and propose actionable strategies for improving customer retention.

---

## 📁 Project Structure

```
SBI-Churn-Analysis/
│
├── SBI Churn Analysis(Python).ipynb      # Python notebook with EDA & ML
├── SBI Churn Analysis(Power BI).pbix     # Power BI report with dashboards
├── SBI Churn Analysis.xlsx               # Cleaned data & master sheet
├── SBI Churn Analysis Powerpoint Presentation.pptx  # Final presentation
└── README.txt                            # This documentation file
```

---

## 🐍 Python Analysis Highlights (`.ipynb`)
### **Data Cleaning & Preprocessing**
- Loaded CSV into Pandas DataFrame.
- Filled missing 'Total Charges' with 0.
- Replaced NaNs in service fields with "N/A".
- Converted `Churn` column to numeric (Yes → 1, No → 0).

### **Exploratory Data Analysis**
- Used histograms, boxplots, and heatmaps to identify churn drivers.
- Key Findings:
  - **Tenure** and **Total Charges** are negatively correlated with churn.
  - **Monthly Charges** have a positive correlation with churn.

### **Code Snippet Example**
```python
df['Churn'] = df['Churn'].map({'Yes': 1, 'No': 0})
df['TotalCharges'] = pd.to_numeric(df['TotalCharges'], errors='coerce').fillna(0)
```

---

## 📈 Power BI Report (`.pbix`)
### Key Visuals:
- **Churn Rate**: 26.54%
- **Customer Segmentation**: Based on tenure, contract, and service use.
- **Retention Dashboard**: Drill-down by payment method, service type, and contract.

### Example Insights:
- Month-to-month customers churn more.
- Electronic check payment method has highest churn.
- Fiber Optic users show highest churn rate.

---

## 📊 Excel Project (`.xlsx`)
### Tasks Performed:
- Cleaned and merged Customer, Internet, and Churn datasets.
- Created a **Master Sheet** using **Power Query** and Customer ID as key.

### Cleaning Steps:
- Handled nulls, invalid dates (e.g., 30th Feb), and ensured leap year validity.
- Computed missing age and senior citizen status.

---

## 📽️ PowerPoint Presentation (`.pptx`)
### Content Overview:
- Project summary, data source explanation, and visual insights.
- Slide visuals for **Churn Distribution**, **Contract Impact**, **Payment Type**, and **Recommendations**.

### Recommendations:
1. Promote long-term contracts with discounts.
2. Improve early-stage customer retention with bonuses.
3. Offer flexible pricing for high-bill customers.
4. Encourage secure & automated payment methods.
5. Bundle services to reduce churn.

---

## 🔍 Conclusion
This project showcases how data analytics can drive customer retention strategies. Using EDA, BI tools, and clean data practices, we uncovered patterns and provided data-backed suggestions to reduce churn and improve loyalty.

---

## 📧 Contact
**Email**: duttaayonika120@gmail.com
