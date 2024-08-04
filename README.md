# Fake News Detection

This repository contains the implementation of a fake news detection system using various machine learning models and text feature extraction techniques.

## Overview

The goal of this project is to classify news articles as either "Fake" or "Real" using machine learning algorithms. We use two feature extraction techniques: TF-IDF and Word2Vec, and compare the performance of different models.

## Dataset

The dataset used for this project is the "Fake or Real News" dataset, which contains labeled news articles. The dataset is available in the repository as `fake_or_real_news.csv`.

## Models

We have used the following models for classification:
- Logistic Regression
- Naive Bayes
- Support Vector Machine (SVM)
- Random Forest

## Feature Extraction

Two feature extraction techniques are used:
1. **TF-IDF (Term Frequency-Inverse Document Frequency)**
2. **Word2Vec**

## Results

The performance of each model with both feature extraction techniques is evaluated using the following metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC

### TF-IDF Results
| Model               | Accuracy | Precision | Recall  | F1 Score | ROC AUC |
|---------------------|----------|-----------|---------|----------|---------|
| Logistic Regression | 0.918    | 0.890     | 0.950   | 0.919    | 0.976   |
| Naive Bayes         | 0.852    | 0.971     | 0.719   | 0.826    | 0.964   |
| SVM                 | 0.938    | 0.921     | 0.956   | 0.938    | 0.984   |
| Random Forest       | 0.915    | 0.919     | 0.906   | 0.913    | 0.967   |

### Word2Vec Results
| Model               | Accuracy | Precision | Recall  | F1 Score | ROC AUC |
|---------------------|----------|-----------|---------|----------|---------|
| Logistic Regression | 0.909    | 0.915     | 0.897   | 0.906    | 0.967   |
| SVM                 | 0.910    | 0.920     | 0.893   | 0.907    | 0.965   |
| Random Forest       | 0.893    | 0.899     | 0.879   | 0.889    | 0.963   |

## How to Use

1. **Clone the repository**:
    ```sh
    git clone https://github.com/Lavanya874/Fake-News-Detection.git
    ```

2. **Install the required packages**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Download and set up Git LFS** (if handling large files):
    ```sh
    git lfs install
    git lfs track "*.csv"
    git add .gitattributes
    git commit -m "Track large CSV files with Git LFS"
    ```

4. **Run the Jupyter Notebook**:
    - Navigate to the project directory.
    - Open and run `Fake News Detection.ipynb` to see the implementation and results.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The dataset used in this project was sourced from [Kaggle](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset).
- Special thanks to all the contributors who helped improve this project.
