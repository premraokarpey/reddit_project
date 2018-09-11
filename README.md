Executive Summary-

In this project we look at reddit.com. Arguably one of the most popular discussion websites online, reddit has a huge population of users. In reddit, each topic is discussed in a particular 'Subreddit'. Our goal for this project is to collect data from the website from 2 subreddits. Once we do this, we are require to model the data and predict which post would go in which subreddit. 

This data collection was very fascinating because it was such a wide range. I wanted my subreddits to be a little different to see how the model I came up with performed on the Data when the words used or topics discussed from ranged from basketball to the stock market. This is why I used r/nba and r/wallstreetbets.

To retrieve the data I came up with a function that would convert the Url to JSON form and scrape from the website. The functionality included the use of the 'after' function to successfully retrieve more than 25 posts at a time. Using a for loop, I was able to retrieve as many posts I wanted, including the use of a time function so as to not overload reddit servers. 

Once I had the data, I converted them to dataframes and combined them. I then use the subreddit column as my reference and converted the titles to 0's and 1's. 

Once I reached this stage, I could utilise Natural Language Processing, and more specially the CountVectorizer and Tf-Idf Functinos to help fit the data. After doing this, using Logisitc Regression we can score the models and also retrieve the keywords that were used to predict which subreddit a particular post would fall in. The words with the most skew were mu,stock,tesla for wallstreetbets and nba,lebron,game for nba. 

We then implemented other regression techniques on the data such as ForestRegressor and DecisionTrees. We scored these models as well and formed our analysis. 

My best scoring model was through Locigal Regression implementing Tf-Idf. In a dataset that is so textheavy, Tf-Idf helped to indentify unique words that were used the most, other than the stopwords to help distinguish between subreddits. This process is extremely helpful and with the right parameter tweaking can be extremely effective.

Some potential uses for these models are to predict efficiency of particular subreddits compared to the workflow of reddit. We can also use parameters to identify keywords to use to maximise the probabilty of making a successful reddit post. 

