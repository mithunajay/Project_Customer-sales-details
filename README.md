1. Exploratory Data Analysis (EDA)
•	Objective: Understand the customer and transaction data for insights.
•	Insights Gained: 
o	The dataset contained profile details (e.g., age, location) and transaction behaviours (e.g., spending and frequency).
o	High-value customers exhibit significantly higher transaction frequency and spend more per transaction.
o	Spending patterns reveal seasonal trends and preferences for specific products.

2. Lookalike Model
•	Objective: Identify potential customers similar to existing high-value customers.
•	Steps Involved:
o	Feature extraction from customer data (e.g., age, location, average spending).
o	Trained a similarity-based model using cosine similarity to find customers matching the profile of high-value customers.
o	Generated a list of lookalike customers with rankings.
•	Output:
o	A ranked list of 100+ potential customers most similar to high-value profiles.
o	This lookalike segment can be targeted for personalized campaigns to maximize ROI.

3. Customer Clustering
•	Objective: Segment customers into clusters based on transaction and profile data to identify behavioral groups.
•	Approach:
o	Used KMeans clustering with 4 clusters (optimal based on DB Index).
o	Features included total spending, transaction count, and average transaction value.
•	Cluster Insights:
o	Cluster 0: High-frequency, high-spending customers (loyal customers).
o	Cluster 1: Average spenders and moderately frequent customers (growth segment).
o	Cluster 2: Low-frequency, low-spending customers (requires engagement).
o	Cluster 3: High-value but infrequent customers (premium customers).
•	Metrics:
o	DB Index: 0.42 (good clustering quality).
o	Silhouette Score: 0.56 (moderately well-defined clusters).
o	Inertia (WCSS): 102.3.
•	Visualization: Clusters were visualized on a spending vs. transaction frequency graph.

