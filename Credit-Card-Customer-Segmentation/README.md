# Credit Card Customer Segmentation using K-Means Clustering

## Project Overview
This project segments credit card customers into distinct groups based on their spending behavior, credit utilization, and payment patterns using unsupervised machine learning (K-Means clustering).

## Business Problem
Banks need to understand different customer segments to:
- Offer personalized marketing campaigns
- Improve customer retention
- Identify high-risk customers
- Optimize credit limit allocation

## Dataset
- **Source**: CC GENERAL.csv
- **Records**: 8,950 credit card customers
- **Features**: 18 behavioral and demographic attributes

## Methodology
1. **Data Preprocessing**: Handled missing values using median imputation
2. **Feature Engineering**: Created `PAYMENT_UTILIZATION` (Balance/Credit_Limit)
3. **Feature Selection**: Used correlation analysis to select key features
4. **Clustering**: Applied K-Means with optimal k=4 determined by Elbow Method
5. **Analysis**: Profiled and interpreted each customer segment

## Key Features Used
- BALANCE
- PURCHASES  
- CREDIT_LIMIT
- PAYMENTS
- PAYMENT_UTILIZATION (engineered feature)

## Results: 4 Customer Segments Identified

| Cluster | Profile Name | Characteristics |
|---------|--------------|-----------------|
| 0 | High Limit, Moderate Users | High balance ($5,077), high credit limit ($9,508), medium utilization (58%) |
| 1 | Low-Risk, Casual Users | Low balance ($414), moderate spending ($879), low utilization (11%) |
| 2 | High-Risk, Cash-Dependent | Medium balance ($1,720), low spending ($438), very high utilization (80%) |
| 3 | Big Spenders, Good Payers | High balance ($4,252), very high spending ($10,687), low utilization (35%) |

## Business Applications
- **Cluster 2**: Target for financial health programs and debt management
- **Cluster 3**: Premium customers for loyalty rewards and card upgrades  
- **Cluster 1**: Low-risk customers for basic card offerings
- **Cluster 0**: Potential for credit limit increases and cross-selling

## Technologies Used
- Python, Pandas, NumPy
- Scikit-learn (KMeans, StandardScaler)
- Seaborn, Matplotlib for visualization
- Jupyter Notebook

## How to Run
1. Clone repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run Jupyter notebook: `jupyter notebook credit_card_segmentation.ipynb`
