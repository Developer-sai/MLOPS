End-to-End MLOps Pipeline for Predicting Student Academic Risk
Summary
This project demonstrates a comprehensive Machine Learning Operations (MLOps) pipeline designed to predict the academic risk of students in higher education. The pipeline encompasses data preprocessing, model training, hyperparameter tuning, model evaluation, visualization, continuous integration, and deployment. By leveraging MLOps practices, the project ensures reproducibility, version control, and efficient deployment of machine learning models.
Key Components
Data Preprocessing:
Handling missing values.
Feature selection and encoding.
Scaling numerical features.
Model Selection and Training:
Evaluation of multiple models (Random Forest, Gradient Boosting).
Training and evaluation using a train-test split.
Hyperparameter Tuning:
Utilizing RandomizedSearchCV to optimize model hyperparameters.
Logging experiments with MLflow for tracking and reproducibility.
Model Evaluation:
Assessing model performance using accuracy, F1 score, precision, and recall.
Generating visualizations such as confusion matrices and feature importance plots.
Continuous Integration:
Implementing CI/CD workflows using GitHub Actions and MLflow.
Automating model training, evaluation, and reporting.
Model Deployment:
Deploying the best model using FastAPI for real-time predictions.
Containerizing the application with Docker for easy deployment.
Conclusion
This project provides a robust framework for developing, deploying, and monitoring machine learning models in a production environment. By following MLOps best practices, the pipeline ensures that the model is scalable, maintainable, and delivers consistent value. The use of tools like MLflow, FastAPI, and Docker enhances the reproducibility and portability of the solution.
