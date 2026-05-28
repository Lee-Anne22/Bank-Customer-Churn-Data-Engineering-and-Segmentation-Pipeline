# **Bank Customer Churn – Data Acquisition, Wrangling & Analytical Structuring**  
*A structured data‑engineering and analytics case study*

---

## **Overview**
This project presents an end‑to‑end data preparation workflow using **three complementary datasets** related to banking and customer churn. The work spans:

- Structured data acquisition  
- Web scraping  
- Data integrity evaluation  
- Dataset consolidation  
- Duplicate and missing‑value treatment  
- Feature engineering (age & value segmentation)  
- Grouped aggregation and pivot‑based structuring  

The project is implemented in Python using Jupyter Notebook and reflects industry‑aligned practices relevant to customer analytics, churn modelling, and financial services.

---

## 📂 **Project Structure**
```plaintext
📁 bank-churn-case-study
│
├── Bank_Churn_Set_1.ipynb
├── Bank_Churn_2.ipynb
|
└── README.md
```

---

## **Data Sources**

### **1. Bank Churn Dataset**
Loaded directly from a public GitHub repository.  
Contains customer demographics, account activity, and financial indicators used to analyse churn behaviour.

### **2. Web‑Scraped Banking Table**
Extracted from Wikipedia using `requests` and `BeautifulSoup`.  
Demonstrates the acquisition and transformation of semi‑structured web data into a usable DataFrame.

### **3. Additional CSV Dataset**
A second structured dataset provided for part 2.  
Used to evaluate schema alignment, consolidate records, and assess data integrity across multiple sources.

---

## **Key Components**

### **Part 1 — Data Acquisition & Initial Inspection**
- Loaded the primary Bank Churn dataset using `pandas.read_csv()`.  
- Displayed head, schema, and column names.  
- Scraped a banking‑related table from Wikipedia and converted it into a DataFrame.  
- Compared structure and degree of organisation across the two sources.

---

### **Part 2 — Data Wrangling & Structural Refinement**

#### **1. Structural Evaluation**
- Assessed the structure of all three datasets.  
- Identified wide vs. long formats.  
- Verified schema alignment between the two CSV datasets.  
- Discussed implications for merging and downstream analysis.

#### **2. Consolidation**
- Combined the two structured CSV datasets into a unified analytical base table.  
- Reported row counts before and after consolidation.  
- Identified potential data integrity risks introduced during merging.

#### **3. Duplicate Analysis**
- Detected and classified duplicate records.  
- Quantified duplication and applied appropriate resolution strategies.  
- Reported dataset size before and after treatment.

#### **4. Missing Value Treatment**
- Identified missing values by variable.  
- Evaluated analytical impact.  
- Applied justified imputation or removal strategies.  
- Verified successful treatment.

#### **5. Data Type & Structural Refinement**
- Ensured correct data types for all variables.  
- Converted categorical fields where appropriate.  
- Removed irrelevant or redundant variables.

---

### **Part 3 — Segmentation, Aggregation & Pivoting**

#### **1. Age‑Based Segmentation**
Created interpretable age bands using custom binning logic.

#### **2. Value‑Based Segmentation**
Segmented customers by financial value using balance or estimated salary.

#### **3. Grouped Aggregation**
Performed multi‑level grouped summaries, including:

- Average balance by age group  
- Mean credit score by churn status  
- Churn rate by geography and gender  

#### **4. Pivot Table Construction**
Built a pivot table to analyse churn behaviour across categorical dimensions and interpreted results in context.

---

## **Technologies Used**
- Python  
- Pandas  
- NumPy  
- BeautifulSoup (bs4)  
- Requests  
- Jupyter Notebook  

---

## **Skills Demonstrated**
- Structured + semi‑structured data acquisition  
- Web scraping  
- Data wrangling and cleaning  
- Duplicate and missing‑value strategy design  
- Feature engineering  
- Segmentation logic  
- Grouped aggregation and pivot‑based structuring  
- Analytical reasoning and data integrity assessment  

---

## **Potential Extensions**
- Predictive churn modelling  
- Customer lifetime value estimation  
- Visual analytics dashboards  
- Bias and fairness evaluation in financial analytics  

---
