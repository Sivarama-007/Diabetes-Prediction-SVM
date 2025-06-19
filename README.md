# Diabetes Prediction using Support Vector Machine (SVM)

## Project Description
This project builds a machine learning system to predict whether a person has diabetes or not using the Pima Indians Diabetes dataset. We use a Support Vector Machine (SVM) classifier with a linear kernel.

---

## Dataset
The dataset contains 768 samples and 8 feature columns related to patient medical attributes, along with a binary outcome column (0: Non-Diabetic, 1: Diabetic).

The dataset is included in the `/data` folder as `diabetes.csv`.

---

## Project Workflow
1. Data Loading and Exploration  
2. Data Standardization (using `StandardScaler`)  
3. Splitting the data into training and test sets (80/20 stratified split)  
4. Training an SVM classifier  
5. Evaluating model performance using accuracy score  
6. Building a prediction function for new inputs

---

## Results

- Training Accuracy: 78.66%  
- Test Accuracy: 77.27%

The model shows good generalization performance with default parameters.

---

## Example Usage

Input example:
```python
input_data = (5,166,72,19,175,25.8,0.587,51)
print(predict_diabetes(input_data))
# Output: The person is Diabetic
