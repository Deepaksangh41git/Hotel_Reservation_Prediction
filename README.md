#  Hotel Booking Prediction - MLOps Project

This project is an end-to-end **Machine Learning + MLOps pipeline** for predicting hotel booking status (confirmed/cancelled). It covers the full lifecycle from data ingestion to deployment using best practices.

---

##  Project Overview

The system performs:

* Data ingestion from Google Cloud Storage
* Data preprocessing (cleaning, encoding, balancing, feature selection)
* Model training with hyperparameter tuning
* Experiment tracking using MLflow
* Model serving using Flask
* Containerization using Docker
* CI/CD using Jenkins

---

##  Tech Stack

* **Python**
* **Scikit-learn, LightGBM**
* **MLflow**
* **Flask**
* **Docker**
* **Jenkins**
* **Google Cloud Platform (GCP)**
* **Google Cloud Storage**
* **SMOTE (Imbalanced-learn)**

##  Features Used for Prediction

Example features:

* Lead time
* Number of special requests
* Average price per room
* Arrival date/month
* Market segment type
* Number of nights (week/weekend)
* Meal plan
* Room type

---

##  Experiment Tracking

* MLflow is used to:

  * Log datasets
  * Log parameters
  * Log metrics
  * Track experiments

---

##  Deployment

The application is deployed on **Google Cloud Platform (GCP)** using Docker containers and automated via Jenkins CI/CD pipeline.

---

##  CI/CD Pipeline (Jenkins + GCP)

This project uses Jenkins for automating the end-to-end pipeline:

- Pulls latest code from GitHub
- Builds Docker image
- Pushes image to container registry (GCP)
- Deploys the application to Google Cloud

Pipeline stages include:
- Build
- Test
- Docker Image Creation
- Deployment to GCP

The application is containerized and deployed on Google Cloud infrastructure.

---

##  Error Handling & Logging

* Custom exception handling implemented 
* Logging system saves logs with timestamps