# CMSC-516-SetimentAnalysis

Text mining frequently employs the technique of sentiment analysis. By analyzing the sentiment of the text (in this case, a tweet), using sophisticated text mining techniques, it is possible to determine if it is positive, negative, or neutral.

# Installation Instructions <br/>
 1)Install Python on you Computer. <br/>
 2)Download Anaconda Navigator. <br/>
 3)Launch jupyter Notebook from Anaconda Navigator.<br/>
 4)Upload the "Twitter sentiment analysis working 76% using TfidfVectorizer-final nlp-tf-idf (1).ipynb" in your Anaconda Navigator.<br/>
 5)Run the ipynb file on your Jupyter Notebook. <br/>
 
# Data <br/>
1)The sentiment140 dataset is shown here. 1,600,000 tweets that were extracted using the twitter api are included. The annotated tweets (0 = negative, 4 = good) can be used to detect sentiment. <br/>
2)These are the features in the dataset. <br/>
  target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)
  ids: The id of the tweet ( 2087)
  date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)
  flag: The query (lyx). If there is no query, then this value is NO_QUERY.
  user: the user that tweeted (robotickilldozr)
  text: the text of the tweet (Lyx is cool)
  ![image](https://user-images.githubusercontent.com/46966138/196498725-8ded1e3c-42cb-40c5-9d07-e74de1b4ce19.png)


 
# Method <br/>
1)Imported all the libraries like pandas, tensorflow, sklearn and nltk.<br/>
2)Loaded the Dataset using pandas. <br/>
3)We are mainly intrested in the target label, text, so we visualize and see the data. <br/>
4)We cleaned the data by removing stopwords,punctuations,repeating characters, url and numbers.<br/>
5)Then we tokenize the tweet text. <br/>
6)We split the dataset into 70% train and 30% test. and use the "target" label for testing. <br/>
7)We used TfidfVectorizer model for feature selection with a max feature limt. <br/>
8)There were a total features of 6100. <br/>
9)Then we used classifiers like naive bayes, Decision Tree, multiLayer Perceptron. <br/>

# Results <br/>
1)Results using Naive Bayes
 ![image](https://user-images.githubusercontent.com/46966138/196499082-f354d6ea-fbe7-4170-9d96-feb095796fbd.png)
2) Results using Decision Tree
 ![image](https://user-images.githubusercontent.com/46966138/196499770-2ee88b64-75da-46e6-9fc9-73fba454a95b.png)
3) Results using Multi Layer Perceptron
  ![image](https://user-images.githubusercontent.com/46966138/196499888-fc3f8adb-2543-4017-9bb3-3d55ce234ac8.png)
  
# Discussion <br/>
Comparing the results from the three classifiers produced me a results of 
Naïve bayes :- 75.83
Decision Tree:- 70.95
MLP:- 77.15
So, using MLP produced us the best accuracy
![image](https://user-images.githubusercontent.com/46966138/196500511-40e4dd97-8bfd-48e5-9dcb-c7ade3037703.png)


# Future Work <br/>
I want to finish my implementation of Bert and word2vec with the same three classifiers and compare the results.
Try to use implement CNN.
![image](https://user-images.githubusercontent.com/46966138/196500616-83d25ad6-f248-4110-b256-d5b171ffe9a9.png)
