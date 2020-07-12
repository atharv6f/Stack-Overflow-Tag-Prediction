# Stack Overflow: Tag Prediction


#  Business Problem
##  Description

Description

Stack Overflow is the largest, most trusted online community for developers to learn, share their programming knowledge, and build their careers.

Stack Overflow is something which every programmer use one way or another. Each month, over 50 million developers come to Stack Overflow to learn, share their knowledge, and build their careers. It features questions and answers on a wide range of topics in computer programming. The website serves as a platform for users to ask and answer questions, and, through membership and active participation, to vote questions and answers up or down and edit questions and answers in a fashion similar to a wiki or Digg. As of April 2014 Stack Overflow has over 4,000,000 registered users, and it exceeded 10,000,000 questions in late August 2015. Based on the type of tags assigned to questions, the top eight most discussed topics on the site are: Java, JavaScript, C#, PHP, Android, jQuery, Python and HTML.

Problem Statemtent
Suggest the tags based on the content that was there in the question posted on Stackoverflow.

Source: https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/
##  Source / useful links

#### 1.Data Source : https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data ####
#### 2.Youtube : https://youtu.be/nNDqbUhtIRg ####
#### 3.Research paper : https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tagging-1.pdf ####
#### 4.Research paper : https://dl.acm.org/citation.cfm?id=2660970&dl=ACM&coll=DL ####


##  Dataset

Refer: https://www.kaggle.com/c/facebook-recruiting-iii-keyword-extraction/data

### Performance metric

Micro-Averaged F1-Score (Mean F Score) : The F1 score can be interpreted as a weighted average of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. The formula for the F1 score is:

F1 = 2 * (precision * recall) / (precision + recall)

In the multi-class and multi-label case, this is the weighted average of the F1 score of each class.

'Micro f1 score':
Calculate metrics globally by counting the total true positives, false negatives and false positives. This is a better metric when we have class imbalance.

'Macro f1 score':
Calculate metrics for each label, and find their unweighted mean. This does not take label imbalance into account.

https://www.kaggle.com/wiki/MeanFScore
http://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html

Hamming loss : The Hamming loss is the fraction of labels that are incorrectly predicted.
https://www.kaggle.com/wiki/HammingLoss


# Machine Learning Models
1. Logistic Regression
2. Linear SVM
##  Converting tags for multilabel problems
A subset of tags is sample instead of using the entire dataset due to limited computing power.

# Conclusion
Using Logistic Regrssion was the obvious choice because of the high dimension of the data. Using RandomForest(XgBoost)wouldn't have made sense due to high dimensonality.



