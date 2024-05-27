# Spam-Email-Classification

Involved developing a spam/ham email classification using the Naive Bayes classifier in a Jupyter Notebook environment, focusing particularly on the extraction and vectorization of text data to be used for training a machine learning model.

STEPS:
1.Data Vectorisation:

I started by importing the necessary libraries and reading two separate datasets (goodware_r.csv and malware_r.csv), which contain examples of 'goodware' and 'malware' respectively.The text data from these files was processed to remove certain characters like commas and quotation marks that could interfere with text vectorization. Using CountVectorizer from the sklearn library, I vectorized the text data while removing stop words (commonly used words in a language that are generally ignored in data processing) and limiting the vectorization to the top 1000 features based on term frequency.

2.Naive Byes Model Training:

After vectorization, the document Malware Matrix was converted into a pandas DataFrame. Each row in this DataFrame corresponds to a document, with columns representing the frequency of each term after vectorization.I then split the dataset into training (70%) and testing (30%) sets.I applied a Multinomial Naive Bayes classifier to the training data. This type of classifier is suitable for classification with discrete features (e.g., word counts for text classification).

3.Model Evaluation:

After training the model, I evaluated its performance on both the training and the test datasets. I calculated the classification accuracy, produced a classification report detailing precision, recall, and F1-score for each class, and generated confusion matrices to understand the true vs. predicted classifications.
The results indicated reasonable performance with a slight difference in accuracy between training and testing, suggesting how well the model generalized on unseen data.

4.Output:
Finally, the outputs, including the classification reports and confusion matrices, were printed out.
Entire work is available through the link  : https://drive.google.com/file/d/1wTkQzvl2eiOUXexSPXDA5K5JRLbXRqhD/view?usp=sharing


