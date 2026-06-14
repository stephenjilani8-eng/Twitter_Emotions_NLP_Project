**BUILDING A MODEL TO RATE SENTIMENTS OF TWEETS ABOUT GOOGLE AND APPLE PRODUCTS**

**1.  BUSINESS UNDERSTANDING**

A Kenyan company an is in a predicament on classifying Twitter sentiments on Google and Apple products. This is with the aim of knowing the perceptions of the products in question to the public. The company has an objective to build a classification models that will help them classify sentiments into positive/negative(binary classification) or positive/neutral/negative(multiclass classification).

**STAKEHOLDERS**

The stakeholder of the project is the Kenyan company at large, however, the specific persons of interest include but not limited to the following:

    1. Customer support.
    2. Product teams.
    3. Sales and marketing department.
    4. Research and development department.

**BUSINESS OBJECTIVES** The primary objective is to build a classification model on twitter reviews on Google and Apple products to better understand customer perception and improve decision making.

    1. Compare multiple models for binary sentiment classification.
    2. Evaluate model performance using F1 Score, precision, and recall.
    3. Provide insights on customer sentiment distribution.

**BUSINESS QUESTIONS**

    1. What are the main drivers of sentiment classification.
    2. What are the most common emotions expressed in reviews.
    3. Which model performs best for sentiment analysis.

**PROJECT SUCCESS METRICS**

This project is going to be a success if the metrics below are met:

    1. If it's possible to identify a binary model that yields the best F1-score, precision and recall.
    2. If it's possible that the multiclass classifier achieves an acceptable F1-score, precision and recall.

**2. DATA UNDERSTANDING**
The data was obtained from CriwdFlower via data.world, and is composed of sentiments which were rated by human raters as positive, negative or either in over 9,000 tweets. The sentiments are in relation to Apple and Google products.

**EXPLORATORY DATA ANALYSIS ON NON-TEXT COLUMNS**

https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/main/Images/Frequency%20Vs%20Brand.PNG

The bar graph shows that Apple products get more revieews compared to the Google products. This may lead to a bias problem in the model. However, a ratio of less that 1:2 is manageable.

https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/main/Images/Frequency%20Vs%20Sentiment.PNG

The bar graph shows that neutral emotions are the majority in the dataset, followed by positive and then negative emotions. This may be an indication that Twitter users are quite indifferent when it comes to choosing either Google or Apple products.

https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/main/Images/Frequency%20Vs%20Brand%20Vs%20Sentiment%20Stacked.PNG

The graph above shows that Apple products are more talked about compared to google products. This is evident in Apple products having more frequency in the dataset. However, the most sentiments are the neutral ones meaning that most reviewers are indifferent on the products they use.

**EXPLORATORY DATA ANALYSIS ON TEXT COLUMN**

https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/main/Images/Frequent%20words%20Vs%20frequency.PNG

The graph shows the most frequent words in the dataset.

https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/main/Images/Frequent%20Bigrams%20Vs%20Frequency.PNG

The graph shows the most frequent bigrams in the dataset.