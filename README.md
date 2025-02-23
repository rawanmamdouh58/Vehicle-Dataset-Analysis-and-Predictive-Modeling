# Discription 
This project demonstrates a comprehensive approach to analyzing a vehicle dataset, from data preprocessing and exploratory analysis to building and evaluating predictive models. 
The models developed can be used to predict the fuel type of vehicles, which could be valuable for various applications such as market analysis, environmental impact studies, and vehicle classification systems.  
The use of both classification and clustering techniques provides insights into the dataset from different perspectives, highlighting patterns and relationships among the features.

# Key Steps and Components:

# 1-Data Loading and Preprocessing:
The dataset is loaded from a CSV file using PySpark.

Null values are identified and handled by dropping rows with missing data.

Duplicate rows are removed to ensure data quality.

# 2-Exploratory Data Analysis (EDA):

Descriptive statistics are computed to understand the distribution of numerical features like year and power.

Histograms are plotted to visualize the distribution of categorical features like brand and year.

The most common fuel types and the distribution of body types among the most frequent brands are analyzed.

# Feature Engineering:

String columns like brand, bodyType, and transmission are indexed using StringIndexer to convert them into numerical format suitable for machine learning models.

Features are assembled into a single vector column using VectorAssembler.

# Predictive Modeling:

Decision Tree Classifier: A decision tree model is trained to predict the fuel type (fuelType) based on features like brand, bodyType, transmission, and year. The model achieves an accuracy of approximately 90.69%.

K-Nearest Neighbors (KNN): A KNN model is implemented using scikit-learn to predict the fuel type, achieving an accuracy of approximately 87.45%.

K-Means Clustering: A clustering model is built to group vehicles based on their features, and the silhouette score is computed to evaluate the clustering performance.

# Model Evaluation:

The accuracy of the classification models (Decision Tree and KNN) is evaluated using test data.

The silhouette score is used to assess the quality of the clustering performed by the K-Means model.
