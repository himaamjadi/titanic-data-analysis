
# Titanic Data Analysis

This project performs data analysis on the Titanic dataset from Kaggle using Google Colab. The analysis includes data preprocessing, feature engineering, and training a machine learning model to predict survival.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis Steps](#analysis-steps)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Titanic dataset is a famous dataset used in data science and machine learning. The goal is to predict whether a passenger survived the sinking of the Titanic based on features like age, gender, class, etc. This project utilizes the dataset to build and evaluate a predictive model.

## Dataset
The dataset used in this project is obtained from the Kaggle Titanic competition:
[Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)

The dataset includes the following files:
- `train.csv`: The training dataset
- `test.csv`: The test dataset

## Installation
To run this project, you need to set up a Google Colab environment and have a Kaggle account.

1. Clone the repository:
    ```bash
    git clone https://github.com/<your-username>/titanic-data-analysis.git
    cd titanic-data-analysis
    ```

2. Install the Kaggle API in your Colab environment:
    ```python
    !pip install kaggle
    ```

3. Upload your `kaggle.json` file to Colab and set up the Kaggle API token:
    ```python
    from google.colab import files
    files.upload()  # Upload the kaggle.json file

    !mkdir -p ~/.kaggle
    !cp kaggle.json ~/.kaggle/
    !chmod 600 ~/.kaggle/kaggle.json
    ```

4. Download the Titanic dataset:
    ```python
    !kaggle competitions download -c titanic
    !unzip titanic.zip
    ```

## Usage
Open the `titanic_data_analysis.ipynb` notebook in Google Colab and run the cells to perform the data analysis.

## Analysis Steps
1. **Load and Analyze the Dataset**
    - Load the dataset
    - Display basic information and data distribution
    - Check for missing values

2. **Basic Data Analysis**
    - Visualize survival distribution
    - Visualize survival rate by class

3. **Feature Engineering**
    - Handle missing values
    - Convert categorical features to numeric

4. **Model Training and Evaluation**
    - Split the data into training and testing sets
    - Train a Random Forest classifier
    - Evaluate the model's performance

## Results
The final model achieves an accuracy of approximately `X%` on the test set. Detailed evaluation metrics and visualizations are provided in the notebook.

## Contributing
Contributions are welcome! Please create an issue or submit a pull request.

## License
This project is licensed under the MIT License.
