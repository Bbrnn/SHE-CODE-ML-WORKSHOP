#  Diabetes prediction

##  Description

This project is a machine learning workshop organized by SHE CODE. It aims to introduce participants to the fundamentals of machine learning and provide hands-on experience with various ML algorithms and techniques. I learned two new features: YData Profiling, used in data analysis, and AutoGluon, used for model prediction.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  

## Installation

To get started with this project, follow these steps:

1. Clone the repository: `git clone https://github.com/Bbrnn/SHE-CODE-ML-WORKSHOP.git`

## Usage

### Exploratory Data Analysis with YData Profiling
One of the key components of this workshop is the use of YData Profiling for exploratory data analysis. YData Profiling is a powerful tool that provides comprehensive insights into your dataset, helping you understand its structure, identify missing values, outliers, and much more. To use YData Profiling, follow these steps:

1. Install YData Profiling: `pip install ydata_profiling`
2. Import the library in your Python script: `from  ydata_profiling import ProfileReport`
3. Load your dataset using pandas: `import pandas as pd; data = pd.read_csv('path/to/your/dataset.csv')`
4. Generate the profile report: `profile = ProfileReport(data); profile.to_file("your_report.html")`

### AutoML with AutoGluon
Another important aspect of this workshop is the use of AutoGluon for automated machine learning (AutoML). AutoGluon is a powerful AutoML toolkit that simplifies the process of training and tuning machine learning models. To use AutoGluon, follow these steps:

1. Install AutoGluon: `pip install autogluon`
2. Import the library in your Python script: `from autogluon.tabular import TabularPredictor`
3. Load your dataset: `train_data = TabularPredictor.load_csv('path/to/your/train_data.csv')`
4. Define the target variable: `label = 'target_column_name'`
5. Train the model: `predictor = TabularPredictor(label=label).fit(train_data)`
6. Make predictions: `test_data = TabularPredictor.load_csv('path/to/your/test_data.csv')`<br>
    `predictions = predictor.predict(test_data)`

Remember to replace `'path/to/your/dataset.csv'`, `'path/to/your/train_data.csv'`, and `'path/to/your/test_data.csv'` with the actual paths to your dataset files.

