FoodHub Data Analysis — Exploratory Data Analysis & Business Recommendations

An exploratory data analysis of ~1,900 food delivery orders for FoodHub, a New York food aggregator app, uncovering demand patterns, delivery performance, and customer rating behavior to drive concrete business recommendations.

The Business Problem

FoodHub connects customers to restaurants through a single app, handling order placement, restaurant confirmation, and delivery tracking end-to-end. With order, rating, cuisine, cost, and timing data captured for every transaction, the goal was to analyze this data as a data scientist would: understand demand patterns across restaurants and cuisines, evaluate delivery performance, and turn findings into recommendations that improve the customer experience and the business.

Dataset

1,898 orders across 9 fields: order ID, customer ID, restaurant name, cuisine type, cost, day of week, customer rating, food preparation time, and delivery time. No missing values.

Analysis Performed
Univariate analysis — distributions of cost, ratings, preparation time, and delivery time across all orders
Multivariate analysis — relationships between cuisine, rating, cost, and delivery/preparation time
Business-driven queries, including:
Top 5 restaurants by order volume
Most popular weekend cuisine
Revenue calculation under FoodHub's tiered commission structure (25% on orders >$20, 15% on orders >$5)
Restaurants qualifying for a promotional offer (50+ ratings, average rating >4)
Weekday vs. weekend delivery time comparison
Top 3 most frequent customers, identified for a targeted discount campaign
Key Findings
~39% of orders went unrated — a major data gap that limits how confidently rating-driven decisions can be made.
Averages were misleading. Spanish cuisine had the highest average rating, but a multivariate breakdown revealed it had only 4 total ratings — American cuisine had both the most 5-star ratings and the highest overall rating volume, making it the more reliable "most-loved" cuisine.
Delivery was slower on weekdays (~28 min) than weekends (~22 min), despite weekend order volume being higher — a counterintuitive result worth operational investigation.
Korean restaurants had the fastest median delivery time, offering a potential internal benchmark for other cuisines to study.
Net revenue across all orders under FoodHub's commission structure: $6,166.30.
Recommendations Delivered
Increase rating capture — incentivize ratings via discount cards or complimentary items for both delivery and dine-in customers, closing the ~39% data gap.
Cross-restaurant knowledge transfer — study how faster cuisines (e.g., Korean) manage delivery logistics and apply learnings to consistently slower ones (French, Vietnamese, Italian).
Targeted intervention for lowest-rated restaurants — audit and address specific experience gaps at the eight lowest-rated restaurants before promoting them further.
Promote high-performing cuisines and deepen partnerships with consistently high-rated restaurants.
Tech Stack

Python, pandas, NumPy, Matplotlib/Seaborn (EDA and visualization), Jupyter Notebook

Files
FDS_Project_LearnerNotebook_FullCode.html — full notebook export with code, visualizations, and analysis
