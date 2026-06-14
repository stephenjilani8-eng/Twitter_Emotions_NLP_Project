**BUILDING A MODEL TO RATE SENTIMENTS OF TWEETS ABOUT GOOGLE AND APPLE PRODUCTS**

**BUSINESS UNDERSTANDING**

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



The bar graph shows that Apple products get more revieews compared to the Google products. This may lead to a bias problem in the model. However, a ratio of less that 1:2 is manageable.



The bar graph shows that neutral emotions are the majority in the dataset, followed by positive and then negative emotions. This may be an indication that Twitter users are quite indifferent when it comes to choosing either Google or Apple products.


![Frequency vs brand](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/bc290089124e92c9d8ee28dafd657bf52d9cb213/Images/Frequency%20Vs%20Brand.PNG)

The bar graph shows that Apple products get more revieews compared to the Google products. This may lead to a bias problem in the model. However, a ratio of less that 1:2 is manageable.

![Frequency vs Sentiment](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/62c52299385258692c03f5d68319d771328ce294/Images/Frequency%20Vs%20Sentiment.PNG)

The bar graph shows that neutral emotions are the majority in the dataset, followed by positive and then negative emotions. This may be an indication that Twitter users are quite indifferent when it comes to choosing either Google or Apple products.

![Frequency Vs Brand Vs Sentiment Stacked](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/fe2f43f088a3dd399326994b647720672aeb4c26/Images/Frequency%20Vs%20Brand%20Vs%20Sentiment%20Stacked.PNG)

The graph above shows that Apple products are more talked about compared to google products. This is evident in Apple products having more frequency in the dataset. However, the most sentiments are the neutral ones meaning that most reviewers are indifferent on the products they use.

**EXPLORATORY DATA ANALYSIS ON TEXT COLUMN**


![Frequent words Vs frequency](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/651e1986763012ac0358f6f95b0b9d95e3ba5903/Images/Frequent%20words%20Vs%20frequency.PNG)
The graph shows the most frequent words in the dataset.

![Frequent Bigrams Vs Frequency](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/adcf51ed714253539702635ccfd0baefb7b16c1e/Images/Frequent%20Bigrams%20Vs%20Frequency.PNG)
The graph shows the most frequent bigrams in the dataset.



**MODELLING AND MODEL EVALUATION**

**i. Binary Classification**
The best model was the tuned XGBoost model whose confusion matrix is as below.

![Tuned XGBoost Binary model](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/b4f65432e08b1ba3c246623c692e59e9b5f4ec1e/Images/Tuned%20XGBoost%20Binary%20Model.PNG)

**Feature importance in Binary Classification**
![Feature importance in Binary Classification](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/24b37aa9466eae8b047a06a797b366de809fb3ab/Images/Feature%20importance%20Binary%20classification.PNG)


**ii. Multiclass Classification**

The best model is the  tuned XGBoost model whose confusion matrix is as below.

![Tuned XGBoost multiclass model](https://github.com/stephenjilani8-eng/Twitter_Emotions_NLP_Project/blob/9e55c95224d9d755371432bac9a34bb1f0f26346/Images/Tuned%20XGBoost%20Multiclass%20Model.PNG)

**Feature importance in Multiclass Classification**

**FINAL MODEL SELECTION**

**i. Binary Classification**

Based on the models above and the insights on each one of them, the best model is the tuned XGBoost Model which achieved an improvement in recall and f1 score for Negative emotions. On the other hand, precision, recall and f1 score maintained at te level with its base model. This generally led to an improvement in the performance of the model hance making it the best model.

**ii. Multiclass Classification**

Multicalass classification was done on XGBoost only with a base and a tuned model. There was a reduction in precision for Negative emotions, an increase for Neutral and Positive emotions. In recall, there was an increase in Negative emotions, a reduction in Neutral emotions and an increase in Positive emotions. For f1-score, there was an increase for Negative emotions, nochange for Neutral Emotions and an increase for Positive emotions. Generally, this model performed better than the base model for MultiClass classification hence making it the better model.




**BUSINESS RECOMMENDATIONS**

1. The stakeholders should implement the best models in the classification of review sentiments
2. The stakeholders need to analys top features that drive negative emotions like headache, suck, hate and identify what exactly lead to such sentiments.
3. The stakeholders should focus more on negative sentiments and route them to customer support and product teams

**EXPECTED IMPACT**

1. Improved customer satisfaction.
2. Understading of product perception in customers

**LIMITATIONS**

1. Class imbalance in the dataset may influence the performance of the model as the data contains very few negatives and a majority of neutral sentiments.
2. The data was social media noisy and that may affect the performance of the model
3. The data may be from a specific region in the world and may not be fit for the stakeholder’s region


The graph shows the most frequent words in the dataset.



The graph shows the most frequent bigrams in the dataset.
