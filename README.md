# 🛒 E-Commerce Data Analysis (Pandas & Exploratory Data Analysis)

This repository contains an Exploratory Data Analysis (EDA) performed on an E-Commerce orders dataset using Python and Pandas. The project focuses on data inspection, filtering, missing value checks, and analyzing sales performance across various categories, products, and payment modes.

---

## 📊 Dataset Overview

The dataset contains order details, customer demographics, pricing, and order fulfillment status.

- **Total Initial Records:** 30,250 rows × 15 columns
- **Filtered Subset (Jaipur Region Analysis):** 1,383 rows × 15 columns

### Dataset Features:
* **Order Info:** `Order_ID`, `Order_Date`, `Order_Status`, `Delivery_Days`
* **Customer Info:** `Customer_Name`, `City`, `Customer_Age`
* **Product Details:** `Product`, `Category`, `Quantity`, `Unit_Price`, `Discount`
* **Financials & Feedback:** `Sales`, `Payment_Mode`, `Rating`

---

## 🛠️ Tech Stack & Libraries Used

* **Python 3.x**
* **Pandas:** Data manipulation, cleaning, and aggregation
* **Jupyter Notebook:** Interactive development environment

---

## 🔑 Key Steps & Analysis Covered

1. **Data Loading & Inspection:**
   * Read raw CSV file (`ecommerce_data.csv`).
   * Checked dataset shape, column data types (`dtypes`), head, and tail rows.

2. **Data Quality & Missing Values:**
   * Handled missing values across key fields like `Rating` (453 missing), `Customer_Name`, `Sales`, `City`, etc.
   * Detected duplicate rows (250 duplicate records found initially).

3. **Data Filtering & Subsetting:**
   * Filtered high-quantity orders (`Quantity > 5`).
   * Subset region-specific data for analysis (e.g., `City == 'Jaipur'`).
   * Isolated completed purchases (`Order_Status == 'Delivered'`).

4. **Group Aggregation & Insights:**
   * **Revenue Analysis:** Total sales calculation by city and average sales by category.
   * **Product Demand:** Grouped total quantity sold per product.
   * **Payment Methods:** Analyzed sales distribution and preferred payment modes (`Credit Card`, `Net Banking`, `UPI`, `Cash`, `Wallet`, etc.).
   * **Order Status Check:** Counted distribution of order statuses (`Delivered`, `Shipped`, `Pending`, `Returned`, `Cancelled`).

---

## 📈 Sample Results & Insights

* **Jaipur Region Total Sales:** ~₹28,87,94,100
* **Average Order Value (Jaipur):** ₹2,10,952.57
* **Top Selling Products (by Quantity):** Cameras, Monitors, Gaming Chairs, Speakers, and Laptops.
* **Payment Mode Trends:** `Credit Card` and `Net Banking` recorded the highest total sales volume among users.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
