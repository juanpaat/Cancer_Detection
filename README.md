# Optimising Cancer Diagnosis with Gene Expression Data Analysis

## Overview

This repository contains the code and resources for the project *Optimising Cancer Diagnosis with Gene Expression Data Analysis*. The project leverages advanced dimensionality reduction techniques and supervised learning models to enhance the classification of cancer types based on gene expression data. By using statistical and machine learning approaches, this project aims to identify relevant genes and improve model accuracy, providing a robust framework for early cancer detection.

## Table of Contents

1. [Project Description](#project-description)
2. [Data](#data)
3. [Methodology](#methodology)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## Project Description

The project explores various dimensionality reduction methods such as two-sample t-tests, variance-based reduction, and LASSO regression, in addition to imputation techniques like median replacement and kNN imputation. These methods are applied to gene expression data to select relevant features for classifying invasive and non-invasive cancers. Supervised models such as k-Nearest Neighbours (KNN) and Support Vector Machines (SVM) are then trained on the reduced datasets and validated using k-fold cross-validation and bootstrapping techniques.

## Data

- **Source:** Gene expression data from cancer patients, classified as invasive or non-invasive cancer types.
- **Description:** The dataset contains high-dimensional gene expression features, making it ideal for testing dimensionality reduction and feature selection methods.

## Methodology

1. **Preprocessing:**
   - Imputation of missing values using median replacement and kNN imputation.
   
2. **Dimensionality Reduction:**
   - Techniques such as two-sample t-tests, variance-based feature reduction, and LASSO regression.

3. **Model Training:**
   - Supervised models like KNN and SVM trained on reduced datasets.

4. **Validation:**
   - Performance validated using k-fold cross-validation and bootstrapping methods.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/cancer-diagnosis-analysis.git
   cd cancer-diagnosis-analysis
   ```
2. Create a virtual environment and install the required packages:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   pip install -r requirements.txt
   ```

## Usage

1. Prepare the data:
   - Place your gene expression data in the `data/` directory.

2. Run the analysis:
   ```bash
   python analysis.py
   ```

3. View results:
   - Check the `results/` folder for performance metrics and visualisations.

## Results

The project demonstrates that dimensionality reduction techniques like t-tests followed by LASSO regression can significantly improve model performance. The results highlight the effectiveness of using PCA on reduced features for enhanced classification of cancer types.

## Contributing

Contributions are welcome! If you find any issues or want to improve the code, feel free to open a pull request or create an issue in the repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

For more details, please refer to the [project report](./report.pdf).
