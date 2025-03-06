# End-to-End Chest Cancer Classification with DVC & MLflow

Welcome to the **End-to-End Chest Cancer Classification** project! This repository showcases a robust machine learning pipeline for classifying chest cancer using state-of-the-art tools like **DVC (Data Version Control)** and **MLflow** for experiment tracking and reproducibility. This project is designed to demonstrate best practices in MLOps, including data versioning, model training, evaluation, and deployment.

---

## 🚀 Project Overview

This project aims to build a machine learning model to classify chest cancer using medical imaging data. The pipeline includes:

- **Data Versioning with DVC**: Track and version datasets, models, and artifacts.
- **Experiment Tracking with MLflow**: Log experiments, metrics, and models for reproducibility.
- **End-to-End Pipeline**: From data ingestion to model deployment.
- **CI/CD Integration**: Automated testing and deployment using GitHub Actions.

---

## 📁 Project Structure

---
- **`.dvc/`**: Contains DVC configuration files for data versioning.
- **`.github/workflows/`**: GitHub Actions workflows for CI/CD automation.
- **`config/`**: Configuration files for the project.
- **`mlruns/`**: MLflow experiment tracking data.
- **`model/`**: Stores trained models.
- **`research/`**: Contains research notebooks and exploratory data analysis (EDA).
- **`src/cnnClassifier/`**: Source code for the CNN classifier.
- **`templates/`**: HTML templates for the Flask web application.
- **`Dockerfile`**: Configuration for Docker containerization.
- **`app.py`**: Flask application for deploying the model.
- **`dvc.lock` & `dvc.yaml`**: DVC pipeline configuration files.
- **`params.yaml`**: Parameters for the pipeline.
- **`requirements.txt`**: Python dependencies for the project.
- **`scores.json`**: Model evaluation scores.
- **`setup.py`**: Setup script for the project.
- **`temp_model.keras`**: Temporary model file.
- **`template.py`**: Script for generating project templates.

---

## 🛠️ Tools and Technologies

- **DVC**: Data versioning and pipeline management.
- **MLflow**: Experiment tracking and model management.
- **TensorFlow/Keras**: Deep learning model development.
- **Flask**: Web application for model deployment.
- **GitHub Actions**: CI/CD automation.
- **Docker**: Containerization for deployment.

---

## 🚀 Getting Started

### Step 1: Clone the Repository
```bash
git clone https://github.com/Mpasha17/End-To-End-Chest-Cancer-Classification.git
cd End-To-End-Chest-Cancer-Classification

### Step 2: Set Up the Environment

1. **Create a virtual environment:**

    ```bash
    conda create -n chest_cancer python=3.10 -y
    conda activate chest_cancer
    ```

2. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

### Step 3: Data Versioning with DVC

1. **Pull the data using DVC:**

    ```bash
    dvc pull
    ```

2. **Reproduce the pipeline:**

    ```bash
    dvc repro
    ```

### Step 4: Experiment Tracking with MLflow

1. **Start the MLflow server:**

    ```bash
    mlflow ui
    ```

2. **View the experiments at [http://localhost:5000](http://localhost:5000).**

## 📊 Data Pipeline

1. **Data Ingestion:**
   - Fetch and preprocess the dataset using DVC for versioning.

2. **Data Validation:**
   - Validate the dataset against a predefined schema.

3. **Model Training:**
   - Train a CNN model using TensorFlow/Keras.
   - Log experiments and metrics using MLflow.

4. **Model Evaluation:**
   - Evaluate the model on a test set and log metrics.

5. **Model Deployment:**
   - Deploy the model using Flask and Docker.

## 🔄 CI/CD Pipeline

### GitHub Actions

- Automated testing and deployment using GitHub Actions.
- Docker image build and push to Docker Hub.

### Docker Deployment

1. **Build the Docker image:**

    ```bash
    docker build -t chest-cancer-classification .
    ```

2. **Run the Docker container:**

    ```bash
    docker run -p 5080:5080 chest-cancer-classification
    ```

3. **Access the web app at [http://localhost:5080](http://localhost:5080).**

## 📈 Results

- **Model Performance:** Achieved an accuracy of X% on the test set.
- **Experiment Tracking:** All experiments are logged in MLflow for reproducibility.
- **Data Versioning:** Datasets and models are versioned using DVC.

## 💬 Connect

If you have any questions or feedback, feel free to reach out:

- **Email:** [mp5272672@gmail.com](mailto:mp5272672@gmail.com)
- **GitHub:** [Mpasha17](https://github.com/Mpasha17)

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
