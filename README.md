ML | Breast Cancer Wisconsin Diagnosis using Logistic Regression
Overview

This project implements a custom Logistic Regression model from scratch to classify breast tumors as malignant or benign using the Breast Cancer Wisconsin (Diagnostic) dataset. 
The project demonstrates end-to-end steps of machine learning including data preprocessing, model training, and evaluation.

Dataset

The dataset contains 569 instances with 32 features. Key features include:

Clump Thickness

Uniformity of Cell Size

Uniformity of Cell Shape

Marginal Adhesion

Single Epithelial Cell Size

Bare Nuclei

Bland Chromatin

Normal Nucleoli

Mitoses

The target variable diagnosis is mapped as:

M → 1 (Malignant)

B → 0 (Benign)

Approach

Data Preprocessing

Remove unnecessary columns (id, Unnamed: 32).

Map categorical target variable to numeric.

Normalize features to the range [0, 1].

Split dataset into training (85%) and testing (15%) sets.

Model Implementation

Initialize weights and bias.

Implement sigmoid function.

Implement forward and backward propagation to compute cost and gradients.

Update weights using gradient descent for a given number of iterations.

Prediction & Evaluation

Predict outcomes on both training and test sets.

Compute accuracy for training and test sets.

Results

Example output from training:

Train accuracy: ~96-97%
Test accuracy: ~95-98%


Note: Accuracy may vary slightly due to random initialization of weights.

Requirements

Python 3.x

numpy

pandas

matplotlib

scikit-learn (for train_test_split)

Install dependencies with:

pip install numpy pandas matplotlib scikit-learn

Usage

Clone the repository:

git clone https://github.com/Mohammed-Saif-07/Breast-Cancer-Diagnosis.git
cd Breast-Cancer-Diagnosis


Place the data.csv file in the repository folder.

Run the script:

python breast_cancer_logreg.py

License

MIT License
