# twitter-sentiment-analysis

## In this project,I have created a simple Twitter Sentiment Analysis supervised learning model using python and NLP libraries.

## Major Steps followed during the project:

### 1.Data Gathering: 

Dataset has been downloaded from kaggle. The dataset consist of 31962 rows and 3 columns. In this dataset, the label column has two values 0 and 1 in which 0 indicates that particular sentiment is positive and 1 indicate that particular sentiment is negative.

### 2.Data PreProcessing:

In this, first of all I have checked for the missing values in the dataset if any. In this, dataset there are no missing values.
Also, done exploratory data analysis to analyze the data with the help of seaborn library which is used for data visualization.

Now, the most important part is to convert the given sentences into numerical values. First of all, I have removed all the punctuation mark from every sentence followed by converting each sentence into lowercase and then convert the sentence into a list of words. Then, checking whether a particular word in a sentence is a stopword or not, if not then converting that particular word into its dictionary form using lemmatization. After this, applying countvectorizer to every sentence and at last transforming it into a numpy array.

Now, our dataset is ready for applying to any machine learning algorithm.

### 3.Model Training:

In this first of all, I have divided the dataset into train and test using the train_test_split method of sklearn library.

For, training my model I have used naive bayes classifier which basically works on probability. It gives an accuracy of 94.90 %. Also, find the value of true positive, true negative, false positive and false negative with the help of confusion matrix.

Since, only accuracy doesn’t tells that how good our model is. So, we have to calculate other performance metrics such as precision, recall, support. These performance metrics can be calculated with the help of classification report.
A classification report is used to measure the quality of predictions from a classification algorithm.
