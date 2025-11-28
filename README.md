# Quantium Virtual Internship – Retail Strategy & Analytics (Task 1)  

## Overview
This project showcases a **sample solution** for the Data Preparation and Customer Analytics Task of the **Quantium Virtual Internship**. The main goal is to explore customer purchasing behavior in the potato chips category, clean and preprocess transaction data, and analyze customer segments to derive actionable insights.  

## Dataset
1. **Transaction Data** (`QVI_transaction_data.csv`)  
   - `DATE`, `STORE_NBR`, `LYLTY_CARD_NBR`, `TXN_ID`, `PROD_NBR`, `PROD_NAME`, `PROD_QTY`, `TOT_SALES`  

2. **Customer Data** (`QVI_purchase_behaviour.csv`)  
   - `LYLTY_CARD_NBR`, `LIFESTAGE` (e.g., Young Singles/Couples, Retirees), `PREMIUM_CUSTOMER` (Premium, Mainstream, Budget)  

## Tools & Libraries
- **R**  
- Packages: `data.table`, `ggplot2`, `ggmosaic`, `readr`  

```r
install.packages(c("data.table", "ggplot2", "ggmosaic", "readr"))
````

## Steps

1. Load and clean the datasets.
2. Remove non-chip products and outliers.
3. Extract pack sizes and standardize brand names.
4. Merge transaction and customer data for analysis.
5. Perform exploratory data analysis (sales trends, brand popularity, customer segmentation).

## Analysis & Insights

* High sales driven by **Budget Older Families**, **Mainstream Young Singles/Couples**, **Mainstream Retirees**.
* Older and young families purchase more units per customer.
* Mainstream young singles/couples pay higher average prices per unit.
* Segment-focused marketing can improve sales and retention.

## How to Run

1. Place CSV files in the working directory.
2. Update `filePath` in the R script:

```r
filePath <- "path_to_your_data/"
transactionData <- fread(paste0(filePath, "QVI_transaction_data.csv"))
customerData <- fread(paste0(filePath, "QVI_purchase_behaviour.csv"))
```

3. Run the R script to generate cleaned data and visualizations.

## Author

**Chalani Navoda** 

```

