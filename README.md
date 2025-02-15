# Machine learning-based Cricket Comments Sentiment Analysis in English.

**Problem Statement**

The primary aim of this project is to develop and evaluate various machine learning models for sentiment analysis of textual data. By leveraging algorithms such as Logistic Regression, Decision Trees, Random Forest, Support Vector Machines (SVM), and Naive Bayes, the objective is to classify texts based on their sentiment (positive, negative, neutral). The performance of these models will be compared using metrics such as accuracy, precision, recall, F1 score, and AUC-ROC to determine the most effective model for sentiment classification.  


**Dataset**

We gathered data from online facebook comment box during India vs Australia final cricket match which are witten in English alphabet from social media platforms.  Currently our dataset has around 50062 comments, with two content types review_text and lable. Our dataset distributed in Positive, Negative and Neutal.

![dataset](https://github.com/user-attachments/assets/f32e1d5a-1bf9-40c6-a307-f71d71882466)


**Sample of dataset**

![ggg](https://github.com/user-attachments/assets/58ec30bc-eafe-486b-8718-db6951b57768)


**Approach**

We implement machine learning approaches for classifying the cricket comments according to their positive,negative and neutral sentiment. The raw contents contain special characters, e.g., @, #, - Etc., punctuations. At the time of preprocessing, we have to remove these special characters and punctuation. Multi sentimantal comments in English. For example ‘wishing india best’ represent  in positive comment,‘drop prediction powerplay score’ represent  in negative comment, ‘omg wicket’ represent  in neutral comment in English. There is some common words. We also have to remove those common words from the dataset. This can be done by preprocessed the comments. Then we have to extract the features from the comments. Using those extracted features we can train the machine learning models. 


 ![model](https://github.com/user-attachments/assets/185abe7a-e8e4-4da6-a2a4-42bda5b36d7a)



**For classifying the cricket comments we used the following steps:**

Step 1: Collect the various cricket comments from social media in English alphabet. We collect those comments from India vs Australia world cup diring final match.

Step 2: Removed special characters, punctuation, stop words, and frequent terms from the content. For collecting the actual feature from the comments, we removed the special characters, punctuation, stop words, and frequent terms from the content. 

Step 3: We utilized tokenizer to tokenize the data after deleting superfluous components. In this step we use tokenization to separate the individual words from comments.

Step 4: We now have a list of terms and the frequency with which they appeared in each piece of cricket comments. The feature was then extracted from the material using tf-idf. Full form of if-idf is Term Frequency Inverse Document Frequency. 

Step 5: We then divided the dataset into 70% for training and 30% for testing. 

Step 6: We then trained a variety of machine learning models to categorize the contents. 
*Machine Leaning Models used:*
•	Logistic Regression
•	Decision Tree
•	Random Forest
•	Multinomial Naive Bayes
•	K-Nearest Neighbor
•	Linear Support Vector Machine
•	RBF Support Vector Machine

Step 7: We used a test dataset to assess the machine learning models. We plot confusion matrix for each model. Then we calculate precision, recall, accuracy, F1-score for each model. We evaluated our machine learning approaches using different test contents from our created dataset. In this case, machine learning models performed well for the Random Forest. 

Step 8: Using the evaluated findings, we selected the best machine learning model. The Random Forest model outperformed the other machine learning models for Unigram features. Using the classifier model, we examined a variety of comments written in English. We achieved 86% accuracy using the Random Forest with Unigram feature.


![vvvvvvv](https://github.com/user-attachments/assets/ed85b4df-e13c-4e5a-ad49-2cc447ec73eb)



Step 9: We then used the Logistic Regression model to forecast the unlabeled content.

**Input Content:**

1. bowling towards hip region rohit huge red flag
2. hazelwood getting smacked brohit rohit revenge mode
3. bowl short brohit punter


**Output Content:**

![positive](https://github.com/user-attachments/assets/6dcb43fb-497d-4ebe-adcf-65dba37148f7)
![negative](https://github.com/user-attachments/assets/ec749991-a358-4e9e-99ca-7903c5121aca)
![neutral](https://github.com/user-attachments/assets/5e30e0c7-c737-44d4-ae2a-f02f06346475)

**Conclusion**
This project has been conducted to offer an approach for classifying multi sentimental coments writing in the English alphabet. With the experiment's findings, we could classify the original positive,negative and neutral comments English alphabets. With all of the conclusions of this experiment, it is possible to infer that the approach is an efficient and accurate method for classifying the cricket sentimental comments in English alphabets during cricket match. 

