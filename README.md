# E-Commerce Product Recommendation System

This repository contains a hybrid recommendation system for Amazon products. The system combines collaborative filtering and content-based filtering to provide personalized product recommendations.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Cleaning and Transformation](#data-cleaning-and-transformation)
3. [Collaborative Filtering](#collaborative-filtering)
4. [Singular Value Decomposition (SVD) for Collaborative Filtering](#singular-value-decomposition-svd-for-collaborative-filtering)
5. [Generate Collaborative Filtering Recommendations](#generate-collaborative-filtering-recommendations)
6. [Content-Based Filtering](#content-based-filtering)
7. [Hybrid Recommendation System](#hybrid-recommendation-system)
8. [Real-Time Recommendations](#real-time-recommendations)
9. [Evaluation](#evaluation)
10. [Usage](#usage)
11. [Dependencies](#dependencies)

## Introduction

This recommendation system leverages both collaborative filtering and content-based filtering techniques to provide users with personalized product recommendations. The collaborative filtering component uses user-item interaction data, while the content-based filtering component uses product features to make recommendations.

## Data Cleaning and Transformation

The dataset is first cleaned by removing duplicates and handling missing values. Text fields are standardized by converting to lowercase and removing extra spaces.

## Collaborative Filtering

A User-Item Interaction Matrix is created based on implicit feedback (browsing history or purchase interactions). Interactions are treated as binary values.

## Singular Value Decomposition (SVD) for Collaborative Filtering

Singular Value Decomposition (SVD) is applied to factorize the interaction matrix and generate user-product recommendations based on similarity.

## Generate Collaborative Filtering Recommendations

Recommendations are generated based on the similarity between users.

## Content-Based Filtering

Content-Based Filtering is implemented using TF-IDF vectorization. The `combined_features` column (which includes both category and about_product) is used to compute the similarity between products.

## Hybrid Recommendation System

The hybrid recommendation system combines both collaborative and content-based recommendations.

## Real-Time Recommendations

For real-time updates, you can simulate real-time browsing or interaction and immediately generate recommendations based on the recent activity.

## Evaluation

The recommendation system can be evaluated using Precision, Recall, or Mean Average Precision (MAP) by comparing the generated recommendations with actual user preferences.

## Usage

To use the recommendation system, follow these steps:

1. Load the dataset and clean the data.
2. Create the User-Item Interaction Matrix.
3. Apply SVD for dimensionality reduction.
4. Generate collaborative filtering recommendations.
5. Implement content-based filtering using TF-IDF vectorization.
6. Combine collaborative and content-based recommendations to form a hybrid recommendation system.
7. Generate real-time recommendations based on recent user activity.
8. Evaluate the recommendation system using appropriate metrics.

## Dependencies

The following Python libraries are required:

- pandas
- numpy
- scikit-learn

You can install these dependencies using pip:

```sh
pip install pandas numpy scikit-learn
```

To install the dependencies listed in the `requirements.txt` file, you can use the following command:

```sh
pip install -r requirements.txt
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Disclaimer

⚠️ This project is solely for educational purposes to acquire knowledge about Collaborative Filtering and Singular Value Decomposition (SVD) for Collaborative Filtering.