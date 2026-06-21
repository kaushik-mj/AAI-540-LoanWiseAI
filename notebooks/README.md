# Loan Approval Prediction System

End-to-End Machine Learning System for Data-Driven Lending Decisions using AWS SageMaker and MLOps


## Project Overview

Financial institutions must continuously balance portfolio growth with credit risk management. Traditional lending processes often rely on manual reviews and static business rules that can be difficult to scale as application volumes increase.

This project develops an end-to-end Loan Approval Prediction System that leverages machine learning to support data-driven lending decisions. The solution demonstrates a complete MLOps workflow on AWS SageMaker, including data engineering, feature management, model development, governance, inference, monitoring, and CI/CD validation.

The objective is not only to build an accurate predictive model but also to establish a scalable, reproducible, and operationally governed machine learning lifecycle.


## Business Problem

Approving high-risk applicants can increase default rates and financial losses, while rejecting creditworthy applicants can reduce revenue opportunities and negatively impact customer experience.

The challenge is no longer access to data—it is the ability to transform historical applicant information into accurate, consistent, and scalable lending decisions.

This project addresses that challenge through predictive analytics and modern MLOps practices.

### Architecture Components

* Amazon S3 Data Lake
* SageMaker Studio
* SageMaker Feature Store
* Model Training & Evaluation
* SageMaker Model Registry
* Model Inference & Validation
* Monitoring & Observability
* CI/CD Validation Pipeline

---

## Dataset

### Source

Home Credit Default Risk Dataset (Kaggle)

### Dataset Strategy

To satisfy project requirements while maintaining low infrastructure costs, a balanced dataset was created:

| Metric         | Value  |
| -------------- | ------ |
| Total Records  | 20,000 |
| Positive Class | 10,000 |
| Negative Class | 10,000 |

The dataset was cleaned, transformed, validated, and prepared for machine learning workflows.

## Machine Learning Workflow

### Notebook 1 – Data Preparation & Feature Store

* Data ingestion and preprocessing
* Missing value treatment
* Feature engineering
* SageMaker Feature Store creation

### Notebook 2 – Model Training & Evaluation

* Logistic Regression
* Random Forest
* XGBoost
* Performance comparison and model selection

### Notebook 3 – Model Registry

* Model registration
* Version management
* Approval workflow

### Notebook 4 – Model Inference & Validation

* Prediction generation
* Operational validation
* Inference artifact creation

### Notebook 5 – Monitoring

* Data Quality Monitoring
* Data Drift Monitoring
* Model Performance Monitoring
* CloudWatch Dashboard

### Notebook 6 – CI/CD Pipeline

* Data Validation
* Feature Validation
* Model Validation
* Evaluation Validation
* Deployment Approval

## Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
| ------------------- | -------: | --------: | -----: | -------: | ------: |
| Logistic Regression |  0.66450 |  0.673158 | 0.6395 | 0.655897 | 0.66450 |
| Random Forest       |  0.67175 |  0.678627 | 0.6525 | 0.665307 | 0.67175 |
| XGBoost             |  0.67125 |  0.672024 | 0.6690 | 0.670509 | 0.67125 |

### Selected Model

**XGBoost** was selected as the final model based on its superior balance between risk detection and overall predictive performance.

Key Results:

* Highest Recall: 0.6690
* Highest F1 Score: 0.670509
* Best balance between Precision and Recall


## AWS Services Used

| Service                  | Purpose                      |
| ------------------------ | ---------------------------- |
| Amazon S3                | Data Lake & Artifact Storage |
| SageMaker Studio         | Development Environment      |
| SageMaker Feature Store  | Feature Management           |
| SageMaker Model Registry | Model Governance             |
| Amazon CloudWatch        | Monitoring & Observability   |
| SageMaker Pipelines      | CI/CD Validation             |


## Repository Structure


loan-approval-prediction-system/
│
├── notebooks/
│   ├── Notebook_1_Data_Preparation_Feature_Store.ipynb
│   ├── Notebook_2_Model_Training_Evaluation.ipynb
│   ├── Notebook_3_Model_Registry.ipynb
│   ├── Notebook_4_Model_Inference_Validation.ipynb
│   ├── Notebook_5_Monitoring.ipynb
│   └── Notebook_6_CICD_Pipeline.ipynb
│
├── artifacts/
├── screenshots/
├── docs/
├── README.md
├── requirements.txt
└── .gitignore


## Key Outcomes

* Built a complete end-to-end machine learning lifecycle on AWS SageMaker.
* Implemented Feature Store, Model Registry, Monitoring, and CI/CD validation.
* Established governance, traceability, and deployment readiness controls.
* Demonstrated production-inspired MLOps practices using a cost-effective architecture.
* Delivered a scalable and reproducible framework for loan approval prediction.


## Future Enhancements

* Automated model retraining
* Explainable AI using SHAP
* Real-time inference endpoints
* Advanced monitoring and alerting
* Expanded feature engineering pipeline

## License

This repository is intended for educational and academic purposes.
