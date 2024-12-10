# Bike Sales Dashboard

The Bike Sales Dashboard is a comprehensive tool developed using the ELK (Elasticsearch, Logstash, and Kibana) stack to visualize and analyze sales data from the European bike market. This dashboard extracts valuable insights from a dataset containing detailed information about transactions across various countries and states in Europe.

## About Dataset<br>
In Europe bikes dataset , Extract the insight of sales in each country and each state of their countries.<br>
In this dataset 18 columns and main column is sales.<br>
[Dataset](https://www.kaggle.com/datasets/sadiqshah/bike-sales-in-europe)<br>

### Column description:
- Date: The specific calendar date of the transaction.<br>
- Day: The day of the week the transaction occurred.<br>
- Month: The month when the transaction took place.<br>
- Year: The year of the transaction.<br>
- Customer_Age: The age of the customer making the purchase.<br>
- Age_Group: The categorized age range of the customer (e.g., Youth, Adults, etc.).<br>
- Customer_Gender: The gender of the customer (M for Male, F for Female).<br>
- Country: The country where the transaction occurred (e.g., Canada, Australia, etc.).<br>
- State: The specific state within the country where the transaction happened.<br>
- Product_Category: The broad category of the product sold (e.g., Accessories, Bikes, etc.).<br>
- Sub_Category: A more detailed classification of the product (e.g., Helmets, Jerseys, etc.).<br>
- Product: The specific product sold, identified categorically.<br>
- Order_Quantity: The number of units of the product purchased in the transaction.<br>
- Unit_Cost: The cost per unit of the product to the seller.<br>
- Unit_Price: The price per unit of the product for the customer.<br>
- Profit: The monetary gain from the transaction (Revenue - Cost).<br>
- Cost: The total cost incurred by the seller for the order (Order_Quantity × Unit_Cost).<br>
- Revenue: The total money earned from the transaction (Order_Quantity × Unit_Price).<br>

## Dashboard
![Complete Dashboard](https://github.com/user-attachments/assets/d27eae90-e264-4bf7-92a9-e4254ce06918)

[ELK_Dashboard_Video.webm](https://github.com/user-attachments/assets/97faec29-08c1-4621-b8ac-98352e7b573f)

## Charts<br>

1. Which age group contributes the most revenue to the business product category wise?<br>
![Graph -1](https://github.com/user-attachments/assets/cce62f8a-b604-42b6-b68b-4c221c7cda02)
The graph shows that **Adults (35-54)** generate the highest revenue across all product categories, with **clothing** being the dominant contributor, followed by **Accessories**. **Young Adults (25-34)** rank second in revenue, while **Youth (<25)** contribute the least. This indicates that marketing efforts should focus on **Adults** and enhancing engagement with the **younger age group**.<br>

2. How has the revenue trended over time compared to profit?<br>
![Graph -3](https://github.com/user-attachments/assets/bd00d6b9-5ae8-4af3-b02c-01292d6ddbc5)
The graph shows that revenue is consistently higher than profit over time, with significant fluctuations in both. A notable gap exists between revenue and profit, suggesting high operating costs or expenses. This dynamic environment highlights the need for deeper analysis to identify causes of volatility, manage risks, and leverage periods of growth.<br>

3. How does revenue change over time?<br>
![Graph -2](https://github.com/user-attachments/assets/cdbebb72-f1dc-49b2-adb7-5cebbe3bbe38)
Revenue spikes occur periodically without a steady trend, reflecting dynamic customer behavior or event-driven sales. Understanding the drivers of these peaks (e.g., promotions or seasonal demand) can help smooth revenue fluctuations and optimize strategies for periods of lower activity.<br>

4. What are the top 5 sub-categories by profit margins, and how do they compare?<br>
![Graph -4](https://github.com/user-attachments/assets/d86a96f9-05d6-408f-9d50-ff27dfe7c8b4)
The key insight is that **Bottles and Cages** lead profit margins **(58.52%)**, followed by **Bike Racks (21.98%)** and **Bike Stands (14.58%)**, while **Cameras and Electronics** are relatively low **(4.92%)**. This indicates the need to focus on the most profitable categories to drive profitability further while exploring opportunities to improve lower-margin products.<br>

5. Which states have the highest sales revenue for the top 6 products?<br>
![Graph -8](https://github.com/user-attachments/assets/b017d811-acbb-4d4e-a16b-93b3a4be2fa0)
**California** leads in **product sales**, with **British Columbia** and **England** also showing strong performance. Other states show moderate sales, indicating a need to focus efforts on these top-performing regions and products for better overall revenue.<br>

6. What are the key regions for further investment and growth opportunities?<br>
![Graph -5](https://github.com/user-attachments/assets/894ac8bb-c8b5-4290-a78d-f3848e73b60d)
The map highlights Country-wise Profit, with **Canada** and the **United States** showing the highest profitability, followed by select regions in **Europe**. **Asia** and **Oceania** show growth potential, while **South America** and **Africa** contribute minimally. A focus on optimizing top markets, while strategies for expanding in Asia and Oceania, and penetrating low-performing regions, can drive global growth. <br>

7. How do different product types compare in revenue contribution?<br>
![Graph -10](https://github.com/user-attachments/assets/c97b54f4-636b-4d6c-b220-e39acd76d552)
This word cloud highlights the top products by revenue, emphasizing items like the **Hitch_Rack_4_Bike** and **AWC_Logo_Cap**, which stand out as major revenue drivers followed by **All_Purpose_Bike_Stand** and **Mountain_Bottle_Cage**.<br>

8. What is the Country wise Ordered Quantity?<br>
![Graph -9 (1)](https://github.com/user-attachments/assets/a73927e5-5caf-4eaa-b131-96f99e67b02b)
The **United States** leads in order quantity **(109,830 units)**, followed by Australia (61,395 units). While maintaining dominance in the U.S., strategies to boost sales in underperforming regions like Germany and "Others" could unlock additional growth potential..<br>

9. What proportion of total revenue is contributed by profit, and how does the average unit cost compare to the average unit price?<br>
![Graph -6](https://github.com/user-attachments/assets/dc4ff53f-050d-46be-a9b0-6a0da63e912e)
![Graph -7](https://github.com/user-attachments/assets/5d798dc7-17e0-4032-9d9e-d70f2698daf2)
Profit constitutes **50.3%** of total revenue **($1.39M of $2.75M)**, indicating a healthy profit margin.<br>
With an average unit cost of **$5.76** making up **42.7%** of the average unit price **($13.50)**, the business maintains a strong profit margin.<br>

## Managerial Insights<br>
- Customer-Centric Marketing and Engagement<br>
  - **Prioritize the Adult Demographic (35–54)**: This age group generates the highest revenue across all product categories, particularly Clothing. Allocate marketing resources to campaigns targeting Adults, emphasizing Clothing and related accessories.<br>
  - **Expand Youth Engagement (<25)**: Youth (<25) contribute the least revenue, suggesting an opportunity to develop targeted campaigns and affordable product options to engage and grow this segment..<br>

- Regional Investment Prioritization<br>
  - **Enhance Performance in High-Revenue Markets**: North America (U.S. and Canada) and Europe are the strongest revenue-generating regions. Prioritize resource allocation, marketing, and supply chain optimization in these markets<br>
  - **Develop Potential in Emerging States**: States with moderate sales, such as South America and Africa, could benefit from increased promotional efforts, particularly improving distribution channels or launching region-specific products.<br>

- Profit-Oriented Product Strategy<br>
  - **Promote High-Margin Products**: Products like "Hitch_Rack_4_Bike" and "AWC_Logo_Cap" drive significant revenue.. Focus marketing and production efforts on these high-performing items to boost overall profitability.<br>
  - **Revise Strategy for Lower-Margin Products**: Evaluate sub-categories with lower profit margins and assess the feasibility of reducing production or enhancing value propositions.<br>

- Revenue and Profit Optimization<br>
  - **Close Revenue-Profit Gap**: The significant gap between revenue and profit highlights high operating costs. Conduct a cost analysis to identify inefficiencies in manufacturing, logistics, or marketing and implement measures to optimize expenditure.<br>
  - **Revenue and Profit Volatility**: Significant fluctuations in revenue and profit suggest a dynamic business environment. Investigating the underlying drivers of this volatility, such as promotions, seasonal demand, or market-specific factors, is essential. Implementing strategies to stabilize revenue trends while leveraging peak periods can enhance financial performance.<br>
  - **Implement Strategic Pricing Models**: With the average unit price significantly higher than the unit cost, consider introducing price segmentation strategies (e.g., premium pricing for high-demand products) to enhance profitability.<br>

- Market Expansion and Growth Strategies<br>
  - **Strengthen Leadership in Key Regions**: The U.S. leads in order quantities, followed by Australia, highlighting their importance as primary markets. Efforts should focus on maintaining this dominance.<br>
  - **Expand Market Share in Under performing Regions**: Regions like South America and Africa have the lowest revenue and order quantities. Implement localized marketing, improve distribution, and assess product relevance to penetrate these markets effectively.<br>

## Conclusion<br>

To drive growth, the business should focus on high-performing markets like the U.S. and Australia while exploring emerging regions such as South America and Africa. Targeted marketing to adults (35–54) and engaging the youth segment will expand the customer base. Prioritizing high-margin products and optimizing costs will improve profitability. Addressing revenue and profit volatility through strategic pricing and cost management will stabilize performance. A balanced approach to market expansion and cost optimization will ensure sustained growth and strengthen the business’s competitive edge.
