
# Model Validation Notebooks

This repository contains a set of predefined validation notebooks to help you validate models based on best practices, with metadata and configuration files to streamline the process.

## How to Use This Repository

1. **Identify Your Model Type**  
   Choose between the available subfolders based on your specific validation needs. This repository currently includes:
   - Custom Extensions
   - Classification Models (wrapping the MoDeVa extension)

2. **Download the Recommended Notebook**  
   In each subfolder, you'll find notebooks pre-configured to handle specific validation tasks. Download the notebook that best fits your requirements.

3. **Customize as Needed**  
   If the default notebook doesn't fully meet your needs, you can modify the provided tests or create your own. Refer to the `custom-extensions` folder for examples on how to add and customize your validation tests.

---

## Folder Overview

### 1. **Classification Models**  
This folder wraps the MoDeVa commercial extension of PiML and provides validation notebooks for classification models. These notebooks include comprehensive tests to evaluate:
   - **Explainability:** Ensures that the model's predictions can be interpreted.
   - **Resilience:** Tests the model's ability to maintain performance under varying conditions.
   - **Robustness:** Measures how sensitive the model is to small changes in the input.
   - **Model Performance:** Evaluates traditional classification metrics like accuracy, precision, recall, F1-score, and AUC.

### 2. **Custom Extensions**  
The `custom-extensions` folder contains an example notebook that demonstrates how to add custom validation tests to your workflow. If you wish to modify the default notebooks or create new ones, follow this guide to integrate your own tests.

---

## How to Customize Your Notebooks

1. **Start with a Default Notebook**  
   Download a default notebook from Vectice APP or get one from one of the subfolders.

2. **Refer to the Custom Extensions Folder**  
   The notebook in `custom-extensions` provides examples of how to create and integrate new validation tests.

3. **Add Your Own Tests**  
   Follow the structure in the example to insert new tests into the existing notebook.

4. **Run Your Custom Tests**  
   Once modified, run your notebook with the configuration file (JSON) to validate your model with the new tests.

---

Feel free to explore the folders and use or modify the notebooks as needed. If you have any questions or need further assistance, reach out to the support team.
