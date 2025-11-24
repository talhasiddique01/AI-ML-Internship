# Task 1: Exploring and Visualizing the Iris Dataset

## Task Objective
The objective of this task is to explore and visualize a simple dataset to understand the underlying patterns, relationships between features, and data distributions. This helps in gaining insights before applying any machine learning models.

## Dataset Used
- Dataset Name: Iris Dataset  
- Source: Seaborn library (`sns.load_dataset('iris’) `)  
- Description: The Iris dataset consists of 150 samples of iris flowers from three species (`setosa`, `versicolor`, `virginica`).  
- Features: 
  - `sepal_length` (cm)
  - `sepal_width` (cm)
  - `petal_length` (cm)
  - `petal_width` (cm)
  - `species` (target class)

## Models Applied
- No predictive models were applied in this task. This task focuses on exploratory data analysis (EDA) and visualization techniques:
  - Scatter plots
  - Pair plots
  - Histograms
  - Box plots

## Key Results and Findings
- Scatter Plots: Showed clear separability between species for some feature pairs, especially petal dimensions.  
- Pair Plots: Provided a comprehensive view of relationships between all features and highlighted clustering of species.  
- Histograms:  Revealed the distribution and spread of each feature.  
- Box Plots: Helped identify potential outliers and compare feature ranges across species.  

Overall, the Iris dataset exhibits distinct clusters based on species, particularly when using petal length and width features, which can guide further modelling and classification tasks.
