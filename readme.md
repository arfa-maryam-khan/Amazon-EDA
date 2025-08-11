# Customer & Sales Insights from Amazon Clothing Transactions

## Project Overview
This project performs exploratory data analysis (EDA) on a real-world dataset of Amazon clothing sales transactions from 2024-2025. The goal is to extract actionable business insights related to sales, returns, customer behavior, pricing, and delivery performance.

---

## Learning Objectives
- Clean and preprocess messy real-world data (handle missing values, inconsistent types, outliers).
- Formulate and test business hypotheses.
- Conduct univariate, bivariate, and multivariate exploratory analyses.
- Derive insights on sales trends, returns, pricing, and delivery.
- Visualize data effectively with clear, insightful charts.
- Structure reproducible code and document findings for sharing.
- Communicate recommendations to product and operations teams.

---

## Dataset Description
**Amazon Clothing Sales 2025**  
Contains 25,000+ transaction records scraped from Amazon product pages and seller listings.  
Categories: Men, Women, Kids, Baby clothing.  

### Key Columns
| Column            | Description                                   |
|-------------------|-----------------------------------------------|
| order_id          | Amazon-style alphanumeric order ID            |
| customer_id       | Unique customer identifier                     |
| product_id        | Product identifier (ASIN format)               |
| product_name      | Product brand and title                        |
| main_category     | Clothing category (Men, Women, Kids, Baby)    |
| sub_category      | Specific item type (e.g., Shirts, Dresses)    |
| brand             | Brand name (Nike, Zara, Carter’s, etc.)       |
| price             | Unit price in USD                              |
| quantity          | Number of units purchased                      |
| discount_percent  | Discount percentage applied                    |
| final_price       | Total paid after discount                      |
| payment_method    | Payment type (Credit Card, PayPal, etc.)      |
| review_rating     | Customer rating (1-5 scale)                    |
| order_date        | Date of purchase                               |
| delivery_days     | Days taken for delivery                         |
| is_returned       | Return status (1 = returned, 0 = not returned)|
| region            | Delivery region (US regions)                   |
| customer_age_group| Age bracket of customer                         |
| device_type       | Device used for purchase (mobile, desktop)    |

---

## Project Structure
- **Cleaned Jupyter Notebook** or Python script containing full EDA workflow.
- **README.md** (this file) outlining project, methods, and insights.
- **Data Quality Report**: Missing data, anomalies, cleaning decisions.
- **Insight Summary**: Top 5-8 key business insights with visuals and recommendations.
- **Hypothesis Testing**: At least 5 business hypotheses explored with supporting analysis.
- **Visualizations**: Well-labeled charts (line, bar, boxplot, heatmaps, scatter, etc.) with captions.

---

## EDA Outline

### 1. Data Cleaning & Preprocessing
- Check data types; convert dates.
- Handle missing values.
- Remove duplicates.
- Validate price and discount consistency.
- Outlier detection and treatment.
- Feature engineering (order month, weekday, discount amount, unit price, delivery speed flags).
- Aggregate customer-level metrics (total spend, order counts, return rates).

### 2. Exploratory Analysis
- **Univariate:** Distribution of prices, discounts, ratings, delivery times.
- **Bivariate & Multivariate:** Revenue trends, discount vs quantity, return rates by category/brand/age/device.
- Customer segmentation (RFM and behavior).
- Delivery performance and hotspots.
- Anomaly detection for suspicious orders.

### 3. Hypothesis Testing Examples
- Higher discounts increase quantity but raise return rates.
- Longer delivery times reduce ratings and increase returns.
- Younger age groups show different buying and return behaviors.
- Mobile users have different return patterns than desktop users.
- Premium brands show different return trends.

### 4. Advanced Analytics
- Cohort analysis for customer retention.
- Price elasticity estimation.
- Return prediction modeling prototype.
- Identification of delivery delay hotspots.

---

## How to Reproduce
1. Clone repository
2. Install dependencies listed in `requirements.txt`
3. Run the notebook/script to perform the full EDA
4. Review charts, tables, and findings
5. Refer to Data Quality Report and Hypothesis Testing sections for detailed analyses

---

## Requirements
- pandas
- numpy
- matplotlib
- seaborn
- fuzzywuzzy
- python-Levenshtein

See `requirements.txt` for exact package versions.

---

## Contact
For questions or collaboration, contact me.

---

*End of README*
