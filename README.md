![mobile2](https://github.com/user-attachments/assets/b8e4e655-51dd-43e7-9070-a87da0851a0d)

# Project Title

Mobile Price Prediction

## Dependencies

Downloads: Jupyter Notebook. 

Libraries to be imported: 

1.  Pandas.
2.  Numpy.
3.  Matplotlib.
4.  SNS.
5.from sklearn.model_selection import train_test_split
6.from sklearn.ensemble import RandomForestRegressor
7.from xgboost import XGBRegressor
8.from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score

## DATA  DESCRIPTION

1.  SOURCE OF MOBILE DATA:  The data used for the analysis is provided by Next Hikes.

2.  FEATURES/VARIABLES INCLUDED:  There are around  12 features and variables included in the data.   The most common and important variables include Memory,  Battery, RAM, Camera, Processor etc.

3.  DATA SIZE AND FORMAT:  The data has around 541 rows and 12 columns in the form of csv.

##  Methodology

1.  Data Loading and Initial Exploration:
	a. Importing the Dataset.
	b. Displaying the First Few Rows of Data
	c. Basic Summary Statistics (mean, median, min, max, etc.)

2.  Data Cleaning and Preprocessing:
	a. Handling Missing Values.
	b. Removing Duplicates.
	c. Checking for Data Integrity Issues.

3.  Exploratory Data Analysis (EDA):
	a. Univariate Analysis:  Conduct a univariate analysis to understand the distribution of key variables 	like house prices. Utilize histograms, kernel density plots, or other visualizations to gain insights into the data.

![1](https://github.com/user-attachments/assets/6f50a734-5916-4ea9-8431-9bc6b3a031b7)

![2](https://github.com/user-attachments/assets/a8f40448-3935-472d-855c-d2536d0f2abf)

![3](https://github.com/user-attachments/assets/658ba95d-cc0a-4569-af64-f3faa7611f95)

b. Multivariate Analysis:  Perform multivariate analysis to understand the correlations and 	dependencies between various
 features. Utilize techniques like
correlation matrices, scatterplots, pairplots, histograms, point plots and violin plots for a comprehensive view.

![4](https://github.com/user-attachments/assets/6c395cb2-2c3a-4467-b3dd-305170208205)

![6](https://github.com/user-attachments/assets/fefb9e71-450c-464b-bb4e-decb44c89458)

![7](https://github.com/user-attachments/assets/5349f5d9-348e-4f17-93cd-c2a5cbcbad12)

![8](https://github.com/user-attachments/assets/6e10df4c-fed9-40a6-94a3-3f4bf682eeba)

![9](https://github.com/user-attachments/assets/81bb18c7-ba00-44b6-a0d1-24e890f765d7)

![10](https://github.com/user-attachments/assets/9b69731a-7691-457d-8c55-08db6a396dce)

![11](https://github.com/user-attachments/assets/20e281a6-a27e-414c-be38-207bee2851da)


5.   Feature Selection:  
Techniques: Use statistical tests, correlation matrices, and domain knowledge to select relevant features for 	model  training.  The below is the most correlated features to the Mobile Price.

![17](https://github.com/user-attachments/assets/e95daea0-815c-4c05-9ef5-78717079eaa1)

Dimensionality Reduction: Apply techniques like Principal Component Analysis (PCA) or feature importance 	ranking to reduce complexity and improve model performance.	It shows that pca is not required as the data has only few number of variables.

5.  Model Selection and Training

	  Regression Models: Worked on different types of regression algorithms with the following accuracy scores.
 
	  1.  Linear Regression:  The R2 score of the Linear Regression Model is too less of 0.44.

	  2.  Decision Tree Regressor:  The R2 score of the Decision Tree Regression Model is	 0.85.
	
	  3.  Adaboost Regressor:  The R2 score of the Adaboost Regression Model is 0.68.

	  4.  XGBoost Regressor:  The R2 score of the XGBoost Regression Model is 0.89.
    
    CONCLUSION:  Based on the above R2 scores XGBoost Regressor was considered as the best suitable model for the Mobile Price Prediction         

  Measuring other Metrics like Mean absolute Error and Root mean squared error through xgboost.  The results are as follows:
  R2 score using XGBoost Regressor:   0.89.			
  Mean absolute Error using XGBoost Regressor:  1118.87
  Room Mean Squared Error using XGBoost Regressor:  2375.79.

  Creating a dataframe with variables and corresponding feature importances.  The results are as follows:

  ![12](https://github.com/user-attachments/assets/08f33188-cae1-4cce-93f3-76b009a040c1)

  ![13](https://github.com/user-attachments/assets/560856b7-e8d1-4691-805a-db0c5f52aa91)

  
Different type of plots for actual vs predicted values like pointplot, scatter plot, joint plot, density plot and box plot for a comprehensive view.

![14](https://github.com/user-attachments/assets/016432e0-663d-4926-bea8-ea45257c2836)

![15](https://github.com/user-attachments/assets/68c74798-2f87-485c-8d23-c9237c64fb69)

![16](https://github.com/user-attachments/assets/eff1ff18-8a78-4eac-9c2b-7ec4dc4f42fe)

![18](https://github.com/user-attachments/assets/37a08739-ffaa-497a-9989-b21900576253)

![19](https://github.com/user-attachments/assets/f9f1f4e7-7e4e-4d49-9a44-a925304adce8)

## Dependencies

Based on the feature importance values provided for mobile price prediction, here’s a conclusion drawn:
1.  MEMORY: Memory capacity (likely referring to internal storage) is the most influential feature for predicting mobile phone prices. Phones with higher storage capacities generally command higher prices.

2.  BATTERY: Battery capacity or battery life is the second most important feature. This suggests that phones with longer battery life or larger battery capacities tend to have higher prices.

3.  RAM: Random Access Memory (RAM) plays a moderately important role in price prediction. Higher RAM allows for smoother multitasking and better performance.

4.  DUAL CAMERA: Having a dual camera setup is also a notable factor but less influential compared to memory, battery, and RAM.
PROCESSOR: The type or performance of the processor is moderately influential.

5.  MODEL: The specific model or brand of the phone has some impact on price prediction.

6.  MOBILE HEIGHT: Mobile phone dimensions (likely referring to physical size or design aspects) contribute marginally to price prediction.

7.  COLOR: The color of the phone has minimal impact on pricing compared to other technical specifications. However, certain colors or finishes may appeal more to specific consumer demographics, influencing pricing to a small extent.

8.AI LENS: The presence of AI lens features has negligible impact on price prediction. This suggests that while AI technology is a trending feature, its direct influence on pricing may be minimal compared to other hardware specifications.

## Acknowledgment

 I would like to express my special thanks of gratitude to my Mentor, "Ms. Swetha Sutar" for the guidance and support by giving some reference articles by which I was very much succesful in understanding and completing my project.
