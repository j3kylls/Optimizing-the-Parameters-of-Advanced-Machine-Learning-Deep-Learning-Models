```markdown
# To Shroom or Not to Shroom

## Project Overview
This project aims to classify mushrooms as either edible or poisonous based on their physical characteristics using various machine learning and deep learning techniques. The project includes data preprocessing, exploratory data analysis, model training, evaluation, and interpretation using Explainable AI (XAI) methods.

## Team Members
- Aliyan Ahmed
- AbdurRehman Haroon
- Eesha Tariq
- Javeria Shahid

## Table of Contents
- [Introduction](#introduction)
- [Dataset Description](#dataset-description)
- [Edibility Classification](#edibility-classification)
- [Data Preprocessing](#data-preprocessing)
- [Feature Selection](#feature-selection)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Explainable AI](#explainable-ai)
- [Deep Learning Model](#deep-learning-model)
- [Conclusion and Future Work](#conclusion-and-future-work)
- [References](#references)

## Introduction
Mushrooms have a long history of use for food, medicine, and spiritual purposes. However, distinguishing between edible and poisonous mushrooms remains a challenge due to their vast diversity. This project aims to predict the edibility of mushrooms based on their physical traits.

## Dataset Description
The dataset contains 61,069 instances with 20 attributes each. It includes features such as cap diameter, shape, surface, color, gill features, stem attributes, veil properties, ring presence, spore print color, habitat, and season. The dataset is sourced from the [UCIML repository](https://archive.ics.uci.edu/dataset/848/secondary+mushroom+dataset).

## Edibility Classification
Our primary objective is to build a classification model to predict whether a mushroom is edible or poisonous. The evaluation metrics include accuracy, precision, recall, and F-score, with a focus on recall to avoid mislabeling poisonous mushrooms as edible.

## Data Preprocessing
- **Data Imputation:** Missing values were replaced using the mean for numerical columns and mode for categorical columns.
- **Outliers and Duplicates:** Outliers were removed using the Interquartile Range (IQR) method, and duplicates were eliminated to ensure data quality.
- **Class Imbalance:** Addressed using the RandomOverSampler to balance the distribution of the target class.

## Feature Selection
- **Filter Method (SelectKBest):** Extracted the most informative features using the chi-square test.
- **Wrapper Method (RFE):** Implemented but found less reliable than SelectKBest.

## Model Training and Evaluation
Nine different machine learning models were trained and evaluated:
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Gradient Boosting
5. Support Vector Machines
6. K Nearest Neighbors
7. Gaussian Naïve Bayes
8. Linear Discriminant Analysis
9. Quadratic Discriminant Analysis

The best-performing models were selected based on mean test accuracy and other classification metrics.

## Explainable AI
- **SHAP:** Used to interpret the impact of each feature on the model's predictions.
- **LIME:** Provided local explanations for individual predictions to improve model transparency.

## Deep Learning Model
A neural network was implemented with two hidden layers (128 and 64 neurons) and an output layer using the sigmoid activation function. The model was optimized using grid search and evaluated for its performance.

## Conclusion and Future Work
The project successfully demonstrated the classification of mushrooms using various machine learning techniques. Future work includes:
- HTML Parsing to expand the dataset.
- Enhancing image recognition capabilities.
- Developing an interactive web application.
- Deploying the model on mobile platforms.
- Addressing potential overfitting issues.

## References
1. [Exploring the Role of Mushrooms Throughout History](https://rrcultivation.com/blogs/mn/exploring-the-role-of-mushrooms-throughout-history#:~:text=Many%20cultures%20that%20ate%20mushrooms,ceremonies%20in%20the%20Middle%20Ages)
2. [Edible Mushrooms: Attributes and Applications](https://www.taylorfrancis.com/chapters/edit/10.1201/9780203753682-15/edible-mushrooms-attributes-applications-john-buswell-shu-ting-chang)
3. [Mushroom Poisoning](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7868946/)
4. [The Mushroom Hunter's Field Guide](https://books.google.com.pk/books?hl=en&lr=&id=TYI4f6fqrfkC&oi=fnd&pg=PA3&dq=can+you+determine+mushroom+edibility+based+on+features&ots=ZHAYnt3qfR&sig=YJZEWWf35hzH6IoSi4EjMT5q9qI&redir_esc=y#v=onepage&q=can%20you%20determine%20mushroom%20edibility%20based)
5. [Acute Liver Injury From Mushroom Ingestion](https://www.cureus.com/articles/184368-acute-liver-injury-from-mushroom-ingestion-a-timely-intervention-in-mushroom-poisoning)
6. [Demographic, Clinical, and Laboratory Findings of Mushroom-Poisoned Patients in Kermanshah](https://bmcpharmacoltoxicol.biomedcentral.com/articles/10.1186/s40360-022-00614-1#:~:text=The%20actual%20annual%20rate%20of,mushroom%20poisoning%20cases%20%5B12%5D)
7. [Diversity of Edible Mushrooms in Pakistan](https://www.cabidigitallibrary.org/doi/full/10.5555/20093347429)
8. [UCIML Secondary Mushroom Dataset](https://archive.ics.uci.edu/dataset/848/secondary+mushroom+dataset)
9. [7 Steps to Mastering Data Cleaning and Preprocessing Techniques](https://www.kdnuggets.com/2023/08/7-steps-mastering-data-cleaning-preprocessing-techniques.html)
10. [imblearn RandomOverSampler](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.RandomOverSampler.html)
11. [Explainable AI - Understanding and Trusting Machine Learning Models](https://www.datacamp.com/tutorial/explainable-ai-understanding-and-trusting-machine-learning-models)
12. [Mushroom World](https://www.mushroom.world/)
13. [A Review on Evaluation Metrics for Data](https://d1wqtxts1xzle7.cloudfront.net/37219940/5215ijdkp01-libre.pdf?1428316763=&response-content-disposition=inline%3B+filename%3DA_REVIEW_ON_EVALUATION_METRICS_FOR_DATA.pdf&Expires=1713458786&Signature=IhDRdXJJDJrh35X6YEJUqTx6H~R7tr2RHvokaV9DAYOp6NrfmH0)
14. [Secondary Mushroom Dataset](https://archive.ics.uci.edu/dataset/848/secondary+mushroom+dataset)
```
