### SCCU Background

SCCU(Swire Coca-Cola United States) tries to optimize logistics by transitioning customers selling below a specific annual volume to an Alternate Route to Market (ARTM). There is an annual 400 gallons volume threshold used to distinguish the customers between the direct delivery route and ARTM. However, SCCU is looking for a more cost-efficient strategy to decide new threshold for optimizing logistics which is driving better operational efficiency and more revenues.
##  My Contribution:
- Led the predictive modeling workflow: data cleaning, feature engineering, and building logistic regression models to identify growth-ready customers.
- Designed and implemented the clustering analysis (KMeans) to optimize delivery routing.
- Conducted before/after cost analysis and visualized results.
- Coordinated integration of technical findings into actionable business recommendations for SCCU.
### SCCU Customer Growth & Delivery Cost Optimization
 # Overview
This project analyzes customer growth patterns and optimizes delivery costs for SCCU using predictive modeling and clustering. By identifying growth-ready customers and optimizing delivery routing, we achieved significant cost reductions and created a scalable framework for future logistics and marketing strategies.
Key Results
# Customer Growth Identification
 - 1,268 customers transitioned from 'below' to 'above' the annual volume threshold (2023 to 2024)
 -  These customers represent high-growth, high-value potential for targeted sales and retention programs

# Predictive Modeling (Logistic Regression)
 -  Accuracy: 87%
 -  Precision (above group): 0.74 | Recall: 0.87 | F1-score: 0.80
 -  The model effectively identifies future growth customers for proactive targeting

# Multi-Dimensional Clustering (ZIP + Volume)
 -  Customers clustered based on ZIP code, annual ordered cases, and gallons
 -  5 optimized clusters support region-specific delivery routing and load planning
 -  Enables smarter delivery zones tailored by order type and customer density

# Gallons vs. Cases Analysis
-  Segmented customers by gallons-per-case ratio to distinguish bulk liquid vs. packaged goods ordering patterns
-  Identified high gallon-per-case customers ideal for liquid delivery planning

# Validated Cost Efficiency: Before vs. After Clustering
##  Delivery Cost Optimization Results

| Scenario             | Avg. Cost per Case | Avg. Cost per Gallon | Savings per Case | Cost Reduction (%) | Savings per Gallon | Cost Reduction (%) |
|----------------------|-------------------:|---------------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| **Before Clustering**|         $40.92     |         $29.95       |        –         |        –           |        –           |        –           |
| **After Clustering** |         $2.19      |         $5.59        |     $38.73       |     94.64%         |     $24.36         |     80.95%         |

*Clustering strategy reduced delivery costs by **94.6% per case** and **80.9% per gallon**.*

Methodology
1 Data Preparation
   -  Cleaned and engineered features from transaction history (2023–2024)
   -  Created target variable: customer transition from 'below' to 'above' threshold

2 Predictive Modeling
   -  Used Logistic Regression to classify growth-ready customers
   -  Balanced classes via manual undersampling for robust modeling

3 Customer Growth Analysis
  -  Counted and profiled customers moving above the threshold year-over-year

4  Clustering
  -  Applied KMeans clustering on improved customers using ZIP code, annual cases, and gallons
  -  Visualized clusters to inform delivery routing and resource allocation

5  Cost Analysis
  -  Compared average delivery costs before and after clustering (both per case and per gallon)
  -  Quantified cost savings and efficiency gains from optimized delivery zones

  -  ##  Difficulties Encountered
  - Integrating and cleaning data from multiple sources with inconsistent formats.
  - Balancing class distributions for predictive modeling.
  - Determining the optimal number of clusters for delivery routing.
  - Translating technical analysis into actionable business recommendations.
  - ##  What I Learned
 - Gained hands-on experience with the full data science pipeline.
 - Learned the importance of business context in analytics.
 - Improved communication skills for presenting technical findings.
 - Discovered the value of iterative experimentation in modeling and clustering.

  - ## Strategic Takeaways
  -  Clustering customers by geography and order behavior dramatically reduces delivery costs
  -  Predictive modeling enables proactive targeting of high-potential growth customers
  -  The approach supports scalable logistics planning with smarter routing and load balancing
  -  Segmentation by order type (cases vs. gallons) allows for tailored delivery strategies

Visualizations
Confusion matrix and classification report for model evaluation
![image](https://github.com/user-attachments/assets/0eb9f30a-fe93-4e59-afc3-7205fd63b41b)

Cluster scatterplots by ZIP code, cases, and gallons
![image](https://github.com/user-attachments/assets/c39b4b62-cf77-45cd-a9be-f25d9ebb6aef)
![image](https://github.com/user-attachments/assets/0eb46fa5-49bc-4b5d-b24c-d7306eb13a13)

Before/after bar charts for delivery cost per case and per gallon
![image](https://github.com/user-attachments/assets/16f2ef1e-9553-4dd8-ac4c-5a1777fb235c)
![image](https://github.com/user-attachments/assets/d53d1095-03f9-47f8-8ad7-adb56c02ee29)

