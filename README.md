#  💬 Topic-Level Sentiment Analysis on Mobile JKN App Reviews
> Originally developed for undergraduate thesis, this project achieved an A as the final grade.

## Project summary
This project entailed topic-level sentiment analysis of user feedback on the Mobile JKN application, 
the official digital health service platform developed by BPJS Kesehatan in Indonesia. 
The objective was to not only categorize user sentiments (positive or negative) but also to uncover the primary topics of discussion within the reviews. 
The dataset, comprising 100,000 reviews scraped from Google Play Store (from September 2018 to March 2025), was cleaned and preprocessed through two stages, 
each tailored for sentiment classification and topic identification, respectively. 
Specifically, I employed a BERT-based neural network (BERT-NN) to categorize user sentiments, attaining an **accuracy of 98%**. 
For topic detection, I utilized BERT embeddings combined with Deep Embedded Clustering (DEC) to identify topic clusters. 
The top keywords for each cluster were extracted using class-based TF-IDF (c-TF-IDF), 
and the interpretation of these keywords into meaningful topics was supported by Generative Pretrained Transformers (GPT). 
As a result, the analysis identified **4 dominant user topics** from the user reviews with a topic coherence score of **0.23428**. 

## Outcome summary
  ![image](https://github.com/user-attachments/assets/afeae662-8375-455e-973c-30af07f3be3c)
The topic-level sentiment analysis revealed that Topics 1 and 3 (Login & Access Issues and Account Registration & Verification) 
were dominated by negative sentiment, at 96% and 93% respectively. 
This indicates that the majority of users experienced issues related to login access, registration, and account verification.
In contrast, Topics 2 and 4 (Information & Mobile JKN Services and Service Comfort & Effectiveness) 
tended to show more positive sentiment, at 53% and 54% respectively, 
suggesting that while users appreciated certain aspects of information delivery, comfort, and service effectiveness, there are still areas that require improvement.
  
## Recommendation for Developers
- Improve the registration, verification, and login systems to reduce user problem and enhance access reliability.
- Enhance the user interface (UI) to ensure that information is effectively communicated and users experience greater comfort and satisfaction during app usage.
  
## Technologies used
`Python` `Transformers (HuggingFace)` `google-play-scraper` `scikit-learn` `pandas` `numpy` `matplotlib` `seaborn`
