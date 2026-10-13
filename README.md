# GiftLane: Customer Segmentation and Product Recommendation

## 1. Project Overview

GiftLane is a retail analytics and machine learning project built using the Online Retail II dataset. The project focuses on preparing transaction data, analyzing customer purchasing behavior, developing product recommendation methods, and identifying customer segments.

The goal is to build a data workflow that is efficient, scalable, and useful for understanding customer behavior and supporting personalized product recommendations.

## 2. Project Objectives

- Clean and validate retail transaction data.
- Develop a reproducible data engineering workflow.
- Reduce the storage requirements of customer–product representations.
- Evaluate product recommendations against a top-10 best-seller baseline using a time-based holdout.
- Segment customers into meaningful groups based on purchasing behavior.
- Produce results that can be explained and used to support business decisions.

## 3. Success Criteria

The project will be evaluated against the following criteria:

1. **Storage efficiency:** Represent customer–product purchasing behavior using a compact representation rather than a full dense matrix.
2. **Processing performance:** Keep the data-processing workflow suitable for scheduled execution within the agreed runtime limit.
3. **Recommendation quality:** Evaluate whether the recommendation method outperforms a top-10 best-seller baseline on held-out purchases.
4. **Customer segmentation:** Produce customer segments that can be profiled and explained using purchasing behavior.
5. **Reproducibility:** Keep the workflow and evaluation steps documented so that the analysis can be reviewed and repeated.

Measured results and thresholds will be documented after verifying the corresponding experiments.

## 4. Dataset and Data Preparation

The project uses the UCI Online Retail II dataset, which contains historical retail transactions.

Data preparation includes:
- Removing cancelled transactions.
- Excluding non-positive quantities and prices.
- Filtering non-product transaction codes.
- Removing records without customer identifiers.
- Using a time-based training and test split to evaluate recommendations on later purchases.

The cleaned data is used for subsequent feature construction, recommendation experiments, and customer segmentation.

## 5. Technical Approach

The project combines data engineering and machine learning.

- **Data engineering:** Data cleaning, validation, temporal splitting, aggregation, and efficient data representation.
- **Recommendation systems:** Customer–product interaction analysis and comparison with a best-seller baseline.
- **Customer segmentation:** Grouping customers based on their purchasing behavior and profiling the resulting segments.
- **Evaluation:** Measuring data efficiency, processing performance, recommendation quality, and segment interpretability.

## 6. Project Structure

```text
giftlane-project/
├── data/
│   └── raw/
├── notebooks/
│   └── analysis.ipynb
├── src/
└── .gitignore
```

The main analysis notebook contains the data engineering and machine learning workflow. Raw and generated data files are maintained separately from the tracked analysis notebook.

## 7. Current Status

The data engineering and machine learning workflow has been developed in the main analysis notebook. The notebook is version-controlled using Git and uploaded to GitHub.

The success criteria will be finalized with measured evidence from the experiments, including recommendation performance, storage efficiency, processing runtime, and customer segment profiles.

## 8. Future Improvements

- Improve and benchmark recommendation methods.
- Optimize data processing and storage.
- Strengthen customer segment profiling.
- Document evaluation results and limitations.
- Improve reproducibility and maintainability of the workflow.
