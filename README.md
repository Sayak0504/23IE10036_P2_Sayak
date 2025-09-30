
# Logistic Regression for Heart Disease Prediction

This project implements a complete machine learning pipeline to predict the 10-year risk of coronary heart disease (CHD) using the Framingham Heart Study dataset. The pipeline includes data cleaning, advanced imputation using a custom K-Nearest Neighbors (KNN) algorithm, and a Logistic Regression model built from scratch with Stochastic Gradient Descent (SGD).

## Project Overview 📋

The goal is to build a binary classification model that predicts whether a patient is at risk of developing heart disease within the next 10 years (`TenYearCHD` target variable).

### Key Features:

  * **Data Cleaning**: Handles missing values by strategically dropping rows from columns with minimal (\<3%) missing data.
  * **Custom KNN Imputer**: Imputes remaining missing values using a from-scratch KNN algorithm with Nan-Euclidean distance for accuracy.
  * **Custom Logistic Regression**: The classification model is a Logistic Regression algorithm built from the ground up, trained using Stochastic Gradient Descent (SGD).
  * **Model Evaluation**: The model's performance is evaluated using Accuracy, Precision, Recall, and F1-Score.
  * **File Output**: The final evaluation metrics are saved to a `model_output.txt` file.

## Directory Structure 📂

Your project directory should be set up as follows for the code to run correctly:

```
Framingham-Heart-Disease-Prediction/
│
├── framingham.csv
├── 23ie10036_p2_sayak.py
├── 23ie10036_p2_sayak.ipynb
├── model_output.txt
└── README.md
```

## Requirements ⚙️

You will need Python 3 installed, along with the following libraries:

  * `pandas`
  * `numpy`
  * `scikit-learn`
  * `jupyter` (for the notebook version)

You can install them using pip:

```bash
pip install pandas numpy scikit-learn jupyter
```

-----

## How to Use the Files 📝

There are two ways to run this project: as a Python script or as a Jupyter Notebook.

### \#\# 1. Using the Jupyter Notebook (`.ipynb` file)

This is the recommended approach for an interactive experience where you can see the output of each step.

**Steps:**

1.  **Launch Jupyter Notebook**: Open your terminal or command prompt, navigate to the project directory, and run the command:
    ```bash
    jupyter notebook
    ```
2.  **Open the Notebook**: Your web browser will open a new tab. Click on the `23ie10036_p2_sayak.ipynb` file to open it.
3.  **Run the Cells**: You can run each cell of the notebook sequentially by clicking on a cell and pressing **`Shift + Enter`**. The notebook is divided into logical steps (data loading, training, evaluation) for clarity.
4.  **View the Output**: The output of each step, including the final evaluation metrics and the contents of `model_output.txt`, will be displayed directly below the cells as you run them.

-----

### \#\# 2. Using the Python Script (`.py` file)

This method is suitable for running the entire pipeline from start to finish in a single command.

**Steps:**

1.  **Navigate to Directory**: Open your terminal or command prompt and navigate to the project directory where `23ie10036_p2_sayak.py` and `framingham.csv` are located.
2.  **Run the Script**: Execute the following command:
    ```bash
    python 23ie10036_p2_sayak.py
    ```
3.  **Follow the Process**: The script will print its progress to the terminal, showing each step from data loading and cleaning to model training and final evaluation.
4.  **Check the Output File**: Once the script is finished, a new file named `model_output.txt` will be created in the directory. This file contains the final performance metrics (Accuracy, Precision, Recall, and F1-Score) of the trained model.