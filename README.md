# CMSC-516-SetimentAnalysis

# Text mining frequently employs the technique of sentiment analysis. By analyzing the sentiment of the text (in this case, a tweet), using sophisticated text mining techniques, it is possible to determine if it is positive, negative, or neutral.

#Installation Instructions
 1)Install Python on you Computer.
 2)Download Anaconda Navigator.
 3)Launch jupyter Notebook from Anaconda Navigator.
 4)Upload the "Twitter sentiment analysis working 76% using TfidfVectorizer-final nlp-tf-idf (1).ipynb" in your Anaconda Navigator.
 5)Run the ipynb file on your Jupyter Notebook.
 
#Data
1)The sentiment140 dataset is shown here. 1,600,000 tweets that were extracted using the twitter api are included. The annotated tweets (0 = negative, 4 = good) can be used to detect sentiment.
2)These are the features in the dataset.
  target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)
  ids: The id of the tweet ( 2087)
  date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)
  flag: The query (lyx). If there is no query, then this value is NO_QUERY.
  user: the user that tweeted (robotickilldozr)
  text: the text of the tweet (Lyx is cool)
  ![image](https://user-images.githubusercontent.com/46966138/196498725-8ded1e3c-42cb-40c5-9d07-e74de1b4ce19.png)


 
#Method
1)Imported all the libraries like pandas, tensorflow, sklearn and nltk
2)Loaded the Dataset using pandas
3)We are mainly intrested in the target label, text, so we visualize and see the data.
4)We cleaned the data by removing stopwords,punctuations,repeating characters, url and numbers
5)Then we tokenize the tweet text.
6)We split the dataset into 70% train and 30% test. and use the "target" label for testing.
7)We used TfidfVectorizer model for feature selection with a max feature limt.
8)There were a total features of 6100.
9)Then we used classifiers like naive bayes, Decision Tree, multiLayer Perceptron.

#Results
1)![image](https://user-images.githubusercontent.com/46966138/196499082-f354d6ea-fbe7-4170-9d96-feb095796fbd.png)

 
