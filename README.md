# Extracting Actionable Insights from User Feedback
In today's competitive market, businesses must continuously adapt and improve their products and services based on customer feedback. User feedback provides valuable insights into customer satisfaction, preferences, and areas needing improvement. However, manually sifting through vast amounts of feedback data can be time-consuming and inefficient. Therefore, automating the process of extracting  actionable insights from user feedback is crucial for timely and effective decision-making. 

#### What are actionable insights?
In its most basic form, actionable insights are meaningful findings that result from raw data in your analytics tool.

### Objective
<ul>
<li>To preprocess IMDB movie reviews for effective sentiment analysis</li>
<li>To classify the reviews into positive and negative sentiments by Sentiment Analysis</li>
<li>To perform topic modeling on negative reviews to identify recurring themes and issues</li>
</ul>

## Methodology
### Approach - 1 :  Sentiment Analysis by Naive Bayes followed by LDA for Topic Modeling

<img width="314" alt="bayesianClassifier" src="https://github.com/user-attachments/assets/e0142ae9-7b2f-4a3e-a86c-9d55d42d3a40">
</br>

#### ComplementNB model -  81.82 %
<img width="316" alt="complementNB" src="https://github.com/user-attachments/assets/5b2f6dd8-a89e-4fd8-8084-a6d3ab72f31f">

#### BernoulliNB model -  82.85 %
<img width="317" alt="bernoulliNB" src="https://github.com/user-attachments/assets/be9e5b16-7ddf-4525-a5da-9a886872120f">

#### MultinomialNB model -  82.02%
<img width="316" alt="multinomialNB" src="https://github.com/user-attachments/assets/f6e51713-5891-4d88-8de9-0d3605af0650">

#### Topics for negative reviews given by LDA model
<img width="308" alt="ldatopics" src="https://github.com/user-attachments/assets/77e830d9-7567-4f93-b622-e22a036a04ec">

#### Coherence Score of LDA model : 0.68 
<img width="311" alt="ldascore" src="https://github.com/user-attachments/assets/8b1e7e04-361a-4253-a8a3-31f5150ff146">

### Approach - 2 : Sentiment Analysis by Bidirectional LSTM followed by LSA for Topic Modeling

#### Bidirectional LSTM - 85.89 %
![bidirectionalLSTM_accuracy](https://github.com/user-attachments/assets/548099d5-2168-4075-8c4a-885a4f9601fe)

#### Topics for negative reviews given by LSA model
<img width="307" alt="lsatopics" src="https://github.com/user-attachments/assets/59c54c51-9db7-4784-ba67-4e5eec3f9a18">

#### Coherence Score of LSA model : 0.7883134196762
<img width="318" alt="lsascore" src="https://github.com/user-attachments/assets/1001ad71-275b-4685-ab24-c1bab7fca849">


