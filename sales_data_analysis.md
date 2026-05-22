

## 📊 Dataset Information

The project utilizes the `festival_sales_data.csv` dataset, which contains transaction records captured during a festive season sale. It features a blend of customer demographics and purchasing behavior metrics across different states in India.

### 🗂️ Data Dictionary

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| **User_ID** | Integer | Unique identifier for each customer |
| **Cust_name** | Object/String | Name of the customer |
| **Product_ID** | Object/String | Unique identifier for the product purchased |
| **Gender** | Object/String | Gender of the customer (`F` for Female, `M` for Male) |
| **Age Group** | Object/String | Categorized age brackets (e.g., `0-17`, `18-25`, `26-35`, `36-45`, `46-50`, `51-55`, `55+`) |
| **Age** | Integer | Exact age of the customer |
| **Marital_Status**| Integer | Marital status indicator (`0` for Unmarried, `1` for Married) |
| **State** | Object/String | Indian state where the transaction occurred (e.g., Maharashtra, Uttar Pradesh, Karnataka) |
| **Zone** | Object/String | Geographic zone of the state (`Central`, `Western`, `Southern`, `Northern`, `Eastern`) |
| **Occupation** | Object/String | Industry sector of the customer (e.g., Healthcare, IT Sector, Aviation, Banking) |
| **Product_Category**| Object/String | Category of the product sold (e.g., Auto, Food, Clothing, Electronics, Stationery) |
| **Orders** | Integer | Number of units/orders placed in the transaction |
| **Amount** | Float/Numeric | Total monetary value (revenue) of the purchase |
| **Status** | Float/Numeric | Empty/unutilized column (dropped/cleaned during preprocessing) |
| **unnamed1** | Float/Numeric | Empty/unutilized column (dropped/cleaned during preprocessing) |

### 📈 Dataset Summary & Shape
- **Total Rows:** ~11,251 records
- **Total Columns:** 15 columns
- **Target Variables for Analysis:** `Orders` and `Amount` grouped by customer demographic features like `Age Group`, `Gender`, and `State`.

### 🧹 Key Data Preprocessing Steps (included in Notebook)
1. **Handling Missing Values:** Identified and dropped unneeded null columns (`Status` and `unnamed1`). Dropped rows with null values in the `Amount` column to maintain computational accuracy.
2. **Data Type Correction:** Converted the `Amount` column from float to integer for clean data handling.


## 📌 Key Insights & Conclusion
Based on the Exploratory Data Analysis (EDA):
* **Top Buyers:** Married women aged between 26-35 years represent the highest purchasing demographic.
* **Geographic Leaders:** Uttar Pradesh, Maharashtra, and Karnataka generated the maximum sales volume and revenue.
* **Top Industries:** Customers working in IT, Healthcare, and Aviation sectors are the most active buyers.
* **Leading Categories:** Food, Clothing, and Electronics are the most sold product categories.
