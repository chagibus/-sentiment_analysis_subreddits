### Project 3 Title: *Sentiment prediction of subreddit posts*
### Created by **Devaraja Mudeppa**


**The folder contains the following data files** 

1. Two files on data scarping code from two different subreddits -- r/UnpopularOpnion (**scrape_unpopular_subr.ipynb**) and r/College (**scrape_college_subr.ipynb**)

2. **EDA_coll_opin_pool.ipynb** is a code file EDA on pooled two subreddit posts 

3. **lemmatization_pooled_college_opin.ipynb** is a code file on removal chars and stopwords, tokenization, and lemmatization of posts
   
4. The files **logreg_coll_opin.ipynb, randforrest_coll_opin.ipynb, SVM_coll_opin.ipynb, and BernoulliNB_coll_opin.ipynb, multinomialNB_coll_opin.ipynb** is on training and testing of LogisticRgression, Random Forest, and SVM and Bernoulli and multinomial Naive Bayes ML models. Each of these files also has a code for predictions on college posts.

5. Project_3 slide deck

**The data subfolder has the following files**

6. The Scrapped data as  .csv file from r/College as **college.csv** and r/UnpopularOpinion as **unpopularopnion.csv**.

7. Sentiment_scored data files of college as **college_senti_zeroed.csv** and unpopularopinion as **opins_senti_oned.csv**

8. Combined sentiment scored college and unpopularopinion as **combined_posts.csv**

9. Lemmatized text file as **combined_posts.csv**

10. Lemmatized college posts as **coll_lemmatized_posts.csv**



### Executive summary

###### Natural language processing (NLP) models are powerful tools for finding the emotion behind social media posts. In this project, my company, asked me to find out if it is  possible accurately detect the sentiment behind social media posts. The NLPs and predictive machine learning models are employed to find the emotion behind the Reddit posts. The College and Unpopularopinion subreddits corpus were scrapped and cleaned for text analysis.  The binary sentiment score (1 and 0) was assigned as the target variable to the corpora to calculate the accuracy of predictions. The corpora were pooled, and emojis, unwanted characters, and stop-words were removed. With the help of tokenization, each sentence in each post was split into words. The parts of speech in the sentences were tagged, then lemmatizing each word from each post. This cleaning process helped reduce the total words from 590194 to 285079 in the pooled 3581 posts—four machine learning models trained and tested predictive powers on the pooled corpus. Multinomial Naïve Bayes (MNB) predicted with the highest accuracy and precision of 98.6 % and 100% recall/sensitivity.  What it means is that the trained MNB ML model correctly classified 100% of predictions (matched with true labels). Only 1.4% of predictions were incorrectly classified.  Of the 1670 predictions, only 23 were incorrectly classified (false negatives). By manually looking at a few posts from these incorrect predictions, it was found that slang,  irony, sarcasm, and expressions of emotions from different cultural backgrounds contributed to the false negatives.  I am confident that by sensitizing the model to slang, sarcasm, and phrases from various cultural backgrounds, the incorrect predictions can be reduced to zero. The more the model we train with vocab from different parts of the world, the better the model gets at prediction. 


```python

```
