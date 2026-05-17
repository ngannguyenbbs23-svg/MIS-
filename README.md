1. Data Overview
   
The Supermarket Sales dataset was selected for this analysis to explore retail sales performance and customer purchasing behaviour. The dataset contains transactional sales data collected from supermarket branches operating across multiple cities. It provides valuable business information that can be used to analyse consumer trends, product demand, and branch performance.

The dataset contains 254 rows (including rows of variables, 253 if not including rows of variables) and 8 columns. Each observation represents a unique sales transaction identified by a sale ID. The variables included are: sale_id, branch, city, customer_type, product_name, product_category, quantity, and total_price. Together, these variables capture important aspects of supermarket operations, including customer segmentation, product categories, sales volume, and revenue generation.

This dataset is appropriate for exploratory data analysis because it enables the examination of relationships between product categories, customer types, and sales outcomes. By applying descriptive statistics and data visualisation techniques, the analysis can generate insights that help businesses improve operational efficiency, understand customer behaviour, and optimise sales strategies.


2. Data Cleaning
   
2.1. Missing values

During the data cleaning process, missing values were identified in several columns of the dataset. The missing values were handled differently depending on the data type of each variable.

<img width="494" height="193" alt="image" src="https://github.com/user-attachments/assets/c3ff87a7-2878-4b69-9b4e-91528880b137" />

For the categorical variables customer_type and product_category, missing values were replaced using the mode (most frequent value). This method was considered appropriate because categorical data represents labels or groups rather than numerical measurements. Replacing missing values with the most frequently occurring category helps preserve the overall distribution of the dataset and reduces the risk of introducing inconsistent or unrealistic values into the analysis.

For the numerical variable quantity, missing values were replaced using the median value. The median was selected because it is less sensitive to extreme values or outliers compared to the mean. Since purchase quantities may vary significantly between transactions, using the median provides a more reliable representation of the typical purchasing quantity within the dataset.

Applying different handling methods according to the nature of each variable improved the overall quality, consistency, and reliability of the dataset. As a result, the cleaned dataset became more suitable for descriptive statistical analysis and data visualisation, allowing more accurate business insights to be generated from the analysis.

2.2. Duplicate row 

After handling missing values, the dataset was examined to identify duplicate records. Detecting duplicate rows is important because repeated transaction records may distort descriptive statistics and lead to inaccurate business insights. 

<img width="707" height="264" alt="image" src="https://github.com/user-attachments/assets/91696f15-a04f-4412-8bb3-db384c47757a" /> 

Figure 1: Result of duplicate row checking using Excel Remove Duplicates feature

The dataset was checked using Excel’s Remove Duplicates feature across all columns. The checking process identified 3 duplicate rows, which were subsequently removed from the dataset. After removing the duplicated records, the dataset contained 250 unique observations and was considered suitable for further analysis. 

<img width="475" height="107" alt="image" src="https://github.com/user-attachments/assets/307b47e0-7b63-4d73-b93c-2207c21a071a" /> 

After cleaning, no missing values or duplicate records remained.


3. Descriptive Statistics
   
3.1. Numerical Variables Summary
   
<img width="471" height="194" alt="image" src="https://github.com/user-attachments/assets/47e36c1f-acef-4842-8e2d-32461fb6f7a1" /> 

Table 1. Summary Statistics of Numerical Variables

The descriptive statistics indicate that the average quantity purchased per transaction is 10.62 items, with most purchases ranging between 5 and 16 items. This suggests moderate purchasing behaviour among customers.
Additionally, the total price variable has a relatively high standard deviation compared to its mean, indicating considerable variation in customer spending. Some transactions generate significantly higher revenue than others.

3.2. Categorical Variables Summary

<img width="468" height="103" alt="image" src="https://github.com/user-attachments/assets/3a459495-d095-4ffe-8793-abe330d23e1d" /> 

Table 2: Summary of Categorical Variables 

The categorical variable summary shows that Branch A appears most frequently in the dataset, accounting for the majority of transactions. In addition, New York records the highest number of sales among all cities.
The “Member” customer type is slightly more common than “Normal” customers, suggesting that loyalty membership may play an important role in customer engagement. Furthermore, “Fruits” is the most frequently purchased product category, indicating strong customer demand for grocery-related products.

3.3. Revenue by Product Category

<img width="467" height="124" alt="image" src="https://github.com/user-attachments/assets/775496df-5147-4f5e-a9bf-d4f5636463a3" /> 

Table 3: Revenue by Product Category 

<img width="410" height="248" alt="image" src="https://github.com/user-attachments/assets/fb92f154-c9e9-4cbd-9ba0-cabdf4cc9bd0" /> 

Figure 2: Total Revenue by Product Category

The “Fruits” category generated the highest total revenue, contributing more than $8,000 in sales and recording the largest number of transactions among all product categories. This suggests that fruit products are highly demanded and play a significant role in the supermarket’s overall revenue performance.

In contrast, the “Personal Care” category recorded the lowest total revenue and the fewest transactions. This may indicate lower customer demand compared to other product categories.

Additionally, “Stationery” achieved the highest average revenue per transaction, suggesting that customers tend to spend more per purchase in this category.

3.4. Revenue by Customer Type

<img width="465" height="61" alt="image" src="https://github.com/user-attachments/assets/bab37490-e158-4a0d-8bc5-c9f96a555f7e" /> 

Table 4: Revenue by Customer Type

<img width="416" height="256" alt="image" src="https://github.com/user-attachments/assets/e1a7c318-8801-4c68-8979-551ff139561f" /> 

Figure 3: Total Revenue by Customer Type

Member customers generated higher total revenue than normal customers, contributing approximately $17,939.55 in total sales. In addition, member customers also recorded a higher average revenue per transaction, indicating stronger purchasing behaviour.

These findings suggest that loyalty membership programs may positively influence customer spending and overall sales performance. Encouraging more customers to become members could help increase long-term revenue growth.


4. Key insights
   
4.1 High Revenue Contribution from the Fruits Category

The analysis showed that the “Fruits” category generated the highest total revenue, contributing approximately $8,024.90 across 64 transactions. Figure 2 also shows that the Fruits category recorded the highest transaction frequency among all product categories. 

This finding suggests that fruits are highly demanded products and play an important role in overall supermarket revenue. Since fruits are essential daily-consumption items, customers are more likely to purchase them regularly, resulting in stable sales performance. From a business perspective, the supermarket should prioritise inventory management and promotional strategies for this category to maximise revenue and maintain customer satisfaction.

4.2 Higher Spending Behaviour Among Member Customers

The analysis revealed that member customers generated approximately $17,939.55 in total revenue, which was higher than the $13,106.73 contributed by normal customers. In addition, member customers recorded a higher average spending value per transaction, as illustrated in Figure 3.

This finding suggests that loyalty membership programs may positively influence customer purchasing behaviour and encourage repeat purchases. Member customers appear to be a more valuable customer segment because they contribute more consistently to supermarket revenue. Therefore, the supermarket should continue strengthening membership programs through rewards, discounts, and personalized promotions to improve customer retention and support long-term revenue growth.


5. Conclusion
   
Overall, the exploratory data analysis identified important patterns in customer purchasing behaviour, product performance, and revenue distribution. The findings suggest that product categories and customer membership status significantly influence supermarket sales performance and can support future business decision-making.
