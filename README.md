# Adult Income Classification ML Project

## Project Goal
The primary goal of this project is to automate the financial decision-making process. By utilizing machine learning, we predict whether an individual's annual income exceeds $50,000 based on census data, including demographics, education, and employment history.

---

## Machine Learning Task & Implementation
* **Task:** Binary Classification.
* **Library:** AutoGluon (Applied Machine Learning).
* **Why ML?** Implementing Machine Learning reduces human error, provides faster results, and can handle complex patterns in data that manual solutions cannot easily identify. It ensures scalability and consistent decision-making across large datasets.

---

## Data & Feature Engineering
* **Dataset:** Adult Income Dataset (32,561 records).
* **Feature Importance:** Through permutation shuffling, `Capital-gain` was identified as the most influential feature, followed by `Marital-status` and `Age`.
* **Preprocessing:** AutoGluon handled automated feature engineering, including categorical encoding and missing value imputation.

---

## Model Evaluation & Metrics
* **Best Model:** WeightedEnsemble_L2.
* **Accuracy:** The model achieved a final accuracy of approximately **87.5%** on the test set.
* **Performance Assessment:** Based on the Confusion Matrix, the model shows high precision in identifying the majority class (<=50K), confirming its reliability for filtering purposes.

---

## Deployment & Deliverables
This project includes a local deployment via an interactive dashboard:
* **Interactive Inference:** A user-friendly interface built with `ipywidgets` allows for real-time predictions.
* **Model Persistence:** The trained predictor is saved and can be reloaded using `TabularPredictor.load()` for future inference without retraining.

---

## Setup and Usage
1.  **Clone the Repository:** Download the project folder containing the notebook and model artifacts.
2.  **Install Dependencies:**
    ```bash
    pip install autogluon ipywidgets pandas matplotlib
    ```
3.  **Run the Notebook:** Open the `.ipynb` file in Google Colab or a local Jupyter environment.
4.  **Execute Inference:** Run the final cells to launch the **Interactive Prediction App** and test the model with custom inputs.