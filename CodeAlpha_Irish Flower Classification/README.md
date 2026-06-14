Iris Flower Classification
Task 1 
Name: Dipti Banik

Project Overview
This project builds machine learning models to classify Iris flowers into three species — Setosa, Versicolor, and Virginica — based on their sepal and petal measurements.

Dataset
Source: Kaggle - Iris CSV
Total Samples: 150 (50 per class — perfectly balanced)
Features: SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm
Target: Species (3 classes)
Missing Values: None

Exploratory Data Analysis : Statistical Summary — Mean, std, min, max and quartiles checked for all 4 features Class Distribution — Confirmed each species has exactly 50 samples (perfectly balanced) Feature Distribution Histograms — Plotted distributions of all 4 features grouped by species; revealed that Setosa is clearly separated while Versicolor and Virginica overlap slightly

Models Used
| K-Nearest Neighbors (KNN) | ~96% | | Random Forest | 100% |

Why Random Forest Got 100%?
Random Forest achieved perfect accuracy on this dataset for two reasons:

Small & clean dataset** — Only 150 samples with no noise or missing values, so the model easily learns all patterns.
Well-separated classes** — Especially Setosa, which is linearly separable from the other two species. Versicolor and Virginica have slight overlap, but Random Forest handles that well using multiple decision trees.
In a larger, real-world dataset with noise and imbalance, Random Forest would likely score lower — 100% here reflects the simplicity of the data, not overfitting.

Key Findings
Petal Length & Petal Width are the most important features for classification.
Setosa is perfectly separable from the other two species.
Versicolor and Virginica have some overlap, but models handle it well. KEY INSIGHTS
Petal length & petal width are the strongest features for classification.
Setosa is perfectly separable; Versicolor & Virginica have slight overlap.
Random Forest achieves higher accuracy than KNN on this dataset.
StandardScaler used for both models to ensure fair comparison.

Tools & Libraries
Python, Pandas, NumPy
Scikit-learn (KNN, Random Forest, StandardScaler)
Matplotlib, Seaborn
