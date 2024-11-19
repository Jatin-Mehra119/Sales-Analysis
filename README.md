# Urban Reach Mart
**Urban Reach Mart** is a multi-branch retail store operating in three major cities of Myanmar—Mandalay, Naypyitaw, and Yangon. The store offers a wide range of products, spanning six distinct categories: Electronic Accessories, Food and Beverages, Sports and Travel, Home and Lifestyle, Fashion Accessories, and Health and Beauty. Known for its diverse offerings, Urban Reach Mart caters to the everyday needs of customers in urban Myanmar.

## Data Analysis Report
-   **Objective of the report:** 
	- This report aims to analyze sales performance across branches, product lines, Customers, to uncover key insights, pattern of sales, Sales trend and Optimize sales operations.
---
-   **Brief overview of the dataset:**
	-  **Number of Transactions:** 100
	- **Time Range:** 1st January 2019 to 30th March 2019
	- **Data Source** - Kaggle
	- **Columns:**
		 -   **Invoice ID:** Unique transaction identifier.
		-   **Branch & City:** Store location.
		-   **Customer Type:** Whether the customer is a member or a normal customer.
		-   **Gender:** Demographic segmentation.
		-   **Product Line:** Category of purchased products.
		-   **Unit Price & Quantity:** Pricing and sales volume.
		-   **Tax 5% & Total:** Financial metrics.
		-   **Date & Time:** Temporal patterns in sales.
		-   **Payment:** Payment method used.
		-   **COGS, Gross Margin, Gross Income:** Profitability insights.
		-   **Rating:** Customer satisfaction metric.
-   **Tools and methods:** 
	- Programming language: Python
	- Libraries: Pandas, Matplotlib, Seaborn
	- Tools: Jupyter Notebook, Power Bi.
---
- **Data cleaning and preprocessing steps:**
	- Checked for Null/Duplicates.
	- Created new features from date and time feature.
---
### **Exploratory Data Analysis (EDA):**
-	**Total Sales:** 3,22,966.74
-	**Average Gross Income Per Transaction:** 15.37
-	**Total Gross Income:** 15379.36	
---
###  **Average Gross Income by Day of Week**:
	
| Day of Week | Average Gross Income |
|-------------|-----------------------|
| Sunday           | 14.437744            |
| Monday           | 15.516047            |
| Tuesday           | 14.562483            |
| Wednesday           | 15.648464            |
| Thursday           | 15.048421            |
| Friday           | 16.295241            |
| Saturday           | 15.917613            |
---

### **Citywise Sales & Revenue**:

| City       | Total Sales Value      | Total Quantity | Total Gross Income |
|------------|-------------|----------|--------------|
| Mandalay   | 106197.6720 | 1820     | 5057.0320    |
| Naypyitaw  | 110568.7065 | 1831     | 5265.1765    |
| Yangon     | 106200.3705 | 1859     | 5057.1605    |

![image](https://github.com/user-attachments/assets/7fa8e5e8-a421-465c-976e-40a95a430b41)

---
### **Customer Behavior**:

- Normal V/s Member:

| Customer Type | Total       | Total Quantity | Total Gross Income |
|---------------|-------------|----------|--------------|
| Member        | 164223.444  | 2785     | 7820.164     |
| Normal        | 158743.305  | 2725     | 7559.205     |

![image](https://github.com/user-attachments/assets/09392e1f-020e-4d77-bc66-e2eeda2b7488)

---
-  Female vs Male Distributions:

| Gender | Total       | Total Quantity | Total Gross Income |
|--------|-------------|----------|--------------|
| Female | 167882.925  | 2869     | 7994.425     |
| Male   | 155083.824  | 2641     | 7384.944     |

![image](https://github.com/user-attachments/assets/b7489be1-5fcf-4286-8aa6-368c4bb82137)
---
### Ratings Trends

- City wise Ratings Trends:

| City       | Branch | Average Ratings    |
|------------|--------|----------|
| Mandalay   | B      | 6.818072 |
| Naypyitaw  | C      | 7.072866 |
| Yangon     | A      | 7.027059 |

---

-  Customer Type Ratings Trends:

| Customer type | Average Ratings |
| ----------------| ----------|
| Member |   6.940319 |
| Normal |  7.005210 |

- Average Ratings by Product line:

![image](https://github.com/user-attachments/assets/a8d5c325-7529-4542-aac2-21219237d957)

---
### Product Line Analysis:
- Distribution

| Product Line           | Count |
|------------------------|-------|
| Electronic accessories | 971   |
| Food and beverages     | 952   |
| Sports and travel      | 920   |
| Home and lifestyle     | 911   |
| Fashion accessories    | 902   |
| Health and beauty      | 854   |

![image](https://github.com/user-attachments/assets/aedb3872-9a0f-4bca-9f97-6be1afc0ca21)

---
- Sales performance of product line:

| Product Line           | Total Sales      | Total Quantity | Total Gross Income |
|------------------------|-------------|----------|--------------|
| Electronic accessories | 54337.53  | 971      | 2587.50    |
| Fashion accessories    | 54305.89  | 902      | 2585.99    |
| Food and beverages     | 56144.84  | 952      | 2673.56    |
| Health and beauty      | 49193.73  | 854      | 2342.55    |
| Home and lifestyle     | 53861.91  | 911      | 2564.85    |
| Sports and travel      | 55122.82  | 920      | 2624.89    |

![image](https://github.com/user-attachments/assets/1444726f-b9f4-4f73-a5fb-21c86fccbb2b)

---
-  Product line performance by Day:

![image](https://github.com/user-attachments/assets/b68c659f-1dc9-452d-90fe-6b54d71b7174)

---
- Product line performance by Day of Week:

![image](https://github.com/user-attachments/assets/2297e736-8104-4b72-9195-5b8b517c4f50)

---
- Product line performance by Hours:

![image](https://github.com/user-attachments/assets/c3b59b41-6a07-471b-b614-9b8f3377b4f5)

---
- Sales Trend over time:

![image](https://github.com/user-attachments/assets/d0d76dfe-d421-42eb-a173-8239229d04df)

---
- Hourly Sales Trend: 

![image](https://github.com/user-attachments/assets/493519b0-d9a7-475e-b7c6-2c0674bcb733)

---
### Analysis of Payment Types:

- Distribution 

 | Payment Type | Counts |
 |----|----|
 | Ewallet |       345 |
 | Cash    |       344 |
 | Credit card  |  311 |

 ![image](https://github.com/user-attachments/assets/b0d6e1ca-1673-4eb8-9727-44d7cfa3bf1e)

---

- Distribution of Payment types in Total Sales Transactions:

| Payment       | Sum        | Mean       |
|---------------|------------|------------|
| Cash          | 112206.570 | 326.181890 |
| Credit card   | 100767.072 | 324.009878 |
| Ewallet       | 109993.107 | 318.820600 |

![image](https://github.com/user-attachments/assets/55a8f4e5-4ad3-4194-82a3-baa0c7128f51)

---

- Average Distribution of Payment types in Gross Income:

| Payment       | Gross Income | Gross Margin Percentage |
|---------------|--------------|-------------------------|
| Cash          | 15.532471    | 4.761905                |
| Credit card   | 15.429042    | 4.761905                |
| Ewallet       | 15.181933    | 4.761905                |

---

- Product line Sales by Payment method

![image](https://github.com/user-attachments/assets/83fa5f53-edd9-4853-99fd-51ce39bc3fa3)

