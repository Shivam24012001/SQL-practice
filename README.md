# 📊 YellowMart Sales SQL Analysis  

## 📌 Overview  
This project contains SQL queries to analyze YellowMart's sales dataset. The dataset includes sales orders, regions, salespersons, products, and financial metrics such as cost, sales, and profit.  

## 🗂️ Dataset Description  
The dataset consists of various attributes such as:  
- **Order Details:** Order Number, Order Date  
- **Location Information:** Region, State, City  
- **Salesperson Details:** First Name, Last Name  
- **Product Information:** Category, Subcategory  
- **Financial Metrics:** Cost, Sales, Profit

## 🏗️ Steps Performed  
1. **Data Extraction:** Downloaded dataset from GitHub using Python.  
2. **Data Loading:** Stored the dataset in an SQLite database (`ylwmart.db`).  
3. **SQL Query Execution:** Performed various data analysis tasks using SQL.  

## 🛠️ Technologies Used  
- **Python** 🐍 - Data processing and database management  
- **Pandas** 📊 - Data manipulation and analysis  
- **SQLite** 🗄️ - Database for running SQL queries  
- **Requests** 🌐 - Downloading the dataset from GitHub  
- **Google Colab** 💻 - Running Python scripts in a cloud environment  
- **SQL** 🏆 - Data querying and analysis using SQLite  

## 🏗️ Tasks and SQL Queries  
The analysis involves various SQL queries to retrieve meaningful insights from the dataset.  

### ✅ Task 1: Retrieve the Sales Data from `ylwmart`  
Retrieve all the available sales records from the `ylwmart` dataset.

### ✅ Task 2: Retrieve Full Name & Email ID of Salesperson  
- Convert names to proper case  
- Generate an email ID in the format `firstname.lastname@yellowmart.com`  

### ✅ Task 3: Extract Full Name, Region, Order Year, Sales & Profit (2020)  
- Ensure proper name formatting  
- Remove extra spaces in the `Region` column  
- Extract `Order Year` from `Order Date`  

### ✅ Task 4: Retrieve Order ID & Its Length  
- Fetch `OrderNumber` along with its length  

### ✅ Task 5: Retrieve Orders Where Order ID Length is 6  
- Include Order ID, its length, and the subcategory  

### ✅ Task 6: Retrieve Category, Subcategory, Sales & Profit for Order ID Length 6  
- Trim spaces from `Category`  

### ✅ Task 7: Retrieve Subcategories Starting With 'O'  
- Display subcategories and their respective categories  

### ✅ Task 8: Compute Total Sales, Cost & Profit by Category  
- Remove any extra spaces from `Category`  

### ✅ Task 9: Compute Total Sales & Profit Per Year & Category (After 2018)  
- Extract `Order Year` from `Order Date`  
- Summarize total sales & profit  

### ✅ Task 10: Retrieve Maximum Sales Amount Per Year  
- Extract `Order Year` and find the highest sales value  

### ✅ Task 11: Count Orders Per Category for 2020  
- Ensure categories are unique  
- Count the number of orders per category  

### ✅ Task 12: Compute Total Sales for East & West Regions by Year  
- Extract `Order Year`  
- Filter for `East` and `West` regions  

### ✅ Task 13: Count Orders Where Order ID Length is 6 & Yearly Orders  
- Count total orders per year  
- Count orders where `Order ID` is of length 6

### ✅ Task 14: Count the Number of Orders Per Year  
- Extract the **Order Year** from the `OrderDate`.  
- Count the total number of orders received each year.  
- Output Columns: `OrderYear`, `OrderCount`.  

## 🔧 Function Used  
- **Aggregation Functions (SUM, COUNT, MAX)**  
- **String Manipulation (REPLACE, TRIM, LOWER, UPPER, CONCAT)**
