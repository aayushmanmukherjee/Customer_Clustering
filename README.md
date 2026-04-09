# **Shopping Mall Customer Segmentation**

The dataset comprises customer information including Customer ID, age, gender, annual income, and spending score. Spending score is determined by analyzing customer behavior and purchasing data. It aids in understanding customer segmentation for strategic marketing decisions.

[Kaggle link](https://www.kaggle.com/datasets/zubairmustafa/shopping-mall-customer-segmentation-data)

## Dataset
- Customer ID: Purchasing ID (removed during preprocessing)
- Age: Customer Age of customers
- Gender: Customer's gender (dropped for better clustering performance)
- Annual Income: Annual income of customers
- Spending Score: Score assigned on customer behavior and spending nature

## Tools Used
Pandas, Matplotlib, Seaborn, Scikit-Learn

## Approach
1. Data Preprocessing
	- Removed irrelevant columns (Customer ID, Gender)
	- Selected important features:
		- Age
	 	- Annual Income
	    - Spending Score
	- Scaled data using StandardScaler

2. Finding Optimal Clusters
	- Used Elbow Method (Inertia)
	- Used Silhouette Score for validation
	- Final choice: k = 5

3. Model Building
   - Applied K-Means clustering
	- Generated cluster labels for each customer

4. Visualization
	- Used PCA to reduce dimensions (3D → 2D)
	- Visualized clusters using scatter plots

## Customer Segments
- **Cluster 0: Mid-Income High Spenders**
  
  Customers with moderate income but high spending behavior.
   
  Ideal targets for promotions, discounts, and loyalty programs.   
- **Cluster 1: Older Low Spenders**
  
  Older customers with low spending despite moderate income.
  
  Less responsive to marketing; focus on essential-value offerings.
- **Cluster 2: Wealthy Conservative Seniors**
  
  High-income senior customers with low spending patterns.
  
  High potential segment; can be targeted with personalized premium offers.
- **Cluster 3: Young High-Income Moderate Spenders**
  
  Younger customers with high income and moderate spending.
   
  Suitable for upselling and premium product marketing.
- **Cluster 4: Senior Premium Customers**
  
  Older customers with high income and high spending behavior.
   
  Most valuable segment; focus on retention and exclusive services.

## Business Impacts
- Enables **targeted marketing campaigns** for different customer groups  
- Helps identify **high-value and high-potential customers**  
- Improves **customer engagement and retention strategies**  
- Supports **efficient allocation of marketing resources**

## How to Clone this Project

1. Clone the repository:
   ```bash
   git clone https://github.com/aayushmanmukherjee/Customer_Clustering.git
   ```
2. Install Python libraries in a virtual environment:

   - For Mac/Linux
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```

   - For Windows
    ```bash
   python3 -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
   ```
    
3. Run the `.ipynb` file
