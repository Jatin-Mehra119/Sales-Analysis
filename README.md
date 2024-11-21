# Urban Reach Mart
**Urban Reach Mart** is a multi-branch retail store operating in three major cities of Myanmar—Mandalay, Naypyitaw, and Yangon. The store offers a wide range of products, spanning six distinct categories: Electronic Accessories, Food and Beverages, Sports and Travel, Home and Lifestyle, Fashion Accessories, and Health and Beauty. Known for its diverse offerings, Urban Reach Mart caters to the everyday needs of customers in urban Myanmar.

## Data Analysis Report
-   **Objective of the report:** 
	- This report aims to analyze sales performance across branches, product lines, Customers, to uncover key insights, pattern of sales, Sales trend and Optimize sales operations.
---
-   **Brief overview of the dataset:**
	-  **Number of Transactions:** 1000
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
- **Total Sales**: 322966.749
- **Average Sales**: 322.966749
- **Toal Gross Income**: 15379.368999999999
- **Average Gross** Income: 15.379368999999999	
---
### **Average Gross Income by Day of Week**:

| Day Name   | Average Gross Income |
|------------|----------------------|
| Monday     | 14.437744            |
| Tuesday    | 15.516047            |
| Wednesday  | 14.562483            |
| Thursday   | 15.648464            |
| Friday     | 15.048421            |
| Saturday   | 16.295241            |
| Sunday     | 15.917613            |


- Saturday has the highest average gross income compared to other days: 6.18 % More than average
---

### **Citywise Sales & Revenue**:

| City       | Total Sales Value      | Total Quantity | Total Gross Income |
|------------|-------------|----------|--------------|
| Mandalay   | 106197.6720 | 1820     | 5057.0320    |
| Naypyitaw  | 110568.7065 | 1831     | 5265.1765    |
| Yangon     | 106200.3705 | 1859     | 5057.1605    |

