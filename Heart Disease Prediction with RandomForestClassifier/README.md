This project aims to predict heart disease diagnoses using the RandomForestClassifier model. The data was divided into 65% for training and 35% for testing. The original dataset contained a significant number of missing values for three variables: the number of major vessels, the thalassemia category, and the slope. To address these missing values, the median and most frequent values were applied. Additionally, all categorical values were converted into numerical types using LabelEncoder to ensure compatibility for training and testing.
The RandomForestClassifier was chosen as it is well-suited for datasets with a multiclass target variable. In this case, the target values represent the severity of heart disease, where 0 indicates no presence of heart disease, 1 indicates mild, 2 moderate, 3 severe, and 4 very severe.
To evaluate the model's performance, a classification report was generated, presenting metrics such as precision, recall, F1-score, and accuracy.
The classification report provides a detailed summary of the performance of a classification model for predicting heart disease. Here's a breakdown of the metrics and their interpretation:
________________________________________
##Metrics Overview:
1.	Precision: Measures the proportion of correct positive predictions out of all positive predictions. It answers, "Of the cases predicted as a specific class, how many were correct?"
2.	Recall (Sensitivity): Measures the proportion of actual positives that were correctly predicted. It answers, "Of the actual cases in this class, how many were detected?"
3.	F1-Score: Harmonic mean of precision and recall, providing a balance between the two.
4.	Support: The number of true instances in each class in the dataset.
________________________________________
##Class-wise Analysis:

Class 0.0:
•	Precision: 0.77 – 77% of predictions for class 0.0 are correct.
•	Recall: 0.94 – 94% of true class 0.0 cases are identified.
•	F1-Score: 0.84 – High precision and recall result in a strong overall performance.
•	Support: 140 – A significant number of samples, contributing to the overall performance.

Class 1.0:
•	Precision: 0.55 – Only 55% of predictions for class 1.0 are correct.
•	Recall: 0.62 – 62% of true class 1.0 cases are identified.
•	F1-Score: 0.59 – Moderate balance between precision and recall.
•	Support: 93 – Moderate representation in the dataset.

Class 2.0:
•	Precision: 0.35 – Low precision indicates many false positives.
•	Recall: 0.24 – Only 24% of true cases are identified.
•	F1-Score: 0.28 – Poor performance due to low precision and recall.
•	Support: 38 – Limited samples may contribute to lower model performance.

Class 3.0:
•	Precision: 0.35 – Similar to class 2.0, precision is low.
•	Recall: 0.17 – The model detects only 17% of true class 3.0 cases.
•	F1-Score: 0.23 – Performance is poor for this class.

Class 4.0:
•	Precision, Recall, F1-Score: 0.00 – The model fails entirely for this class, either due to insufficient training data or severe imbalance.
•	Support: 10 – Very few samples likely contribute to poor results.

##Overall Performance:

•	Accuracy: 0.64 – The model correctly predicts 64% of all samples.
•	Macro Avg (Precision/Recall/F1-Score): ~0.39 – Average performance across all classes, treating each class equally. Low due to poor performance on underrepresented classes.
•	Weighted Avg (Precision/Recall/F1-Score): ~0.60 – Average performance weighted by class support. Higher than macro average because class 0.0 (majority class) performs well and has significant weight.
•	The overall result shows that the model performs well for Class 0, followed by Class 1. However, the model demonstrates poor performance for Classes 2, 3, and 4. This outcome is impacted by the class imbalance in the dataset. The available dataset indicates that the number of heart disease diagnoses is distributed as follows: Class 0 = 411, Class 1 = 265, Class 2 = 109, Class 3 = 107, and Class 4 = 28. Larger class sizes provide more training opportunities, enabling the model to generate better results compared to smaller classes.
•	The model’s accuracy is 0.64, meaning it correctly predicts 64% of all samples. However, for imbalanced datasets like this, accuracy is not always a reliable metric. It is better to focus on metrics such as the F1-score, especially for minority classes. For future projects, data augmentation could be used to generate additional samples for minority classes, improving the model’s generalization and performance.

---------------------------------------------------------------------------------
For the visualization, ROC curve is provided to represent the trade off between True Positive rate and False Positive rate for each class. ROC curve demonstrate how well model can distinguish between the classes. High performance for a class is indicated by an Area Under Curve (AUC) value close to 1, means the model can successfully rank the correct class higher than others for most samples.
