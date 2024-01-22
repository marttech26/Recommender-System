# Movie Recommendation System 

## Overview

![recommendations readme](https://github.com/Perception-ui/phase_4/assets/139771882/39015c1f-e986-43fc-8570-95464634040b)

This project entails the development of a movie recommendation system utilizing collaborative filtering techniques on the MovieLens dataset. The primary objective is to provide users with personalized top 5 movie suggestions based on their preferences and historical ratings.

The document comprehensively covers the entire data science life cycle, including business understanding, data cleaning, exploratory analysis, modeling, evaluation, and final model deployment.

## Business Understanding

The central business objective is to enhance user engagement and satisfaction on a streaming platform by delivering tailored movie recommendations. The ultimate goal is to prolong user interaction with the platform, potentially leading to increased revenue.

## Problem Statement

To achieve our business objective, the project aims to actively involve users by delivering personalized movie recommendations. This involves employing machine learning algorithms, specifically collaborative filtering and content-based filtering, to analyze user ratings and preferences.

## Metric of Success

The success of the model will be measured by the Root Mean Squared Error (RMSE).

## Objectives
### Primary Objective:

Develop and implement a movie recommendation system using collaborative filtering techniques to provide personalized top 5 movie recommendations for users.

### Specific Objectives:

  1.Understand movie ratings distribution and user preferences.<br>
  2.Analyze data to identify highest-rated movies.<br>
  3.Examine monthly user engagement.<br>
  4.Analyze and identify highest-rated genres.<br>

## Data Understanding

The MovieLens dataset consists of 100,000 ratings from 610 users across 9,742 movies ranging from March 1996 to September 2018.

It comprises 4 key data files - movies, links, ratings, tags. The movies and ratings files were the primary data sources.

The movies file contains movie titles, genres. The ratings file has details of user ratings on a 5-star scale.

## Data Preparation

Data preparation involved merging key movies and ratings data files into a single DataFrame using pandas. Extensive data cleaning was performed, including missing value treatment, duplicate removal, and feature engineering.

## Exploratory Data Analysis
Both univariate and bivariate analyses were performed:

Analyzed peak hourly and monthly viewing trends and rating patterns

Computed average ratings per user and overall distributions

Studied correlations of ratings with genres using plots and heatmaps

Identified most frequently rated and highest/lowest rated movies

## Model Building

The Surprise library was leveraged to develop a collaborative filtering recommendation system. Multiple techniques were compared, and hyperparameters were tuned using grid search. The final model, a Matrix factorization SVD algorithm with 50 latent factors and 0.05 regularization, achieved the lowest RMSE of 0.8686 on the test set.

## Model Usage

The recommendation system adapts to evolving user preferences and displays the top 5 movie recommendations based on the SVD model.

## Conclusions

The SVD model was chosen for its superior performance in building the recommendation system.<br> 
User ratings were effectively incorporated to personalize suggestions, and the system successfully adapts to changing user preferences.

## Recommendations

*Web application:* Develop a web application to enhance user interaction and increase accessibility to the collaborative filtering recommendation system.

*Explore Deep Learning Models:* Consider exploring deep learning-based recommendation models, such as neural collaborative filtering (NCF) or recurrent neural networks (RNNs), to capture complex patterns and dependencies in user behavior.

## Next Steps

Implement a real-time recommendation system to provide users with up-to-date suggestions. Continuously update the model based on new ratings and interactions, ensuring the provision of current and pertinent movie suggestions. This approach is poised to significantly elevate user engagement on the platform.

## Collaborators

[Lewis Otsieka](https://github.com/Perception-ui)<br>
[Ejidiah Kanyi](https://github.com/EjiKanyi)<br>
[Gichogu Macharia](https://github.com/Mr-Macharia)<br>
[Laureen Chepkoech](https://github.com/Lawrync)<br>
[Yusra Mohamed](https://github.com/Yusra12)<br>
[Emmanuel Rono](https://github.com/marttech26)<br>
