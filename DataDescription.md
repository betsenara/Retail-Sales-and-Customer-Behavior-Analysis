## Overview

The dataset retail_data.csv includes a total of a million rows and 100+ columns

## Data Source

The dataset is obtained from [Kaggle]([https://www.kaggle.com/datasets/utkalk/large-retail-data-set-for-eda?resource=download])). 

### Detailed Column Descriptions

**Customer Information:**

customer_id: Unique identifier for each customer.\
age: Age of the customer.\
gender: Gender of the customer (e.g., Male, Female, Other).\
income_bracket: Income bracket of the customer (e.g., Low, Medium, High).\
loyalty_program: Whether the customer is part of a loyalty program (Yes/No).\
membership_years: Number of years the customer has been a member.\
churned: Whether the customer has churned (Yes/No) - Target for classification.\
marital_status: Marital status of the customer.\
number_of_children: Number of children the customer has.\
education_level: Education level of the customer (e.g., High School, Bachelor's, Master's).\
occupation: Occupation of the customer.\

**Transactional Data:**

transaction_id: Unique identifier for each transaction.\
transaction_date: Date of the transaction.\
product_id: Unique identifier for each product.\
product_category: Category of the product (e.g., Electronics, Clothing, Groceries).\
quantity: Quantity of the product purchased.\
unit_price: Price per unit of the product.\
discount_applied: Discount applied on the transaction.\
payment_method: Payment method used (e.g., Credit Card, Debit Card, Cash).\
store_location: Location of the store where the purchase was made.\

**Customer Behavior Metrics:**

avg_purchase_value: Average value of purchases made by the customer.\
purchase_frequency: Frequency of purchases (e.g., Daily, Weekly, Monthly, Yearly).\
last_purchase_date: Date of the last purchase made by the customer.\
avg_discount_used: Average discount percentage used by the customer.\
preferred_store: Store location most frequently visited by the customer.\
online_purchases: Number of online purchases made by the customer.\
in_store_purchases: Number of in-store purchases made by the customer.\
avg_items_per_transaction: Average number of items per transaction.\
avg_transaction_value: Average value per transaction.\
total_returned_items: Total number of items returned by the customer.\
total_returned_value: Total value of returned items.\

**Sales Data:**

total_sales: Total sales amount for each customer over the last year - Target for regression.\
total_transactions: Total number of transactions made by each customer.\
total_items_purchased: Total number of items purchased by each customer.\
total_discounts_received: Total discounts received by each customer.\
avg_spent_per_category: Average amount spent per product category.\
max_single_purchase_value: Maximum value of a single purchase.\
min_single_purchase_value: Minimum value of a single purchase.\

**Product Information:**

product_name: Name of the product.\
product_brand: Brand of the product.\
product_rating: Customer rating of the product.\
product_review_count: Number of reviews for the product.\
product_stock: Stock availability of the product.\
product_return_rate: Rate at which the product is returned.\
product_size: Size of the product (if applicable).\
product_weight: Weight of the product (if applicable).\
product_color: Color of the product (if applicable).\
product_material: Material of the product (if applicable).\
product_manufacture_date: Manufacture date of the product.\
product_expiry_date: Expiry date of the product (if applicable).\
product_shelf_life: Shelf life of the product (if applicable).\

**Promotional Data:**

promotion_id: Unique identifier for each promotion.\
promotion_type: Type of promotion (e.g., Buy One Get One Free, 20% Off).\
promotion_start_date: Start date of the promotion.\
promotion_end_date: End date of the promotion.\
promotion_effectiveness: Effectiveness of the promotion (e.g., High, Medium, Low).\
promotion_channel: Channel through which the promotion was advertised (e.g., Online, In-store, Social Media).\
promotion_target_audience: Target audience for the promotion (e.g., New Customers, Returning Customers).\

**Geographical Data:**

customer_zip_code: Zip code of the customer's residence.\
customer_city: City of the customer's residence.\
customer_state: State of the customer's residence.\
store_zip_code: Zip code of the store.\
store_city: City where the store is located.\
store_state: State where the store is located.\
distance_to_store: Distance from the customer's residence to the store.\

**Seasonal and Temporal Data:**

holiday_season: Whether the transaction occurred during a holiday season (Yes/No).\
season: Season of the year (e.g., Winter, Spring, Summer, Fall).\
weekend: Whether the transaction occurred on a weekend (Yes/No).\

**Customer Interaction Data:**

customer_support_calls: Number of calls made to customer support.\
email_subscriptions: Whether the customer is subscribed to marketing emails (Yes/No).\
app_usage: Frequency of usage of the store's mobile app.\
website_visits: Number of visits to the store's website.\
social_media_engagement: Level of engagement with the store on social media (e.g., Likes, Comments, Shares).\
Derived Features (from existing columns):\

days_since_last_purchase: Days since the customer's last purchase.\
avg_purchase_interval: Average number of days between purchases.\
customer_lifetime_value: Predicted lifetime value of the customer.\
loyalty_score: A score representing customer loyalty based on various factors (e.g., membership_years, avg_purchase_value).\
churn_risk_score: A score representing the risk of customer churn based on purchase frequency, recency, and total sales.\

**Linking of Columns Customer Information:**

Columns like customer_id, age, gender, income_bracket, and membership_years are linked to customer demographics and loyalty, which can influence their purchasing behavior, average purchase value, and likelihood to churn.\

**Transactional Data:**

transaction_id is linked to customer_id, providing insights into each customer's purchasing patterns over time.\
product_id, product_category, quantity, unit_price, and discount_applied are linked to the transactional details, influencing total_sales and avg_purchase_value.\

**Customer Behavior Metrics:**

Metrics such as avg_purchase_value, purchase_frequency, and last_purchase_date are derived from transactional data and provide insights into customer behavior and loyalty.\

**Sales Data:**

Columns like total_sales, total_transactions, and total_items_purchased summarize the overall spending and purchasing habits of each customer, directly linked to customer_id and transactional data.\

**Product Information:**

Details such as product_name, product_brand, product_rating, and product_review_count are linked to product_id, providing insights into product performance and customer preferences.\

**Promotional Data:**

Promotional details (promotion_id, promotion_type, promotion_start_date, and promotion_end_date) are linked to transaction_id, influencing purchasing behavior during promotional periods.\

**Geographical Data:**

Geographical details like customer_zip_code, customer_city, and customer_state are linked to store_zip_code, store_city, and store_state, providing insights into the impact of location on purchasing behavior and store performance.\

