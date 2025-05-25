# Coding-Club-ML-project

# Task 1

## Overview

We have a student data set of 649 students studying in 2 higher secondary schools collected from a survey. We help to uncover how hidden factors influence student life on campus, from grades to relationships. We also have to design a model that can predict whether a student is in a romantic relationship.

## Level 1

We have to identify 3 anonymized features using data analysis :

- We use value counts for Feature 1 and suspect it to be age
- Plot a line graph of Feature 1 vs average past class failures
- Positive correlation confirms that Feature 1 is Age

- We use value counts for Feature 2 and suspect it to be a categorical feature
- As other lifestyle and behavioral features are already covered in other columns, we suspect it to be study or stress levels
- Plot a line graph of Feature 2 vs average Final grade(G3)
- Positive correlation and slight dip at the end suggests study patterns and confirms Feature 2 to be study time level

- We use value counts for Feature 3 and again suspect it to be a categorical/ordinal feature
- We find similar and proportionate value counts distribution as Dalc, suggesting it could be Walc
- Plot the frequency of value counts for Feature 3 vs Dalc
- Plot a line graph of average freetime vs Feature 3
- Plot a line graph of average goout vs Feature 3
- Similar graph as Dalc and positive correlation with freetime and goout confirms Feature 3 is Walc

## Level 2

- Identification of columns having null values
- Removal of rows with >= 4 null values
- Implementing imputation strategies - using mode for categorical/ordinal features and median for numeric features
- Filling G2 null values with max(G1,G3)

## Level 3

5 plots which have been plotted :

- Line graph of average health vs weekend consumption of alcohol by students
- Box plot with jitter of study time vs final grade received by the students
- Violin plot of parental status vs family relationship quality of students
- Bar chart distribution of number of students in a relationship by school and gender
- Histogram of estimated weekly study hours of students

## Level 4

- Selection of 3 classification models - Logistic Regresseion, Random Forest, SVM
- Finding accuracy first by training the model on all features
- We also plot a bar graph showing feature importance
- Take all features with greater than 0.03 importance and train the model only on these 11 features
- Finding accuracy by training the model on these features
- Overall, logistic regression produced the highest accuracy while considering all the features

## Level 5

- Importing SHAP, xgboost and sklearn libraries
- Plot decision boundaries of different classification models used
- Plot a bar chart showing global feature importance of different features using SHAP
- Generating local explanation for two students – one predicted "yes" and one predicted "no"


# Task 2

## Overview
We are using Langgraph powered by an LLM (we are using Gemini). We have to set up the chatbot, install it with a calculator, then a weather extractor tool and a fashion recommender tool. We also have to make sure this chatbot (WeatherMind) knows which tools to use based on user input and chat with the user accordingly. In brief, WeatherMind is a multi-agent AI system capable of making weather-based fashion recommendations by chaining multiple intelligent agents.

## Level 1

- Importing os and write the API key
- Importing langchain, langgraph and typing
- Constructing the Langgraph node - chatbot
- Defining the calculator tool (follows BODMAS rule) and the calculator node
- Defining chatbot node to make decision to use calculator tool or not
- Rendering the graph of Langgraph as an image in langgraph_visualization.png

## Level 2

- Writing the weather API key from OpenWeatherMap
- Import reports, re and bs4
- Coding the fashion recommender and weather extractor tool

## Level 3

- Classifying specific keywords related to fashion and weather in two groups separately
- Making a memory class so that WeatherMind remembers previous conversations
- Enabling WeatherMind to make decisions based on query which tool to use
- Creating an interaction cell to chat with WeatherMind

## Level 4



