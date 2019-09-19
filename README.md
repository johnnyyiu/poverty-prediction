# Poverty Prediction (Microsoft Data Science Professional Certification)

## Overview
The motivation of creating this notebook is a data science competition hosted by **Microsoft** and **DrivenData**, which is a part of the Capstone project of the **Microsoft Professional Certificate in Data Science** and also my very first competition related to machine learning. By the end of the competition, I was at the **top 4%** on the leaderboard, and I am happy to share with you my approach, especially to those who are just beginning their journey on data science.

<a href="https://datasciencecapstone.org/competitions/15/predicting-poverty/leaderboard/"><img src="https://i.imgur.com/Yo4Oeya.png" title="Leaderboard" /></a>

<a href="https://datasciencecapstone.org/competitions/15/predicting-poverty/leaderboard/"><img src="https://i.imgur.com/ItktCZr.png" title="Best Score" /></a>

## Goal
Participants are to predict the probability that individuals across 7 different countries live below the poverty line at the $2.50/day threshold, given other socioeconomic indicators. The probability of being in poverty was calculated using the **Poverty Probability Index (PPI)**, which estimates an individual's poverty status using 10 questions about a household’s characteristics and asset ownership. The remaining data comes from the **Financial Inclusion Insights** household surveys conducted by InterMedia.

<a href="https://www.povertyindex.org"><img src="https://www.povertyindex.org/sites/default/files/PPI-logo-RGB-header-image.png" title="PPI" /></a>
<a href="http://finclusion.org"><img src="https://i.imgur.com/jjPjT06.png" title="Fii" /></a>

## Data
The dataset was retrieved from datasciencecapstone.org and contains the PPI along with 58 features of 12,600 individuals across 7 different countries.

**Information on the competition and the data:**
https://datasciencecapstone.org/competitions/15/predicting-poverty/page/47/

## Model
I have hand-picked 3 regression-based models (Gboost, XGBoost and LightGBM) and used a 5-fold cross validation to evaluation their performance. A stacked model of the 3 is then tested for prediction results. The final r2 score was 0.4213, resulting a top 4% on the leaderboard. 

**The model stacking approach here is inspired by Serigne, make sure to check it out at:**
[Serigne's Stacked Regressions Notebook](https://www.kaggle.com/serigne/stacked-regressions-top-4-on-leaderboard).

Please check out my kaggle kernel for run result, and if you liked it - give it an up-vote!! :) 
https://www.kaggle.com/johnnyyiu/poverty-prediction-from-visualization-to-stacking

