# WorkPulse: Employee Burnout Prediction System

## Overview
WorkPulse is a machine learning–based system designed to predict employee burnout risk using workload-related data. The project provides early burnout detection through predictive analytics and visualizes insights using Grafana dashboards while maintaining ethical and privacy-preserving standards.

## Problem Statement
Employee burnout is often identified only after it impacts productivity and mental well-being. There is a lack of automated, data-driven systems that can predict burnout risk early using objective workload indicators.

## Objectives
- Predict employee burnout risk using machine learning
- Analyze workload patterns through structured data
- Visualize burnout trends using dashboards
- Ensure ethical and privacy-preserving analytics
- Support workforce well-being decision-making

## System Architecture
Workload Data → Feature Engineering → ML Model → Predictions → Supabase (PostgreSQL) → Grafana Dashboard

## Dataset
The dataset is synthetically generated and does not contain real employee data.

### Features
- employee_id  
- work_hours  
- tasks_completed  
- tasks_pending  
- overtime_hours  
- breaks_count  
- after_hours_work  

### Engineered Features
- task_completion_rate  
- workload_score  

### Target Label
- burnout_label (Low / Medium / High)

## Burnout Prediction Methodology

### Labeling Strategy
- High: Long work hours, high overtime, low breaks
- Medium: Moderate workload imbalance
- Low: Balanced workload with sufficient breaks

### Machine Learning Model
- Random Forest Classifier
- Train-test split: 80/20
- Feature importance analysis

## Tech Stack

### Machine Learning
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

### Backend & Database
- Supabase
- PostgreSQL

### Visualization
- Grafana

## Workflow
1. Generate synthetic workload data  
2. Perform feature engineering  
3. Train and evaluate ML model  
4. Save trained model and encoder  
5. Predict burnout risk for new data  
6. Store predictions in Supabase  
7. Visualize insights in Grafana  

## Model Evaluation
- Accuracy score
- Classification report
- Confusion matrix
- Feature importance visualization


## Output

#### Output1 - Grafana dashboard illustrating employee burnout prediction results and workload trends

![1](https://github.com/user-attachments/assets/91b9c53b-9fde-4839-9eab-4b90b40bb67c)


#### Output2 -  Burnout risk distribution and high-risk workload trends visualization

![WhatsApp Image 2026-02-01 at 1 23 49 PM](https://github.com/user-attachments/assets/bdb88ddc-64df-4a5e-8596-737126fa4173)


## Results and Impact
The WorkPulse: Employee Burnout Prediction System successfully demonstrates the effectiveness of machine learning in identifying early signs of employee burnout using workload-related data. The trained models accurately classify employees into Low, Medium, and High burnout risk categories, enabling timely recognition of workload imbalance and stress patterns.

The interactive Grafana dashboards provide clear and actionable visual insights into employee workload trends, overtime frequency, and burnout risk distribution over time. This visualization helps decision-makers quickly identify high-risk scenarios and understand contributing factors, improving situational awareness and planning.

## Articles published / References
1. O. Batata, V. Augusto, and X. Xie, “Mixed Machine Learning and Agent-Based Simulation for Respite Care Evaluation,” in Proc. 2018 Winter Simulation Conf. (WSC), Gothenburg, Sweden, Dec. 2018, pp. 2668–2679.
     doi:10.1109/WSC.2018.8632385.
2. Kiranashree, B. K., Ambika, V., & Radhika, A. D. (2021). Analysis of machine learning techniques for stress detection among employees. Asian J. Comp. Sci. & Technol.




