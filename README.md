# Movie Recommender System

This project implements a movie recommender system using the well-known MovieLens dataset. The code utilizes the small version of the dataset for simplicity.

## Dataset

The MovieLens dataset is retrieved from the GroupLens research group and contains user ratings for movies. The dataset is downloaded from the provided URL and stored locally for processing.

## Setup

To run the code successfully, ensure the following dependencies are installed:

- `numpy`
- `requests`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-surprise`

## Code Overview

The code performs the following steps:

1. Downloads and extracts the MovieLens dataset from the GroupLens website.
2. Reads the ratings and movies data into pandas DataFrames.
3. Preprocesses the data by filtering movies and users based on a minimum number of ratings.
4. Analyzes the distribution of ratings per user and per movie using histograms.
5. Evaluates different recommender algorithms (KNNBasic, SVD, SlopeOne, NMF) using cross-validation and computes the RMSE and MAE metrics.
6. Compares the performance of the algorithms and visualizes the results using bar plots.

## Results

The evaluation results show the performance of each algorithm based on the test RMSE and MAE metrics. The computation time for fitting and testing the algorithms is also provided.

The SVD algorithm performed the best in terms of test RMSE and test MAE, followed by SlopeOne and NMF. KNNBasic performed the worst among the evaluated algorithms.

## Usage and Customization

The provided code serves as a starting point for building a movie recommender system. You can further customize and experiment with different algorithms or try different variations of the dataset.

## Conclusion

The Movie Recommender System demonstrates the use of collaborative filtering algorithms to generate movie recommendations based on user ratings. The project provides insights into the performance of different recommender algorithms and helps in choosing the most suitable algorithm for a specific dataset.

