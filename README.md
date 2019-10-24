# Spam-Detection-using-NLP-ML-models
_This jupyter notebook has a ML classification model to detected a mail as spam or not._
_Our goal is to build a predictive model which will determine whether a text message is spam or ham. For the code, see here._

## Introduction

In recent times, unwanted commercial bulk emails called spam has become a huge problem on the internet. The person sending the spam messages is referred to as the spammer. Such a person gathers email addresses from different websites, chatrooms, and viruses. Spam prevents the user from making full and good use of time, storage capacity and network bandwidth. The huge volume of spam mails flowing through the computer networks have destructive effects on the memory space of email servers, communication bandwidth, CPU power and user time. The menace of spam email is on the increase on yearly basis and is responsible for over 77% of the whole global email traffic. Users who receive spam emails that they did not request find it very irritating. It is also resulted to untold financial loss to many users who have fallen victim of internet scams and other fraudulent practices.

## 1. Inspecting the dataset

Taking a data which is categorized in to ham or spam with the text in data.
 ### a. Importing the required modules/packages
 ### b. Loading file and looking into the dimensions of data
 
 ## 2. Text preprocessing
 
There are many feature engineering strategies for transforming text data into features. Some involve assigning each unique word-like term to a feature and counting the number of occurrences per training example. However, if we were to perform this strategy right now, we'd end up with an absurd number of features, a result of the myriad possible terms. The classifier would take too long to train and likely overfit. As a result, each NLP problem requires a tailored approach to determine which terms are relevant and meaningful.

## 3. Vectorizing the Text

In the first part of this series, we explored the most basic type of word vectorizer, the Bag of Words Model, which will not work very well for our Spam or Ham classifier due to its simplicity.

Instead, we will use the TF-IDF vectorizer (Term Frequency — Inverse Document Frequency), a similar embedding technique which takes into account the importance of each term to document.

While most vectorizers have their unique advantages, it is not always clear which one to use. In our case, the TF-IDF vectorizer was chosen for its simplicity and efficiency in vectorizing documents such as text messages.

TF-IDF vectorizes documents by calculating a TF-IDF statistic between the document and each term in the vocabulary. The document vector is constructed by using each statistic as an element in the vector.
