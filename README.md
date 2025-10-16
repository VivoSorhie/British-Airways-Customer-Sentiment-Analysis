# British Airways Review: Sentiment Analysis & Interactive Dashboard

> An end-to-end project analyzing 3,500+ customer reviews to build a sentiment prediction model and an interactive Tableau dashboard for strategic insights.

![Tableau Dashboard Screenshot](image_b15e25.jpg) 
*(Note: You will need to add your dashboard screenshot to an 'images' folder in your GitHub repo and update the path)*

---

## Table of Contents
* [Project Overview](#project-overview)
* [Interactive Dashboard](#interactive-dashboard)
* [Key Insights from EDA](#key-insights-from-eda)
* [Tech Stack](#tech-stack)
* [Modeling and Results](#modeling-and-results)
* [Installation and Usage](#installation-and-usage)

---

## Project Overview

This project analyzes over 3,500 historical customer reviews of British Airways to uncover actionable insights for improving customer experience. It involves a two-pronged approach:

1.  **NLP Sentiment Model**: A machine learning model trained to accurately classify review text as positive or negative.
2.  **Business Intelligence Dashboard**: An interactive Tableau dashboard created to visualize key trends and allow stakeholders to explore the data dynamically.

The ultimate goal is to translate raw customer feedback into a strategic tool for service recovery and operational improvement.

---

## Interactive Dashboard

A key deliverable of this project is a comprehensive Tableau dashboard designed for business users. It provides a high-level overview of customer satisfaction and allows for deep-dive analysis.

**Key Features:**
* **Executive KPIs**: At-a-glance metrics for overall rating and specific service components like Cabin Staff, Food, Ground Service, and Value for Money.
* **Dynamic Filtering**: Ability to slice the data by date, continent, aircraft type, seat class, and traveller type.
* **Multiple Views**: Includes temporal trends, geographical performance maps, and categorical breakdowns to provide a holistic understanding of the customer experience.

---

## Key Insights from EDA

* **Declining Satisfaction**: Analysis revealed a consistent downward trend in average customer ratings since a peak in 2014, hitting an all-time low in recent years.
* **Service Weaknesses**: `Value for Money` and `Ground Service` were identified as the most significant drivers of customer dissatisfaction.
* **Polarized Feedback**: The review data is highly polarized, with a large volume of very negative reviews (1/10) and a smaller cluster of positive reviews (7-10/10).

---

## Tech Stack
* **Data Analysis & Modeling**: Python, Pandas, Scikit-learn
* **Data Visualization**: Matplotlib, Seaborn
* **BI & Dashboarding**: Tableau
* **Environment**: Jupyter Notebook

---

## Modeling and Results

The project focused on a binary classification task: identifying reviews as **Positive** or **Negative**.

1.  **Feature Engineering**: Review text was vectorized using TF-IDF, incorporating both unigrams and bigrams (`ngram_range=(1, 2)`).
2.  **Model Selection**: A Linear Support Vector Classifier (LinearSVC) was chosen for its strong performance on text data.
3.  **Hyperparameter Tuning**: `GridSearchCV` was used to find the optimal hyperparameters, maximizing the F1-score.
4.  **Final Performance**: The final tuned model achieved an overall **accuracy of 92%**.
    * **Negative Sentiment F1-Score**: 0.93
    * **Positive Sentiment F1-Score**: 0.89

---

