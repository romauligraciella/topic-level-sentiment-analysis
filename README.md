#  💬 Topic-Level Sentiment Analysis on Mobile JKN App Reviews
> Originally developed for undergraduate thesis, this project achieved an A as the final grade.

## Project summary
This project explored what users are saying and how they feel about the Mobile JKN app, the official digital health service developed by BPJS Kesehatan in Indonesia. The goal was not only to classify user sentiment (positive or negative), but also to understand the main topics mentioned in the reviews. A total of 100,000 user reviews, collected from the Google Play Store between September 2018 and March 2025, was used in the analysis. The data was cleaned and preprocessed in two stages for sentiment classification and topic modeling.
For sentiment classification, a BERT-based neural network was used, achieving an **accuracy of 98%**. For topic modeling, BERT embeddings were combined with Deep Embedded Clustering (DEC) to identify topic clusters. The top keywords for each cluster were extracted using class-based TF-IDF (c-TF-IDF), and the interpretation of these keywords into meaningful topics was supported by Generative Pretrained Transformers (GPT). As a result, the analysis identified **4 main topics** with a topic coherence score of 0.23428. 

## Outcome summary
![image](https://github.com/user-attachments/assets/6427be81-2bb5-43d1-900d-ba3b32135a5a)


The topic-level sentiment analysis revealed that Topics 1 and 3 were dominated by negative sentiment, at 96% and 93% respectively. 
This indicates that the majority of users experienced issues related to login access, registration, and account verification.
In contrast, Topics 2 and 4 tended to show more positive sentiment, at 53% and 54% respectively, 
suggesting that while users appreciated certain aspects of information delivery, comfort, and service effectiveness, there are still areas that require improvement.
  
## Recommendation for Developers
- Improve the registration, verification, and login systems to reduce user problem and enhance access reliability.
- Enhance the user interface (UI) to ensure that information is effectively communicated and users experience greater comfort and satisfaction during app usage.
  
## Technologies used
`Python` `Transformers (HuggingFace)` `BERT` `DEC` `google-play-scraper` `scikit-learn` `pandas` `numpy` `matplotlib` `seaborn`
