# ZAALIMA-INTERNSHIP-PROJECT-2-
CUSTOMER SEGMETATION 

📊 Customer Segmentation using K-Means Clustering
Project Overview
This project utilizes unsupervised machine learning (K-Means Clustering) to segment a customer base into distinct groups based on demographic and behavioral data (Age and Estimated Salary). The primary goal is to provide data-driven insights that can inform and enable targeted marketing strategies, optimizing resource allocation and improving conversion rates.

Methodology
The analysis follows a standard data science pipeline:

Data Loading & EDA: Initial data inspection confirms 400 complete records with no missing values. Features include Gender, Age, EstimatedSalary, and the binary target variable Purchased.

Pre-processing: The key features for clustering, Age and EstimatedSalary, were scaled using MinMaxScaler to ensure equal weighting during the clustering process.

Clustering: The K-Means algorithm was applied, identifying an optimal number of 4 clusters (K=4).

Cluster Profiling: Each segment was analyzed based on its average characteristics to define marketing personas.

💡 Key Findings & Segment Profiles (K=4)
The clustering revealed four distinct customer segments, each requiring a different marketing approach:

Cluster ID	Avg. Age	Avg. Salary	Purchase Rate	Marketing Persona & Strategy
1	44.1	$121,654	86.4%	Affluent High-Value Targets: Highly engaged, high-income customers. Strategy: Focus on premium offerings, loyalty programs, and relationship maintenance.
3	51.0	$41,955	83.3%	Older Budget Buyers: Older, lower-income segment with a high tendency to purchase. Strategy: Emphasize product value, necessity, and non-price benefits.
0	35.8	$71,146	11.4%	General Population/Non-Buyers: Moderately aged and salaried customers who have mostly not purchased. Strategy: General awareness campaigns and mid-tier product pitches.
2	26.0	$42,453	0.0%	Young Non-Buyers: Youngest demographic with the lowest purchase rate. Strategy: Marketing aimed at future conversion, focusing on brand building and affordability options.
🛠️ Technologies & Libraries
Language: Python

Core Libraries:

pandas (Data manipulation)

numpy (Numerical operations)

matplotlib / seaborn (Data Visualization/EDA)

scikit-learn (MinMaxScaler, KMeans)

🚀 How to Run the Project
Prerequisites
You need Python installed, along with the required libraries.

Bash

pip install pandas numpy scikit-learn matplotlib seaborn
File Structure
The core files for this project are:

.
├── CUSTOMER_SEGMENTATION.ipynb  # The main Jupyter Notebook for the analysis.
├── Customer_Behaviour.csv         # The dataset used for the analysis (assumed).
└── eda_plots.png                  # Generated visualizations from the EDA phase.
Execution
Clone the repository:

Bash

git clone [YOUR_REPOSITORY_URL]
Navigate to the project directory.

Open the Colab Notebook:

Bash

Colab notebook CUSTOMER_SEGMENTATION.ipynb
Run all cells in the notebook sequentially to reproduce the data loading, pre-processing, clustering, and cluster profiling steps.
