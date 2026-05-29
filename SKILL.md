# Applied ML Coursework Skill

## Purpose

This skill helps with applied machine learning, data science, and data mining coursework. It supports the full workflow from understanding an assignment brief to designing experiments, building notebooks, evaluating models, interpreting results, writing reports, and checking final deliverables.

It is suitable for coursework involving:

- exploratory data analysis
- data preprocessing
- feature engineering
- classification
- regression
- clustering
- association rule mining
- text mining
- time series prediction
- model comparison
- academic report writing

The skill should not invent results, citations, datasets, or unsupported claims.

---

## When to Use This Skill

Use this skill when the user is working on a practical data or machine learning assignment and needs help with:

- reading the assignment brief
- understanding required tasks
- planning a Jupyter Notebook
- choosing suitable algorithms
- checking for data leakage
- evaluating model performance
- interpreting tables and figures
- writing an academic report
- checking final deliverables

---

## Core Workflow

Follow this workflow unless the user asks for a different approach:

1. Read and summarize the assignment brief.
2. Identify required tasks, methods, metrics, and deliverables.
3. Review lecture slides or rubrics if provided.
4. Inspect the dataset or help choose a suitable dataset.
5. Define the modelling or analysis problem.
6. Identify input features, target variables, labels, and fields to exclude.
7. Check for possible data leakage.
8. Plan the notebook or code structure.
9. Perform focused exploratory data analysis.
10. Apply preprocessing and feature engineering.
11. Run the required algorithms.
12. Evaluate results using suitable metrics.
13. Generate required tables and figures.
14. Interpret results in simple academic language.
15. Compare methods if required.
16. Draft or improve the report.
17. Check final submission files.

---

## Important Rule: Do Not Invent Results

Only use actual results from the user's notebook, output files, screenshots, or provided data.

Do not invent:

- accuracy values
- F1-scores
- confusion matrix values
- clustering results
- table values
- references
- dataset details

If a result is missing, ask the user to run the notebook or inspect the output file.

---

## Data Leakage Check

Always check whether some columns directly or indirectly reveal the target.

Examples of risky columns:

- ID fields
- target-related IDs
- category IDs
- cluster IDs
- labels
- post-event fields
- duplicated target information

For supervised learning, target labels must not be used as input features.

For unsupervised learning, labels must not be used during clustering. Labels may only be used after clustering for interpretation.

---

## Classification Guidance

For classification tasks, include:

- task definition
- input features
- target variable
- train/test split
- at least the required number of algorithms
- accuracy
- precision
- recall
- F1-score
- confusion matrix
- model comparison
- explanation of the best model
- discussion of common errors

For multi-class classification, clarify whether macro average, weighted average, or both should be used.

If the user wants to treat all classes equally, use macro precision, macro recall, and macro F1-score as the main metrics.

---

## Regression Guidance

For regression tasks, include:

- target variable
- input features
- train/test split
- algorithms used
- MAE
- MSE
- RMSE
- R-squared if appropriate
- discussion of prediction errors

Do not use classification metrics for regression tasks.

---

## Clustering Guidance

For clustering tasks, include:

- clustering task definition
- input features
- clustering algorithm
- method for choosing the number of clusters
- cluster visualization if useful
- cluster interpretation
- limitations

For K-Means:

- test several values of k
- plot inertia against k
- use the Elbow Method
- explain that inertia normally decreases as k increases
- do not claim there is a clear elbow if the plot is unclear
- select k based on both the elbow trend and interpretability if needed

---

## Association Rule Mining Guidance

For association rule mining tasks, include:

- transaction definition
- itemset preparation
- minimum support
- minimum confidence
- lift
- frequent itemsets
- association rules
- interpretation of useful rules

Explain:

- support means how often an itemset appears
- confidence means how often the consequent appears when the antecedent appears
- lift means how much stronger the rule is compared with random co-occurrence

Warn that high confidence alone can be misleading if lift is low.

---

## Text Mining Guidance

For text datasets:

- use simple text cleaning
- keep meaningful numbers if they represent model numbers, sizes, capacity, or technical specifications
- use TF-IDF for basic text classification or clustering
- use TruncatedSVD when dimensionality reduction is needed for sparse TF-IDF features

Avoid unnecessary complex NLP methods unless the assignment requires them.

---

## Report Writing Guidance

Use simple academic English.

A general report structure can be:

1. Introduction
2. Dataset Description
3. Exploratory Data Analysis
4. Data Preprocessing
5. Methodology
6. Results
7. Discussion
8. Conclusion
9. References
10. Appendix

Keep the report focused on assignment requirements.

Avoid:

- overly long theory
- unnecessary EDA
- generic AI-style writing
- unsupported claims
- invented citations
- invented results

---

## Final Deliverables Checklist

Before submission, check whether the user has:

- final report
- notebook or source code
- required figures
- required tables
- performance metrics
- references
- appendix or code link if needed
- clear file names
- no private data accidentally included