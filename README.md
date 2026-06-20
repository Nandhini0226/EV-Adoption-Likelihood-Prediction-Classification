# Electric Vehicle (EV) Adoption Likelihood Prediction

## Project Overview

This project aims to predict a customer's likelihood of adopting an Electric Vehicle (EV) using Machine Learning techniques. The model analyzes demographic characteristics, travel behavior, charging infrastructure accessibility, environmental awareness, and technology adoption patterns to classify customers into one of three categories:

* High EV Adoption Likelihood
* Medium EV Adoption Likelihood
* Low EV Adoption Likelihood

The project helps EV manufacturers, policymakers, and charging infrastructure providers identify potential EV adopters and make data-driven decisions.

---

## Business Problem

As the automotive industry moves toward sustainable transportation, understanding consumer readiness for EV adoption is crucial. Organizations can leverage predictive analytics to:

* Target potential EV customers more effectively.
* Improve charging infrastructure planning.
* Design effective incentive and awareness programs.
* Support sustainable transportation initiatives.

---

## Dataset Features

### Numerical Features

* annual_income
* charging_station_accessibility
* technology_affinity_score
* environmental_awareness_score
* range_anxiety_score
* ev_knowledge_score
* battery_replacement_concern
* government_incentive_awareness
* nearest_charging_station_km

### Categorical Features

* previous_ev_experience
* city_type
* home_charging_available

### Target Variable

* ev_adoption_likelihood

---

## Data Preprocessing

The following preprocessing steps were performed:

* Missing value treatment using mode and median imputation.
* Data type validation.
* Outlier treatment using IQR-based Winsorization.
* Standardization of numerical features using StandardScaler.
* One-Hot Encoding of categorical variables.
* Stratified Train-Test Split (80:20).
* Pipeline implementation to prevent data leakage.

---

## Exploratory Data Analysis

Key findings include:

* Higher income individuals show greater EV adoption likelihood.
* Better charging station accessibility increases EV adoption.
* Environmental awareness positively influences EV adoption.
* Higher EV knowledge scores are associated with greater adoption likelihood.
* Lower range anxiety encourages EV adoption.
* Home charging availability significantly improves adoption likelihood.
* Urban residents demonstrate higher adoption rates than rural and suburban residents.

---

## Machine Learning Models

The following classification models were implemented and evaluated:

1. Logistic Regression
2. Random Forest Classifier
3. XGBoost Classifier

Evaluation metrics:

* Accuracy
* Precision
* Recall
* F1 Score

---

## Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score |
| ------------------- | -------: | --------: | -----: | -------: |
| Logistic Regression |   87.95% |    87.84% | 87.95% |   87.89% |
| XGBoost             |   86.76% |    86.71% | 86.76% |   86.73% |
| Random Forest       |   86.19% |    86.10% | 86.19% |   86.13% |

---

## Best Model

**Logistic Regression** achieved the highest performance across all evaluation metrics.

### Why Logistic Regression?

* Highest Accuracy and F1 Score.
* Computationally efficient.
* Easy to interpret and deploy.
* Captures the underlying relationships effectively.

---

## Business Recommendations

* Expand charging infrastructure in suburban and rural regions.
* Increase awareness of government EV incentives.
* Promote EV test-drive and experience programs.
* Encourage installation of home charging facilities.
* Focus marketing efforts on environmentally conscious and technology-oriented consumers.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost

---

## Project Workflow

Data Collection → Data Cleaning → Exploratory Data Analysis → Feature Selection → Data Preprocessing → Model Training → Model Evaluation → Model Comparison → Business Insights

---

## Conclusion

The study demonstrates that demographic, behavioral, technological, and infrastructure-related factors significantly influence EV adoption decisions. Logistic Regression emerged as the most effective model, achieving an F1 Score of 87.89%. The model can support EV manufacturers, policymakers, and energy providers in identifying potential EV adopters and accelerating the transition toward sustainable transportation.
