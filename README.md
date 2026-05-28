# **Bank Customer Churn – Data Acquisition, Wrangling & Analytical Structuring**  
*A structured data‑engineering and analytics case study*

## **Overview**
This project demonstrates a full end‑to‑end data preparation workflow using a real‑world banking churn dataset. The work spans **data acquisition**, **web scraping**, **data quality assessment**, **consolidation**, **duplicate and missing‑value treatment**, **feature engineering**, and **segmentation‑based aggregation**.  

The project is implemented in Python using Jupyter Notebook and reflects industry‑aligned data‑wrangling practices relevant to customer analytics, churn modelling, and financial services insights.

---

## **Objectives**
- Acquire and inspect structured and semi‑structured data programmatically.  
- Evaluate dataset structure, schema alignment, and data integrity.  
- Consolidate multiple datasets into a unified analytical base table.  
- Identify and resolve duplicates and missing values using justified strategies.  
- Engineer new features, including age‑based and value‑based customer segments.  
- Produce grouped aggregations and pivot‑based summaries to support downstream modelling and visualisation.

---

## **Data Sources**
### **1. Bank Churn Dataset (Primary Dataset)**
Loaded directly from a public GitHub repository.  
Includes customer demographics, account activity, and financial indicators used to analyse churn behaviour.

### **2. Web‑Scraped Banking Table**
Extracted from Wikipedia using `requests` and `BeautifulSoup`.  
Demonstrates semi‑structured data acquisition and transformation into a Pandas DataFrame.

---

## **Key Components**

### **Part 1 — Data Acquisition & Initial Inspection**
- Loaded structured CSV data using `pandas.read_csv()`.  
- Displayed head, schema, and column names.  
- Scraped a banking‑related table from Wikipedia and converted it into a DataFrame.  
- Compared structure and degree of organisation across both sources.

---

### **Part 2 — Data Wrangling & Structural Refinement**
#### **1. Structural Evaluation**
- Assessed dataset formats (wide vs. long).  
- Verified schema alignment between datasets.  
- Discussed implications for merging and downstream analysis.

#### **2. Consolidation**
- Combined datasets using a justified merge/concatenation strategy.  
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
- Removed irrelevant or redundant variables with justification.

---

### **Part 3 — Segmentation, Aggregation & Pivoting**
#### **1. Age‑Based Segmentation**
- Created interpretable age bands using custom binning logic.

#### **2. Value‑Based Segmentation**
- Segmented customers by financial value using balance or estimated salary.

#### **3. Grouped Aggregation**
- Produced multi‑level grouped summaries (e.g., churn rate by geography and gender).  
- Included segmentation‑based aggregations (e.g., average balance by age group).

#### **4. Pivot Table Construction**
- Built a pivot table to analyse churn behaviour across categorical dimensions.  
- Interpreted results in a business‑relevant context.

---

## **Tools & Technologies**
- **Python**  
- **Pandas**  
- **NumPy**  
- **BeautifulSoup (bs4)**  
- **Requests**  
- **Jupyter Notebook**

---

## **Skills Demonstrated**
- Data acquisition (structured + web‑scraped)  
- Data wrangling and cleaning  
- Duplicate and missing‑value strategy design  
- Feature engineering  
- Segmentation logic  
- Grouped aggregation and pivot‑based structuring  
- Analytical reasoning and data integrity assessment  

---

## **Project Structure**
```
📁 bank-churn-case-study
│
├── SS1_Data_Acquisition.ipynb
├── SS2_Data_Wrangling_and_Structuring.ipynb
├── reflection.pdf
└── README.md
```

---

## **Potential Extensions**
This project sets the foundation for:  
- Predictive churn modelling (logistic regression, tree‑based models)  
- Customer lifetime value estimation  
- Visual analytics dashboards (Power BI, Tableau, or Python visualisation)  
- Bias and fairness evaluation in financial analytics  

