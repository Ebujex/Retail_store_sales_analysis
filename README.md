# 📊 Retail Store Sales Dashboard

## 📝 Introduction
This Retail Store Sales Dashboard was created to showcase my fundamental skills in Excel for Data Analytics. The goal was to transform raw transaction records into an interactive dashboard that aids in decision-making.

The dataset was sourced from **Kaggle** and it contains Product Category, Payment Method, Location, and Revenue generated.

### Dashboard File  
My final dashboard is in [retail_store_sales_clean.xlsx](https://github.com/user-attachments/files/24079868/retail_store_sales_clean.xlsx)


## 🛠 Excel Skills Used
The following Excel skills were utilized for this analysis:
*   **Data Cleaning:** Handling missing values and standardizing text.
*   **Formulas & Functions:** XLOOKUP, TEXTJOIN, TEXT, etc.
*   **Pivot Tables:** Summarizing large datasets.
*   **Data Visualization:** Bar Charts, Column Charts, and Slicers.

## 📂 The Dataset
The dataset used for this project contains retail store sales information for the year 2024. It includes detailed information on:
*   **Category:** The type of product sold.
*   **Payment Method:** How the customer paid (Cash, Card, etc.).
*   **Location:** Online or Offline stores.
*   **Total Spent:** The revenue generated per transaction.

---

## 📐 Formulas and Functions

### 1. Filling Missing Data (XLOOKUP)
```excel
=XLOOKUP(C2, C$2:C$1048576, G$2:G$1048576)
```  


*  **Function Used:** XLOOKUP  
*  **Purpose:** This formula populates the "Category_short" column by filling in empty cells based on the main Category column. It ensures every row has a standardized abbreviation.
  
<img width="244" height="149" alt="category_short" src="https://github.com/user-attachments/assets/e956ca47-76ef-4c02-864c-2e254fad5be0" />  

### 2. Joining Text (TEXTJOIN)

```excel
=TEXTJOIN("_", TRUE, D2, E2)
```  
* **Function Used:** TEXTJOIN
* **Purpose:** Used to create unique identifiers. After splitting a column into multiple parts, this formula re-joined specific text strings using an underscore (_) as a delimiter.

  <img width="178" height="162" alt="item_join" src="https://github.com/user-attachments/assets/c70cc2ad-38b1-49b6-bf10-529f18e63f7e" />

###  3. Month Extraction (TEXT)
```excel
=TEXT(L2, "mmmm")
```

* **Function Used:** TEXT
* **Purpose:** To extract the full month name (e.g., "January") from the transaction date column to facilitate monthly trend analysis.

  <img width="178" height="160" alt="transaction_month" src="https://github.com/user-attachments/assets/5e278e4d-a91b-494e-b587-b72b1b587746" />

##  📊 Dashboard Visualizations
### 1. Total Monthly Sales (Column Chart)   
<img width="562" height="267" alt="monthly_sales_dashboard" src="https://github.com/user-attachments/assets/9ebac578-59e3-4036-bf75-41e6850518e1" />  

* **Excel Features:** Clustered Column Chart.  
* **Design Choice:** A vertical bar chart was used for visual comparison of monthly revenue.  
* **Data Organization:** Months are sorted chronologically (Jan-Dec).  
* **Insights:** The chart highlights revenue trends, showing that the store achieved its highest revenue in January.
  
### 2. Total Revenue by Category (Bar Chart)  
<img width="533" height="246" alt="category_sales_dashboard" src="https://github.com/user-attachments/assets/8bc6e518-310a-484b-bef3-a11c21ac88de" />  

* **Excel Features:** Horizontal Bar Chart.  
* **Design Choice:** Horizontal orientation was chosen to make category names easier to read.  
* **Data Organization:** Categories are sorted by total revenue (Descending) to highlight top performers instantly.  
* **Insights:** "Butchers" and "Electric Household Essentials" generate significantly more revenue than other categories.

### 3. Dashboard Interactivity (Slicers)  
<img width="145" height="75" alt="location_slicer" src="https://github.com/user-attachments/assets/67babf73-a900-4378-8dbe-e3a245000a6a" />  


<img width="144" height="96" alt="payment_method_slicer" src="https://github.com/user-attachments/assets/f686599a-b573-4d57-98ec-209971e13e37" />  

*   **Feature:** Dynamic Slicers for **Location** (Online/Offline) and **Payment Method**.
*   **Functionality:** I connected these Slicers to every Pivot Chart using "Report Connections." This allows the user to filter the entire dashboard with a single click.
*   **User Experience:** This feature transforms the report from a static image into an interactive tool, allowing stakeholders to drill down into specific data points (e.g., viewing performance specifically for *Online* customers).

## 🎯 Conclusion  
I created this dashboard to provide actionable insights into the 2024 sales performance of a retail store. By utilizing Data Cleaning and Pivot Tables, this project transforms raw data into a clear story, allowing stakeholders to identify top-selling products and seasonal trends.  



