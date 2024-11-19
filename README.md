# Visual-Taxonomy-Meesho


1. Introduction
This project focuses on predicting multi-label attributes for images using a hybrid approach. A custom Convolutional Neural Network (CNN) is employed for feature extraction, and XGBoost classifiers are trained for predicting each attribute. The solution includes detailed data preprocessing, feature engineering, and model training on a multi-class, multi-label dataset.

2. Data Preprocessing :
   1. Missing Values: Missing values in attribute columns were filled using random imputation based on existing values within the same category.
   2. Irrelevant Attributes: Missing or irrelevant attribute values were replaced with the placeholder DV.
   3. Encoding: Categorical attributes were encoded using LabelEncoder.

3. Modeling Approach :
   1. Feature Extractor: A custom CNN with convolutional and pooling layers was implemented for feature extraction.
   2. Classifiers: XGBoost classifiers were chosen for each attribute due to their efficiency and performance in multi-class classification tasks.

Remarks:
1. The training on CPU may have taken longer compared to GPU-based training, but the results demonstrate the feasibility of achieving competitive performance without GPU resources.
2. The model's performance varies across attributes, indicating that some attributes may benefit from further optimization, such as hyperparameter tuning or enhanced preprocessing.
3. Future improvements can explore distributed computing or cloud-based GPU resources to accelerate training and experimentation.

