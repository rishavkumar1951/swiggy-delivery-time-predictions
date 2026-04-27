# 🍽️ Food Delivery Time Prediction

This project uses **Machine Learning** to predict **food delivery times** based on features like **location**, **distance**, and **traffic conditions**.  
The goal is to enhance delivery **accuracy**, **efficiency**, and **customer satisfaction** through data-driven predictions.

---

## 🚀 Overview

Food delivery services face major challenges in estimating accurate delivery times due to varying real-world conditions such as traffic, distance, and demand.  
This project builds and deploys an ML pipeline to predict delivery times from Swiggy-style datasets using reproducible workflows powered by **DVC**, **Docker**, and **CI/CD pipelines**.

---

## 🧠 Key Features

- 🟙️ **Feature Engineering**: Incorporates spatial and temporal data like distance, location clusters, and real-time traffic indicators.  
- ⚙️ **ML Modeling**: Trained and evaluated multiple regression models (Linear Regression, XGBoost, Random Forest, etc.) to identify the best performer.  
- 📊 **Experiment Tracking**: Managed experiments and datasets using **DVC (Data Version Control)**.  
- 🤪 **Testing & CI/CD**: Automated tests and deployment pipelines with **GitHub Actions**.  
- 🐳 **Containerized Deployment**: End-to-end Dockerized environment with ready-to-run scripts.  
- 🌐 **API Interface**: Flask-based `app.py` to serve predictions for real-time inference.

---

## 🧮 Tech Stack

| Category | Tools / Frameworks |
|-----------|--------------------|
| **Programming** | Python (NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn) |
| **ML Workflow** | DVC, MLflow (optional) |
| **Deployment** | Flask, Docker, AWS CodeDeploy |
| **Version Control** | Git, GitHub Actions |
| **Visualization** | Jupyter, Matplotlib, Plotly |

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/vishvaspatel/food-delivery-time-prediction.git
cd food-delivery-time-prediction
```

### 2️⃣ Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate   # on Mac/Linux
venv\Scripts\activate      # on Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Set Up DVC
```bash
dvc init
dvc repro
```

### 5️⃣ Run Application
```bash
python app.py
```

Then open your browser and go to:
```
http://127.0.0.1:5000
```

---

## 📊 Model Development Workflow

1. **Data Preprocessing** – Cleaning, encoding categorical features, handling outliers.  
2. **EDA** – Visual analysis of features like distance vs delivery time.  
3. **Feature Engineering** – Deriving new predictors (e.g., time of day, distance bins).  
4. **Model Training** – Comparing multiple regression models.  
5. **Evaluation** – Metrics such as MAE, RMSE, R².  
6. **Versioning** – Model and dataset tracking with DVC.  
7. **Deployment** – Containerized Flask API for real-time predictions.

---

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
