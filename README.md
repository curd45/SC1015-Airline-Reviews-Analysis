# SC1015-Airline-Reviews-Analysis

## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on analysing passenger reviews on airlines. 

## Problem Definition
Analyse airline reviews to identify factors affecting passenger ratings and recommendations. Given a list of passenger reviews, we wanted to analyse the importance of various cabin classes in the rating and recommendation of an airline. Moreover, we also wanted to rank the factors that matters most to passengers (from these 'Seat Comfort', 'Cabin Staff Service', 'Food & Beverages', 'Ground Service', 'Inflight Entertainment', 'Wifi & Connectivity', 'Value for Money') and also looked at how the rankings have changed before and after COVID. 

For simplicity sake, we split reviews before 1 Jan 2020 as pre COVID and reviews on and after 1 Jan 2020 as post COVID

At the end, we have also provided our final judgement by ranking the factors and provided actionable insights that airlines can undertake to boost their overall rating and recommendation numbers. 

## Project Summary 
The dataset we used for this project is from Kaggle (https://www.kaggle.com/datasets/juhibhojani/airline-reviews) 

### Project Motivation
With the ever increasing demand for global travel and the constant push by airlines to attract and retain customers, we wanted to analyse what factors matter most to a passenger when evaluating an airline. 

### Data Preperation
We dropped unverified reviews to have a reliable basis for our analysis. Moreover, we identified that many reviews had NaN values for certain columns potentially due to the fact that the airline or route they were flying on did not offer those services. Hence, we created two datasets, one that fills NaN values with 0 to retain airlines that do not offer the full suite of services and the other that drops all rows with NaN values to ensure our analysis is not skewed in any way. 

### Exploratory Data Analysis 
We analysed how seat type affects the mean overall rating and recommendation and then looked at how ('Seat Comfort', 'Cabin Staff Service', 'Food & Beverages', 'Ground Service', 'Inflight Entertainment', 'Wifi & Connectivity') affects the mean overall rating and recommendation as well. 

### Machine Learning Techniques
We used the decision tree as our base model to evalaute factors. Then, we looked at Random Forest to improve classfication accuracy. Lastly, we implemented an XGBoost Model that allows airlines to predict their overall rating and recommendation status by inputing values for these ('Seat Comfort', 'Cabin Staff Service', 'Food & Beverages', 'Ground Service', 'Inflight Entertainment', 'Wifi & Connectivity') factors. 

### Data Driven Insights 
Seat Types that yield the best reviews for Airlines:

Recommendation -> 1) First Class, 2) Business Class, 3) Premium Economy, 4) Economy
Overall Rating -> 1) Business Class, 2) First Class, 3) Premium Economy, 4) Economy

Top Services to Focus on for Airlines (Our Final Judgement)

Recommendation -> 1) Ground Service, 2) Seat Comfort, 3) Food & Beverages
Overall Rating -> 1) Ground Service, 2) Cabin Staff Service, 3) Seat Comfort

### Contributors
@Wong Yi Jie - Data Preparation and EDA
@Timothy - EDA & XGBoost
@curd45 (Param) - Problem, ML and Data Driven Insights

Full source code can be found in the Airline Review.ipynb


### References
https://www.kaggle.com/datasets/juhibhojani/airline-reviews
<br> https://www.iata.org/en/pressroom/2022-releases/2022-03-01-01/
<br> https://www.iata.org/en/pressroom/2023-releases/2023-12-06-01/#:~:text=Airline%20profitability%20for%202023%20performed,93%20billion%20higher%20than%20expected
