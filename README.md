# **Breast Cancer Prediction with Cross Validation Scores**

This project focuses on predicting breast cancer using machine learning models through cross-validation techniques. The dataset utilized in this study is the Breast Cancer Wisconsin (Diagnostic) dataset, which contains features computed from digitized images of fine needle aspirates (FNA) of breast masses. Each instance in the dataset describes the characteristics of cell nuclei present in these images. 

The dataset comprises 569 instances, with each instance having 30 real-valued features that describe the cell nuclei's properties. These features include measurements such as radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension. For each feature, the mean, standard error, and worst (largest) values are recorded, providing a comprehensive description of each cell nucleus. 

The classification task involves distinguishing between malignant (212 cases) and benign (357 cases) tumors. To achieve this, various machine learning models are trained and evaluated using cross-validation to ensure robust performance. The goal is to develop a reliable predictive model that can assist in the early detection and diagnosis of breast cancer, thereby improving patient outcomes. This dataset is publicly available and can be accessed through the UCI Machine Learning Repository or the University of Wisconsin-Madison's CS FTP server.

## **Data Exploration and Preprocessing**

- Imported the required libraries and loaded the dataset.
- Explored the dataset, including checking for null values, duplicate values, and the distribution of the target variable.
- Encoded the target variable (diagnosis) as 1 for malignant and 0 for benign.
- Analyzed the correlation between features using a heatmap and identified highly inter-correlated features.
- Created a new dataframe by removing the highly inter-correlated features to see the impact on model performance.

## **Model Evaluation and Comparison**

- Implemented a function to perform 5-fold cross-validation on the dataset.
- Trained and evaluated the following models:
    - Logistic Regression
    - Support Vector Machine
    - Gaussian Naive Bayes Classifier
    - Decision Tree Classifier
    - Random Forest Classifier
- Compared the cross-validation scores for the models on both the original and the cleaned datasets.
- Observed that the Random Forest Classifier performed the best, achieving a cross-validation score of around 95%.

## **Conclusion**
The results suggest that removing highly inter-correlated features may not always lead to better performance, as it depends on the dataset and the model used. In this case, the Random Forest Classifier achieved the highest cross-validation score of around 95%, indicating its effectiveness in predicting breast cancer from the given dataset.

## **Future Work**
- Explore additional feature engineering techniques to further improve the model's performance.
- Investigate the importance of individual features and their contribution to the model's predictions.
- Experiment with other machine learning algorithms and ensemble methods to potentially achieve even higher accuracy.
- Deploy the trained model in a real-world setting to assist in the early detection and diagnosis of breast cancer.

## **Acknowledgments**
The authors would like to acknowledge the University of Wisconsin-Madison and the UCI Machine Learning Repository for providing the Breast Cancer Wisconsin (Diagnostic) dataset used in this project