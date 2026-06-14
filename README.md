# Bank-Churn-Prediction-System

## Nonlinear Customer Behavior Analytics Using Chaos Learning

A machine learning and nonlinear behavioral intelligence platform designed to predict customer attrition by modeling banking behavior as a dynamic system. The platform combines supervised learning with Chaos Learning techniques such as phase-space reconstruction, Lyapunov exponent analysis, entropy measurement, attractor discovery, and nonlinear state-space modeling to identify hidden churn indicators before customer disengagement becomes observable.

---

## Problem Statement

Customer churn remains one of the most significant revenue challenges for financial institutions. Traditional churn prediction systems primarily rely on demographic variables, transactional aggregates, and static behavioral indicators, often failing to capture evolving behavioral instability that emerges before churn occurs.

Common challenges include:

* Rising customer acquisition costs
* Declining customer lifetime value
* Delayed churn detection
* Limited visibility into behavioral transitions
* Inefficient retention targeting

A more adaptive and behavior-centric approach is required to identify hidden churn signals and support proactive customer retention strategies.

---

## Solution Overview

The Bank Churn Prediction System combines Chaos Learning and Machine Learning to transform customer activity into dynamic behavioral trajectories and extract nonlinear indicators associated with churn risk.

The platform integrates:

* Behavioral Time-Series Modeling
* Phase-Space Reconstruction
* Lyapunov Exponent Analysis
* Entropy-Based Behavioral Analysis
* Attractor Discovery
* Supervised Machine Learning
* Risk Scoring and Prediction Services

By combining nonlinear dynamics with predictive analytics, the system enables earlier churn identification and more informed customer retention planning.

---

## Key Features

### Customer Intelligence

* Customer churn probability prediction
* Churn risk scoring
* Customer lifecycle analysis
* Behavioral stability monitoring
* Retention opportunity identification
* Portfolio-level churn analytics

### Chaos Learning Engine

* Phase-space reconstruction
* Lyapunov exponent computation
* Entropy analysis
* Attractor state identification
* Nonlinear temporal pattern extraction
* Dynamic customer state modeling

### Machine Learning Engine

* Automated feature engineering
* Feature selection pipeline
* Ensemble learning framework
* Hyperparameter optimization
* Probability-based prediction
* Feature importance analysis

### Decision Support

* Customer segmentation analytics
* Retention targeting insights
* Risk monitoring dashboard
* Automated churn alerts
* Performance monitoring

---

## System Architecture

### High-Level Workflow

```text
Customer Data Sources
        │
        ▼
Data Acquisition Pipeline
        │
        ▼
Data Cleaning & Preprocessing
        │
        ▼
Behavioral Time-Series Generation
        │
        ▼
Chaos Learning Engine
 ├─ Phase-Space Reconstruction
 ├─ Entropy Analysis
 ├─ Attractor Detection
 ├─ Lyapunov Exponent Analysis
 └─ Nonlinear Feature Extraction
        │
        ▼
Feature Engineering Pipeline
        │
        ▼
Machine Learning Models
        │
        ▼
Churn Probability Generation
        │
        ▼
Risk Analytics Dashboard
```

### Architecture Diagram

![Architecture](architecture/architecture.png)

---

## Dataset

### Source

Bank Customer Churn Dataset

### Dataset Characteristics

* Customer demographics
* Account information
* Transaction history
* Product usage metrics
* Customer engagement indicators

### Target Variable

* Churn Status (Exited / Retained)

### Data Processing

* Missing value handling
* Outlier treatment
* Feature normalization
* Behavioral sequence construction
* Chaos feature extraction

---

## Technology Stack

| Layer            | Technologies                                    |
| ---------------- | ----------------------------------------------- |
| Programming      | Python                                          |
| Machine Learning | Scikit-Learn, XGBoost                           |
| Data Processing  | Pandas, NumPy                                   |
| Chaos Learning   | SciPy, Nolds, Custom Nonlinear Dynamics Modules |
| Backend          | FastAPI                                         |
| Frontend         | Streamlit                                       |
| Database         | PostgreSQL, SQLite                              |
| Visualization    | Plotly, Matplotlib                              |
| Infrastructure   | Docker                                          |
| Version Control  | Git, GitHub                                     |

---

## Project Structure

```text
bank-churn-prediction-system/
│
├── README.md
├── LICENSE
├── requirements.txt
│
├── architecture/
│   └── architecture.png
│
├── screenshots/
│   └── dashboard.png
│
├── docs/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── feature_store/
│
├── notebooks/
│
├── src/
│   ├── ingestion/
│   ├── preprocessing/
│   ├── chaos_learning/
│   ├── feature_engineering/
│   ├── models/
│   ├── evaluation/
│   ├── prediction/
│   └── utils/
│
├── api/
├── dashboard/
├── tests/
└── docker/
```

---

## Implementation Highlights

### Chaos Learning Methodology

