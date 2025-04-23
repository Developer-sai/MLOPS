End-to-End MLOps Pipeline for Predicting Student Academic Risk
Overview
This project demonstrates a complete Machine Learning Operations (MLOps) pipeline for predicting the academic risk of students in higher education. The pipeline includes data preprocessing, model training, hyperparameter tuning, model evaluation, visualization, continuous integration, and deployment.
Table of Contents
Introduction
Setup and Installation
Data Preprocessing
Model Selection and Training
Hyperparameter Tuning
Model Evaluation
Visualization and Results Analysis
Continuous Integration with MLflow
Model Deployment with FastAPI
Dockerization
Conclusion
Introduction
MLOps combines DevOps principles with machine learning to streamline the deployment and maintenance of ML models. This project aims to predict the academic risk of students, specifically whether they will drop out, remain enrolled, or graduate.
Setup and Installation
To run this project, you need to have Python and Docker installed. Follow these steps to set up the environment:
Install Required Libraries:
bash
Copy
pip install scikit-learn pandas numpy matplotlib seaborn mlflow joblib fastapi uvicorn pydantic docker
Clone the Repository:
bash
Copy
git clone https://github.com/yourusername/academic-risk-predictor.git
cd academic-risk-predictor
Install Project Dependencies:
bash
Copy
pip install -r requirements.txt
Data Preprocessing
The dataset is preprocessed to handle missing values, encode categorical features, and scale numerical features. The preprocessing steps are encapsulated in a ColumnTransformer to ensure consistency across training and test sets.
Model Selection and Training
Multiple models are trained and evaluated to determine the best-performing model. The models include:
Random Forest Classifier
Gradient Boosting Classifier
Hyperparameter Tuning
Hyperparameter tuning is performed using RandomizedSearchCV to find the optimal hyperparameters for the best-performing models.
Model Evaluation
The best model is evaluated on a test set to assess its performance. Key metrics include accuracy, F1 score, precision, and recall.
Visualization and Results Analysis
Visualizations such as the confusion matrix and feature importance plots are generated to provide insights into the model's performance.
Continuous Integration with MLflow
MLflow is used for experiment tracking, logging model parameters, and metrics. This ensures reproducibility and ease of comparison between different runs.
Model Deployment with FastAPI
The best model is deployed using FastAPI to create a RESTful API for real-time predictions. The API is containerized using Docker for easy deployment.
Dockerization
A Dockerfile is provided to containerize the FastAPI application. The Docker image can be built and run to serve the model predictions.
Conclusion
This project demonstrates a complete MLOps pipeline, from data preprocessing to model deployment and monitoring. Each step is carefully designed to ensure reproducibility, version control, and efficient deployment of the machine learning model.
How to Run
Build the Docker Image:
bash
Copy
docker build -t academic-risk-predictor .
Run the Docker Container:
bash
Copy
docker run -p 8000:8000 academic-risk-predictor
Access the API:
Open your browser and navigate to http://localhost:8000 to access the deployed model.
