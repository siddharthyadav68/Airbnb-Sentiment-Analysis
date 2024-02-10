# Airbnb-Sentiment-Analysis
The dataset under analysis, "San Diego Airbnb Reviews and Ratings," focuses on the sentiment expressed in reviews for listings in San Diego. Sentiment analysis categorizes reviews as positive, neutral, or negative, providing valuable insights into the perceptions of Airbnb guests regarding their stay experiences.

Introduction
Founded in 2008, Airbnb has become a leading force in the hospitality industry, transforming the way people travel and experience accommodations. This online platform connects hosts offering unique stays with travelers seeking personalized and authentic lodging experiences, creating a global community that goes beyond traditional hotel accommodations.
The dataset under analysis, "San Diego Airbnb Reviews and Ratings," focuses on the sentiment expressed in reviews for listings in San Diego. Sentiment analysis categorizes reviews as positive, neutral, or negative, providing valuable insights into the perceptions of Airbnb guests regarding their stay experiences.

Questions we would like to answer for the analysis is as follows:
HOW CAN AIRBNB DETECT AND ANALYZE SENTIMENT IN REVIEWS?
ANY RELATIONSHIPS BETWEEN  VARIABLES AND REVIEW SENTIMENT?
Visualize data to see the relationship with other variables
Perform a Sentiment Analysis to detect positive and negative reviews 
Analyze Word Frequency

Data
Data Overview
Sourced information from two key datasets: 'listings.csv' and 'reviews.csv’.
'listings.csv' provides comprehensive details about Airbnb listings, including:
Listing specifics like ID, name, and description. 
Host information. 
Property features such as room types and amenities. 
Guest review scores on various aspects. 

'reviews.csv' includes:
Actual guest review texts. 
Metadata like review ID, listing ID, and date. 
These datasets together form the basis for our sentiment analysis, linking guest opinions to specific properties and experiences.

Data Preprocessing 
Identified and removed missing data from the 'review' dataset. 
Combined listing details with corresponding reviews through an inner join on listing ID.

Analysis 
1. Sentiment Analysis
Sentiment Analysis is a type of Natural Language Processing(NLP) method that classifies texts into various sentiments, such as positive, negative and neutral.
In this analysis, we used NLTK’s VADER(Valance Aware Dictionary for Sentiment Reasoning), which is a pre-trained machine learning model. Since it is pre-trained based on social media text data, it seemed to suit our case, which is to look at customer reviews on the website and we decided to use the model. The model gives immediate sentiment scoring by extracting various  sentiment dimensions: compound, negative, neutral, and positive. For each sentiment it provides the percentage of the sentiment in the text along with the compound score. The compound score is the sum of positive, negative and neutral scores which is then normalized between -1, which is extreme negative and -1, which is extreme positive.

Conclusion
A comprehensive sentiment analysis of Airbnb reviews yielded valuable insights into customer perceptions and preferences. The analysis highlighted key themes, identified areas for improvement, and underscored factors contributing to positive customer experiences. Airbnb should prioritize maintaining positive aspects and addressing concerns raised in negative reviews to enhance customer satisfaction and solidify its market position. Continuous sentiment monitoring can ensure proactive identification of trends and issues, driving business growth and industry leadership.
