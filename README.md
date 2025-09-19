# Food-Delivery-Cost-and-Profit-Analysis
Problem Statement

In the highly competitive food delivery market, managing costs and maintaining profitability is critical for businesses. Delivery fees, commissions, and operational expenses can directly impact profitability, making it essential to analyze key metrics such as order values, delivery fees, commission rates, and payment methods. This project aims to develop an interactive Power BI dashboard to provide insights into delivery costs, profitability by restaurant, order trends, and customer behavior.

Project Goals
Profitability Analysis : Measure profits per restaurant, per order, and by time period (daily/monthly).

Delivery Cost Insights : Analyze the impact of delivery fees and commission rates on profitability.

Customer Behavior : Understand order patterns by analyzing customer preferences in payment methods, peak order times, and delivery durations.

Restaurant Performance : Identify the top-performing restaurants based on order value, delivery fees, and profitability.

Interactive Visualizations : Enable users to filter data by restaurant, order date, payment method, or delivery fee for detailed insights.

Data Source
The data used for this project was sourced from internal delivery records. It contains information on :

https://www.kaggle.com/datasets/romanniki/food-delivery-cost-and-profitability

Data Preprocessing Involved
Data Cleaning
Handling missing values: Identified and removed rows with missing or incomplete data (e.g., null customer IDs or delivery times).
Removing duplicates: Eliminated any duplicate orders from the dataset.
Standardizing text data: Fixed inconsistent naming of restaurants, payment methods, and delivery statuses.
Data Transforamtion
Converted order dates and delivery times to appropriate datetime formats for time-based analysis.
Identified outliers in order values and delivery fees, which were transformed to ensure they didn’t skew analysis.
Created new calculated fields such as
Total Cost = Delivery Fee + Commission Fee + Payment Processing Fee
Profit per Order = Order Value – Total Cost
Data Integration
Merged restaurant details with order records to calculate total profitability per restaurant.
Combined customer and order data to analyze repeat customers and their impact on profitability.
Data Validation
Verified data alignment to ensure that no restaurant or customer had duplicate orders or mismatched payment methods.
Steps Followed
Step 1 : Load the dataset onto Power Query Editor.

Step 2 : Data transformation based on the requirements. Included steps like creating tables like Date, Measures and other metrices.

Step 3 : Created the following measures to extract key statistics from dataset:

image

image

Step 4 : Rectified the Relational Model by linking Primary keys, foreign keys and updating table cardinalities. image

Step 5 : Visualized the dashboard structure based on three key questions:

  Q1. What type of data is being dealt here?
   Ans. Time series data, categorical, geospatial and hierarchical.

  Q2. What am I trying to communicate here?
   Ans. Comparison between categories over time, depicting compositions.

  Q3. Who is the end-user?
   Ans. The Viewers           
Step 7 : Created three pages to provide different insights to the viewer:

Overview insights
Customer Insights
Restaurant Performance
Time-Series Analysis
Step 8 : The dashboard was complete with all my target requirements being met. Finally, I linked all the pages using Buttons to facilitate smooth navigation.

Step 9 : Uploaded the entire Dashboard to PowerBI Service.

Key Insights from the Food Delivery Cost & Profitability Analysis
Restaurant Performance:

The top 3 restaurants generated over 30% of the total profit, demonstrating a clear advantage in customer preference.
Restaurants with higher delivery fees didn’t necessarily have higher profits, suggesting that optimal pricing strategies matter.
Customer Insights:

Cash on Delivery accounted for 60% of the payment methods, indicating customer preference despite the trend toward online payments.
Peak order times were between 7 PM and 10 PM, with the highest order values recorded on weekends.
Delivery Fee and Profit Correlation:

A moderate positive correlation was found between delivery fees and profit, but high fees led to fewer repeat orders.
Outliers with small orders but high delivery costs reduced overall profitability.
Profitability Trends:

Orders with optimized delivery fees and minimal commission charges contributed significantly to profitability.
Restaurants offering discounts saw higher order volumes, but their overall profit margins were lower.
Challenges Faced During the Project
Data Limitations:

Incomplete data: Some orders lacked key information such as delivery times or processing fees.
Outliers: Several extreme values needed transformation to avoid skewing the results.
Technical Issues:

Performance challenges: Complex DAX calculations and large datasets slowed down Power BI during filtering.
Data model alignment: Creating proper relationships between orders, customers, and restaurants required manual adjustments.
Future Improvements for the Project
Real-Time Data Integration: Incorporate live order data feeds to monitor delivery performance and profitability dynamically.
Predictive Analytics: Use machine learning to forecast future profits and identify top-performing restaurants.
Deeper Customer Insights: Expand the dataset to include customer demographics for more targeted analysis.
Advanced Visualizations: Add heat maps to highlight high-profit delivery zones and time-series animations to capture trends over time.
Optimization for Large Data: Improve dashboard performance when handling large datasets by optimizing data models, reducing file size, and incorporating efficient query techniques for smoother user experience.
Conclusion
The Food Delivery Cost & Profitability Analysis dashboard provides valuable insights into order trends, customer behavior, and restaurant performance. It enables stakeholders to make data-driven decisions by identifying key areas of improvement in delivery strategies, pricing models, and cost optimization.
