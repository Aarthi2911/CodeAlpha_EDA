# E-Commerce Sales Exploratory Data Analysis

## Project Overview

This project was completed as part of the CodeAlpha Data Analytics Internship. The objective is to perform Exploratory Data Analysis (EDA) on an e-commerce sales dataset to understand product performance, customer preferences, pricing patterns, monthly sales trends, and customer reviews.

## Dataset Description

The dataset contains 1,000 unique e-commerce products across 7 different categories and includes 18 original columns.

### Key Features

- `product_id` - Unique identifier for each product
- `product_name` - Name of the product
- `category` - Product category
- `price` - Price of the product in USD
- `review_score` - Average customer review score from 1 to 5
- `review_count` - Total number of customer reviews
- `sales_month_1` to `sales_month_12` - Monthly unit sales over a 12-month period

Two additional features were created during the analysis:

- `total_sales` - Total units sold across all 12 months
- `estimated_revenue` - Product price multiplied by total annual unit sales

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Visual Studio Code

## Exploratory Data Analysis Performed

The following analyses were performed:

1. Loaded and inspected the dataset.
2. Examined dataset dimensions, column names, and data types.
3. Checked for missing values and duplicate records.
4. Analyzed the distribution of products across categories.
5. Calculated total annual sales for each product.
6. Estimated annual revenue for each product.
7. Identified the top-selling products.
8. Analyzed category-level sales and estimated revenue.
9. Examined average customer review scores by category.
10. Analyzed monthly sales trends.
11. Studied correlations between price, reviews, and total sales.
12. Detected potential outliers using the Interquartile Range (IQR) method.
13. Generated a correlation matrix for key numerical features.

## Key Insights

- The dataset contains **1,000 unique products** across **7 categories**.
- **Books** was the best-selling category with **938,229 units sold**.
- **Home & Kitchen** recorded the lowest category sales with **742,141 units sold**.
- **Product_224**, from the Electronics category, was the top-selling individual product with **9,151 units sold**.
- **Month 10** recorded the highest overall sales with **514,798 units sold**.
- **Month 5** recorded the lowest overall sales with **487,194 units sold**.
- The correlation between product price and total sales was **-0.016**, indicating virtually no linear relationship.
- The IQR method identified **13 potential total-sales outliers**.
- Total estimated annual revenue was approximately **$1.49 billion**.

## Conclusion

The exploratory data analysis revealed meaningful insights into product performance, category-level sales, monthly sales patterns, customer reviews, pricing relationships, and potential anomalies.

Books emerged as the strongest category based on total units sold, while Product_224 was the highest-selling individual product. Sales remained relatively consistent throughout the 12-month period, with Month 10 recording the highest performance. The near-zero correlation between product price and total sales suggests that price alone was not a significant linear predictor of sales volume in this dataset.

## Project Structure

```text
CodeAlpha_EDA/
│
├── dataset/
│   ├── ecommerce_sales_analysis.csv
│   └── ecommerce_sales_cleaned.csv
│
├── EDA_Analysis.ipynb
├── README.md
└── requirements.txt