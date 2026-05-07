# Credit-card-fraud-detection-using-clustering-
This project focuses on detecting fraudulent credit card transactions using unsupervised machine learning techniques, specifically clustering. Unlike traditional classification problems, fraud detection is challenging because fraudulent transactions are rare and highly imbalanced, making it difficult to train supervised models effectively.
### Objective
## The main objective of this project is to:
* Detect unusual credit card transactions
* Apply clustering techniques for anomaly detection
* Evaluate clustering performance against actual fraud labels
* Visualize anomalies using PCA
## Dataset
The dataset contains credit card transactions made by European cardholders.
Features:
Numerical transaction features
Time
Amount
Class
0 → Normal Transaction
1 → Fraudulent Transaction
The dataset is highly imbalanced because fraud cases are very rare.
## Technologies Used
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Project Workflow
## 1. Data Understanding
Loaded the dataset
Checked dataset shape and columns
Identified missing values
Analyzed class distribution
Observation
Most transactions are normal, while only a very small percentage are fraudulent. This makes it an anomaly detection problem.
## 2. Data Preprocessing
Removed the Class column from training data
Applied feature scaling using StandardScaler
Prepared the dataset for clustering
## 3. Clustering using K-Means
Applied the Elbow Method to determine optimal clusters
Trained the K-Means model
Assigned cluster labels to transactions
## 4. Anomaly Detection
Calculated distance of each transaction from cluster centroids
Selected the top 1% farthest points
Marked them as anomalies
Logic
Transactions far away from cluster centers are considered unusual and potentially fraudulent.
## 5. Model Evaluation
Compared predicted anomalies with actual fraud labels using:
Confusion Matrix
Precision Score
Recall Score
Metrics Explanation
Precision
Measures how many detected fraud transactions were actually fraud.
Recall
Measures how many actual fraud transactions were successfully detected.
## 6. Data Visualization
Used PCA (Principal Component Analysis) to reduce dimensions and visualize:
K-Means clusters
Normal vs fraudulent transactions
## Results
The project successfully identified anomalous transactions using clustering techniques.
Key findings:
Fraud detection is challenging due to extreme class imbalance
K-Means can identify unusual patterns effectively
Distance-based anomaly detection helps isolate suspicious transactions
## Conclusion
This project demonstrates how unsupervised learning can be applied to real-world fraud detection problems.
Even without using transaction labels during training, clustering techniques can identify suspicious behavior by detecting outliers in the dataset.
Future Improvements
Possible improvements include:
DBSCAN clustering
Isolation Forest
Autoencoders
Deep Learning-based anomaly detection
Hyperparameter tuning
Skills Demonstrated
Data Cleaning
Data Preprocessing
Feature Scaling
Clustering Algorithms
Anomaly Detection
Model Evaluation
Data Visualization
Machine Learning Workflow