![image](https://github.com/user-attachments/assets/7fa8e5e8-a421-465c-976e-40a95a430b41)

- Naypyitaw has the highest gross income compared to other cities: 2.71 % More than average
- Yangon has the highest quantity compared to other cities: 1.22 % More than average
---
### **Customer Behavior**:

- Normal V/s Member:

| Customer Type | Total       | Total Quantity | Total Gross Income |
|---------------|-------------|----------|--------------|
| Member        | 164223.444  | 2785     | 7820.164     |
| Normal        | 158743.305  | 2725     | 7559.205     |

![image](https://github.com/user-attachments/assets/09392e1f-020e-4d77-bc66-e2eeda2b7488)

- Member has higher total sales compared to Normal: 3.45 % More than average
- Member has higher quantity compared to Normal: 2.20 % More than average
---
-  Female vs Male Distributions:

| Gender | Total       | Total Quantity | Total Gross Income |
|--------|-------------|----------|--------------|
| Female | 167882.925  | 2869     | 7994.425     |
| Male   | 155083.824  | 2641     | 7384.944     |

![image](https://github.com/user-attachments/assets/b7489be1-5fcf-4286-8aa6-368c4bb82137)

- The female has produced the highest gross income compared to male : 3.96 % More than average
- The female has produced the highest quantity compared to male : 4.14 % More than average
---
### Ratings Trends

- City wise Ratings Trends:

| City       | Branch | Average Ratings    |
|------------|--------|----------|
| Mandalay   | B      | 6.818072 |
| Naypyitaw  | C      | 7.072866 |
| Yangon     | A      | 7.027059 |

- Branch A has the highest average rating compared to other branches: 1.44 % More than average
---

-  Customer Type Ratings Trends:

| Customer type | Average Ratings |
| ----------------| ----------|
| Member |   6.940319 |
| Normal |  7.005210 |

- Average Ratings by Product line:

![image](https://github.com/user-attachments/assets/a8d5c325-7529-4542-aac2-21219237d957)

- Normal Customers are more statisfied compared to Members: 0.93 % More than Members
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

- Electronic accessories has the highest quantity sold compared to other product lines: 5.74 % More than average
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

- Food and beverages has the highest gross income compared to other product lines: 4.30 % More than average

---
-  Product line performance by Day:

![image](https://github.com/user-attachments/assets/b68c659f-1dc9-452d-90fe-6b54d71b7174)


| **Product Line**          | **Day with Max Sales** | **Percentage Above Average** |
|----------------------------|------------------------|-------------------------------|
| Electronic Accessories     | 19                    | 129.87%                      |
| Fashion Accessories        | 8                     | 119.96%                      |
| Food and Beverages         | 27                    | 82.77%                       |
| Health and Beauty          | 15                    | 138.88%                      |
| Home and Lifestyle         | 3                     | 94.29%                       |
| Sports and Travel          | 17                    | 95.43%                       |


---
- Product line performance by Day of Week:

![image](https://github.com/user-attachments/assets/2297e736-8104-4b72-9195-5b8b517c4f50)

## Product Line Performance Analysis

| **Product Line**          | **Day with Max Sales** | **Percentage Above Average** |
|----------------------------|------------------------|-------------------------------|
| Electronic Accessories     | Thursday              | 53.55%                       |
| Fashion Accessories        | Saturday              | 38.91%                       |
| Food and Beverages         | Wednesday             | 36.03%                       |
| Health and Beauty          | Tuesday               | 27.05%                       |
| Home and Lifestyle         | Sunday                | 43.69%                       |
| Sports and Travel          | Saturday              | 32.39%                       |


---
- Product line performance by Hours:

![image](https://github.com/user-attachments/assets/c3b59b41-6a07-471b-b614-9b8f3377b4f5)

## Hourly Performance Analysis by Product Line

| **Product Line**          | **Hour with Max Sales** | **Percentage Above Average** |
|----------------------------|-------------------------|-------------------------------|
| Electronic Accessories     | 19                    | 18.95%                       |
| Fashion Accessories        | 13                    | 36.59%                       |
| Food and Beverages         | 19                    | 59.45%                       |
| Health and Beauty          | 14                    | 53.28%                       |
| Home and Lifestyle         | 17                    | 48.52%                       |
| Sports and Travel          | 19                    | 56.63%                       |


---
- Sales Trend over time:

![image](https://github.com/user-attachments/assets/d0d76dfe-d421-42eb-a173-8239229d04df)

- Month with highest sales: 1
- Percentage by which it exceeds the average sales: 8.02%

---

- Sales Trend in Days of Week:

![image](https://github.com/user-attachments/assets/b01ac67d-0506-4311-83cb-0f526e957059)

| Day Name   | Total       |
|------------|-------------|
| Monday     | 37899.0780  |
| Tuesday    | 51482.2455  |
| Wednesday  | 43731.1350  |
| Thursday   | 45349.2480  |
| Friday     | 43926.3405  |
| Saturday   | 56120.8095  |
| Sunday     | 44457.8925  |


- Day with highest sales: Saturday Day of Week with 56120.8095 sales more than average by 21.64%

---
- Hourly Sales Trend: 

![image](https://github.com/user-attachments/assets/493519b0-d9a7-475e-b7c6-2c0674bcb733)

- Most sales occur at 19 Hour: 35.21 % More than average


---
### Analysis of Payment Types:

- Distribution 

 | Payment Type | Counts |
 |----|----|
 | Ewallet |       345 |
 | Cash    |       344 |
 | Credit card  |  311 |

 ![image](https://github.com/user-attachments/assets/b0d6e1ca-1673-4eb8-9727-44d7cfa3bf1e)

- Ewallet is used for most transactions
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


# Q & A

#### **Q1: Which city generates the highest sales and gross income?**

-   **Answer:**  
    Naypyitaw generates the highest sales and gross income with **110,568.71 in sales** and **5,265.18 in gross income**, surpassing the average by **2.71%**.  
    **Insight:** Focus on strengthening marketing campaigns in Naypyitaw to sustain and expand this lead.

----------

#### **Q2: Which customer type contributes more to sales and gross income?**

-   **Answer:**  
    Members outperform normal customers with **164,223.44 in sales** and **7,820.16 in gross income**, accounting for **3.45% more than average sales** and **2.20% higher quantities sold**.  
    **Insight:** Membership loyalty programs are effective. Consider adding exclusive perks to retain members.

----------

#### **Q3: How does gender influence sales and gross income?**

-   **Answer:**  
    Female customers lead with **167,882.93 in sales** and **7,994.43 in gross income**, contributing **3.96% more to gross income** than males.  
    **Insight:** Tailored promotions for female customers, especially in **Health and Beauty** and **Fashion Accessories**, could increase engagement.

----------

#### **Q4: What is the most profitable day of the week?**

-   **Answer:**  
    **Saturday** has the highest average gross income at **16.30**, which is **6.18% above the weekly average**.  
    **Insight:** Targeted promotions or special events on Saturdays could amplify this trend.

----------

#### **Q5: Which product line has the highest gross income?**

-   **Answer:**  
    **Food and Beverages** leads with **2,673.56 in gross income**, outperforming the average by **4.30%**.  
    **Insight:** Expand offerings in this category and consider bundling strategies to boost sales.

----------

#### **Q6: How do payment methods impact sales and customer preferences?**

-   **Answer:**
    -   **Ewallet** is the most preferred payment method with **345 transactions** but has the lowest average gross income per transaction at **15.18**.
    -   **Cash** payments generate the highest gross income per transaction at **15.53**.  
        **Insight:** Incentivize the use of Ewallet through discounts to maintain its popularity while improving profitability.

----------

#### **Q7: What is the trend in ratings?**

-   **Answer:**
    -   **Branch A (Yangon)** has the highest average rating of **7.03**.
    -   Normal customers have a slightly better satisfaction score (**7.01**) than members (**6.94**).  
        **Insight:** Investigate member feedback to enhance their experience and satisfaction levels.

----------

#### **Q8: When do most sales occur during the day?**

-   **Answer:**  
    The **19th hour (7 PM)** sees the highest sales, **35.21% above the hourly average**.  
    **Insight:** Boost staffing and optimize inventory replenishment during this peak hour to maximize efficiency.

----------

#### **Q9: What are the top-performing days and hours for product lines?**

-   **Answer:**
    -   **Food and Beverages** perform best on **Wednesdays** and at **7 PM**, with sales **82.77% above daily average** and **59.45% above hourly average**, respectively.
    -   **Health and Beauty** sees peak sales on **Tuesdays** and at **2 PM**, with sales **138.88% above the daily average** and **53.28% above hourly average**, respectively.  
        **Insight:** Develop time-specific campaigns for different product lines to leverage these trends.

----------

#### **Q10: Which product line sells the most quantity?**

-   **Answer:**  
    **Electronic Accessories** leads with **971 units sold**, exceeding the average quantity by **5.74%**.  
    **Insight:** Ensure ample stock availability and explore cross-selling opportunities with complementary product lines.

----------

#### **Q11: How does the sales trend evolve over the months?**

-   **Answer:**  
    January exhibits the highest sales, **8.02% above the average monthly sales**.  
    **Insight:** Capitalize on this strong start with new year promotions and clearance sales.

----------

## **Conclusion**

Urban Reach Mart's sales are heavily influenced by **location (Naypyitaw)**, **customer type (members)**, and **timing (Fridays, 7 PM)**. Investing in customer loyalty programs, optimizing peak-time operations, and tailoring promotions to customer demographics can drive sustained growth. Payment incentives and product-specific campaigns could further enhance revenue and customer satisfaction. Businesses can **capitalize on the growing preference for E-wallets** by offering exclusive discounts or rewards for digital payments to further encourage adoption.

