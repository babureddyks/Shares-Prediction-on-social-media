# Shares Prediction on social media
Our main goal is to predict the popularity of news or articles through the given variables using different algorithms.

Information gathering has become an integral part of assessing people’s behaviors and actions. The Internet is used as an online learning site for sharing and exchanging ideas. People can actively give their reviews and recommendations for variety of products and services using popular social sites and personal blogs. Social networking sites, including Twitter, Facebook, and Google+, are examples of the sites used to share opinion. The stock market (SM) is an essential area of the economy and plays a significant role in trade and industry development. Predicting SM movements is a well-known and area of interest to researchers. Social networking perfectly reflects the public’s views of current affairs. Financial news stories are thought to have an impact on the return of stock trend prices and many data mining techniques are used address fluctuations in the SM.

   Machine learning can provide a more accurate and robust approach to handle SM-related predictions. We sought to identify how movements in a company’s stock prices correlate with the expressed opinions (sentiments) of the public about that company. We designed and implemented a stock price prediction accuracy tool considering public sentiment apart from other parameters. The proposed algorithm considers public sentiment, opinions, news and historical stock prices to forecast future stock prices. Our experiments were performed using machine-learning and deep-learning methods including Support Vector Machine, MNB classifier, linear regression, Naïve Bayes and Long Short-Term Memory. Our results validate the success of the proposed methodology.

Using Machine Learning techniques to determine the popularity of online news.  

We've tried to implement and improvise upon the techniques implemented in this paper - <http://cs229.stanford.edu/proj2015/328_report.pdf>. The dataset we use is the `UCI's Online News Popularity dataset` - <https://archive.ics.uci.edu/ml/datasets/Online+News+Popularity>  

For dimensionality reduction, `Fischer Scores` were used as doing so yielded better results than `PCA`.  

The ML algos used are:  
1. Linear Regression  
2. Logistic Regression  
3. Naive Bayes classifier  
4. MLP/Neural Nets  
5. SVM  
6. Random Forest  
7. REPTree  

Some of them are library implementations - `scikit-learn`, while some are coded from scratch.  

And then we used the `TFIDF` approach followed by the above ML algos.  

- Most of the code in the root dir can be run with a simple `python filename.py` where the filename indicates the ML algorithm implemented. Some of them can take quite some time to run.  
- The root dir also contains various graphs and plots generated based on the results.  
- `OnlineNewsPopularity.csv` is the dataset.  
- The file `NewOnlineNewsPopularity.arff` is an input for `Algorithmia's` ML algos - <https://algorithmia.com/tags/machine%20learning> which can be run online.  
- The directory `Feature Extractor` contains code to select a subset of the original features based on `Fischer scores`  
- The directory `FetchPost` contains code in Go - this was our first attempt at `scraping full articles` off the `Mashable url's` provided in the dataset.  
- The directory `newfetchpost` contains working code to scrape full articles using `python goose` - takes quite some time. It also contains `counter.py` which implements various ML algos as pipelines on the extracted full articles using the `TFIDF` approach - again, this takes time as the TFIDF approach inherently implies usage of a rich feature set.  
- `201503003.zip` is the final submission.  


Please go through notebook everything is mentioned in detail.
https://github.com/Babu6030/Project-Shares-Prediction-on-social-media/blob/main/projectmedia1.ipynb
