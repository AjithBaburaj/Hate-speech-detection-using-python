# Hate-speech-detection-in-Social-Media-using-python


## Description of the project

In this project, I begin by addressing the issue of freedom of speech on the Internet and the misuse of social media platforms like Twitter. These challenges serve as my primary motivation.
To achieve my goals, I utilize a publicly available dataset from CrowdFlower and apply natural language processing (NLP) techniques. I outline the workflow, starting with dataset analysis and followed by text preprocessing to create a cleaner dataset. This cleaned dataset is then used for feature engineering.
I extract unique and significant features, organizing them into different sets for comparison. I analyze the performance of various machine learning classification algorithms concerning each feature set.
Finally, I delve into a detailed analysis of the results obtained, explaining the reasons behind misclassifications in my model.

## Results Obtained:

The logistic regression algorithm works consistently well with all feature sets except for F7 as precision, recall and subsequently the f1-score for “hate” label results in zero which is shown in Fig-23. Random Forest classifier works pretty well when it comes to F1 and also shows a significant performance in all other feature sets but its performance is hugely impacted when tf-idf scores are not included in the feature set as shown in Fig-24. The overall performance of the Naïve Bayes classifier is found to be less significant for the purpose of classifying tweets into hate, offensive or neither labels but it performs significantly better with feature set of F7 compared to other feature sets which is shown in Fig-25. SVM classifier also seems to be consistent throughout all feature sets except for F4 and F7 as shown in Fig26. From the above graphs we analyse that the most important feature was found to be F1 i.e. the tf-idf scores which helps in better classification of hate speech. The sentiment scores also prove to be an important feature for the differing of hate speech and offensive language .Doc2vec columns are not found to be very significant in classification purpose as it makes very less difference when it’s removed from the feature set. On comparing all the graphs above Random Forest is clearly the winner

## Summary of the project

I began by collecting data to create my hate speech dataset, which posed a challenge because what one person considers hate speech may be seen as normal text by someone else. To clean the dataset, I applied text preprocessing techniques, which included removing punctuation, tokenizing, eliminating stopwords, stemming, and getting rid of URLs and mention names.
The processed text was then used for feature extraction. I extracted various features, such as n-gram TF-IDF weights, sentiment polarity scores, Doc2Vec vector columns, and readability scores. These features were combined in different sets to be used with various classification models.
I evaluated these classification models based on accuracy and F1-scores, using different feature sets. The results clearly demonstrate the difficulty of distinguishing between hate speech and offensive language. They also highlight the advantages of utilizing the proposed features and serve as a valuable resource for addressing toxic language issues on Twitter. A more detailed analysis of these features and errors could lead to more robust feature extraction methods and help overcome the existing challenges in this field.