Unlike conventional churn systems that rely solely on statistical indicators, this platform models customer behavior as a nonlinear dynamical system.

#### Phase-Space Reconstruction

Transforms customer activity sequences into multidimensional behavioral trajectories to uncover hidden state transitions.

#### Lyapunov Exponent Analysis

Measures behavioral instability and divergence rates to identify customers approaching churn-prone states.

#### Entropy Analysis

Quantifies uncertainty and disorder in customer interactions, highlighting increasing behavioral unpredictability.

#### Attractor Discovery

Identifies stable and unstable behavioral regions that characterize long-term customer engagement patterns.

### Machine Learning Pipeline

#### Data Processing

* Missing value treatment
* Outlier detection
* Data normalization
* Behavioral sequence construction

#### Feature Engineering

* Demographic indicators
* Financial behavior metrics
* Product engagement metrics
* Transaction activity features
* Chaos-derived behavioral features

#### Model Training

Supported models:

* Logistic Regression
* Random Forest
* XGBoost
* Support Vector Machines
* Gradient Boosting
* Ensemble Architectures

### Scalability Considerations

* Modular analytics architecture
* Feature-store design
* Containerized deployment
* Batch prediction support
* Independent service components

### Reliability Measures

* Input validation
* Data quality checks
* Feature consistency validation
* Model evaluation framework

### Security Considerations

* Customer data anonymization
* Secure API validation
* Environment variable management
* Dependency isolation

---

## Model Performance

| Metric    | Value |
| --------- | ----- |
| Accuracy  | TBD   |
| Precision | TBD   |
| Recall    | TBD   |
| F1 Score  | TBD   |
| ROC-AUC   | TBD   |

Performance metrics will be updated after final model evaluation and validation.

---

## Screenshots

### Dashboard

![Dashboard](screenshots/dashboard.png)

---

## Installation & Setup

### Clone Repository

```bash
git clone https://github.com/Samarth-D-Suryavamshi/Bank-Churn-Prediction-System.git

cd Bank-Churn-Prediction-System
```

### Backend Setup

```bash
python -m venv venv

source venv/bin/activate
```

Windows:

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### Environment Variables

```env
DATABASE_URL=
MODEL_PATH=
ENVIRONMENT=development
```

### Run Application

```bash
uvicorn main:app --reload
```

---

## API Overview

| Endpoint       | Method | Description               |
| -------------- | ------ | ------------------------- |
| /predict       | POST   | Generate churn prediction |
| /risk-score    | GET    | Retrieve churn risk score |
| /model-metrics | GET    | Retrieve model metrics    |
| /health        | GET    | Service health status     |

---

## Results & Business Impact

The platform demonstrates how nonlinear behavioral indicators can complement traditional churn prediction models by identifying hidden instability patterns and improving churn-risk visibility.

Potential applications include:

* Customer retention planning
* Early churn-risk identification
* Behavioral analytics
* Customer segmentation
* Decision-support systems

---

## Future Enhancements

### Machine Learning

* Bayesian uncertainty estimation
* Explainable AI (XAI)
* Automated retraining workflows
* Active learning pipelines

### Chaos Learning

* Adaptive chaos-feature generation
* Advanced attractor analysis
* Temporal nonlinear behavior tracking

### Infrastructure

* CI/CD pipelines
* Kubernetes deployment
* Real-time inference services
* Event-driven processing

### Analytics

* Real-time churn monitoring
* Advanced customer segmentation
* Retention recommendation engine

---

## Learning Outcomes

This project demonstrates practical application of:

### Machine Learning

* Supervised learning
* Ensemble learning
* Feature engineering
* Predictive analytics

### Chaos Theory

* Nonlinear dynamics
* Entropy analysis
* Lyapunov exponents
* Phase-space reconstruction
* Attractor modeling

### Software Engineering

* API development
* Backend architecture
* Modular system design
* Containerized deployment

### Data Engineering

* Data preprocessing
* Pipeline development
* Feature-store design
* Dataset management

---

## Contributors

### Samarth D Suryavamshi

**Role:** Machine Learning Engineer & System Developer

**Responsibilities:**

* System Architecture
* Chaos Learning Framework Design
* Feature Engineering
* Model Development
* Backend Development
* API Development
* Deployment & Testing

**LinkedIn:**
https://www.linkedin.com/in/samarth-suryavamshi-a15642298/

**GitHub:**
https://github.com/Samarth-D-Suryavamshi

---

### Rashmi M D

**Role:** Research & Data Engineering Contributor

**Responsibilities:**

* Research Support
* Literature Review
* Dataset Analysis
* Data Collection
* Data Preprocessing
* Data Validation
* Documentation Support

**LinkedIn:**
https://www.linkedin.com/in/rashmi-m-d-815762344

**GitHub:**
[To Be Added]

---

## License

This project is released under the MIT License.

See the LICENSE file for additional details.
