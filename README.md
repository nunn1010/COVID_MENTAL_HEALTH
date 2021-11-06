## Project Abstract
COVID-19 has significantly disrupted all facets of life for Canadians. Accordingly, multiple studies1,2,3  have demonstrated the significant impact that the pandemic has had on the mental health of Canadians. As the pandemic persists and restrictions continue to fluctuate throughout the country, Canadians are likely to continue facing associated mental health challenges. However, the exact nature of these challenges are difficult to predict. While it is generally accepted that COVID-19 is negatively impacting mental health, the magnitude and type of mental health issues likely to arise remains an area of open investigation. Additionally, how these changes are associated with specific public health measures in Canada is not well understood. 

In order to effectively address these issues, it is important to understand the types of mental health services that are likely to see an increased demand due to COVID-19. Additionally, understanding how mental health issues related to COVID-19 vary across demographics and regions may help to effectively allocate resources to meet growing demands. 

Research Question
●	Can we build a text classification model to effectively predict the mental health indication related to a social media post?


Data Sources

Reddit Data: 
Approximate file size: 8414 KB (~18407 mentions)

Twitter Data:
Approximate File Size: 5174KB (~7588 mentions)



Approach

Social media posts relating to specific mental health conditions will be retrieved from subreddits dedicated to conversations on those indications (r/Depression, r/Anxiety, r/Bipolar, r/Schizophrenia). These posts will be used as labelled inputs to train a text classification model to interpret the specific indication of mental health related Tweets. By analyzing the distribution of Tweets within each mental health indication, we aim to understand which mental health issues have seen the highest demand during COVID-19.





Techniques Used
 














Steps

1.	Extract labelled social posts related to various mental health indications from subreddits
2.	Feature Engineering:
○	Text preprocessing via NLTK library
○	Label encoding
○	TF-IDF via Scikitlearn tfidfVectorizer
3.	Predictive Model:
○	Results from Naïve Bayes, Logistic Regression and KNN models will be compared in order to select the most accurate model. 
○	Accuracy will be used to assess model performance. This metric is selected over other metrics such as Precision, Recall & F1 score we are not using binary classification (making these metrics more tedious to interpret) and we are interested only in correct categorization of posts - sensitivity and specificity based on false negatives and false positives is not particularly valuable in the context of our analysis.

Output
A model will be produced which is able to predict the mental health indication a social media post is related to. In future projects, this model can be applied to categorize social media posts and understand which mental health indications are seeing an increase in activity over time. Additionally, by analyzing mental health post distributions regionally based on Twitter data, this model can be used to evaluate which areas of Canada may require a higher level of mental health support within various indications.

Link to Github Repository

https://github.com/nunn1010/COVID_MENTAL_HEALTH.git

