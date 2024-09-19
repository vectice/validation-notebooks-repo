# Model Validation Notebooks

This repository contains a set of predefined validation notebooks to help you validate models based on best practices, with metadata and configuration files to streamline the process. You can get prepopulated configuration files (JSON) for the model you would like to validate from the Vectice UI.

## How to Use This Repository

1. **Identify which validation suite to run**  
   This repository is structured to guide you towards the appropriate validation suite based on your specific use case. The folders are organized by validation categories, and each category contains specialized test suites to assess different aspects of your model.

2. **Select the Appropriate Test Suite**  
   Navigate through the folder structure to select the most relevant test suite for your needs. Each test suite is designed for specific validation tasks such as **Classification**, **Explainability**, **Resilience**, **Robustness**, **Model Performance**, or **PD Models**.

3. **Download and Customize as Needed**  
   Once you’ve identified the correct test suite, download the corresponding notebook. If the default notebook doesn’t fully meet your needs, you can modify the provided tests or create your own. The repository also includes example notebooks to help you customize your validation tests.

---

## Folder Structure Overview

The repository is structured around key validation categories, with each category containing specialized test suites to cover different validation needs. Below is a guide to help you choose the right suite based on your use case:

| **Use Case**                                       | **Validation Category** | **Folder**                         | **Test Suites Available**                                                                                   |
|----------------------------------------------------|-------------------------|------------------------------------|--------------------------------------------------------------------------------------------------------------|
| **Validating model predictions for classification** | Classification          | `classification`                   | - `classification_notebook.ipynb`: Covers accuracy, precision, recall, F1-score, AUC.                        |
| **Ensuring model predictions are interpretable**   | Explainability          | `explainability`                   | - `shap_explainability_notebook.ipynb`: Uses SHAP for model interpretation.<br>- `lime_explainability.ipynb`: Uses LIME for model interpretation. |
| **Testing model robustness to input variations**   | Robustness              | `robustness`                       | - `robustness_notebook.ipynb`: Evaluates model sensitivity to small input changes.                           |
| **Assessing model performance under varied conditions** | Resilience             | `resilience`                       | - `resilience_notebook.ipynb`: Measures how well the model maintains performance under stress tests.         |
| **Evaluating overall model performance**           | Model Performance       | `performance`                      | - `performance_notebook.ipynb`: Provides an overview of standard performance metrics.                        |
| **Validating Probability of Default (PD) models**  | PD Models               | `pd_models`                        | - `pd_validation_notebook.ipynb`: Tests focused on validating probability of default predictions. |

### Folder Descriptions

1. **Classification**  
   Contains test suites focused on evaluating classification model metrics like accuracy, precision, recall, F1-score, and AUC.

2. **Explainability**  
   Focuses on tests that ensure the model's predictions can be interpreted. Includes notebooks using SHAP and LIME for model explainability.

3. **Robustness**  
   Includes test suites designed to evaluate how sensitive the model is to small changes in the input data.

4. **Resilience**  
   Contains test suites that assess how well the model maintains its performance under varied conditions, such as different data distributions or adversarial scenarios.

5. **Model Performance**  
   Provides a comprehensive evaluation of the model’s performance across multiple metrics, offering a holistic view of its effectiveness.

6. **PD Models**  
   This folder is dedicated to validating Probability of Default (PD) models. It includes tests to assess the calibration, discriminatory power, and overall reliability of PD predictions.
