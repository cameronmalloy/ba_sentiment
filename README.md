# Bay Area Twitter Sentiment During a Pandemic

Repository for [the blog post of the same name](https://cameronmalloy.github.io/ba-sentiment.html) This is meant to be a compainion for the blog post for anyone who would like to repeat or create a similar analysis.

## Download the Data
To recreate, first you must download data.
First we can download the Sander's test corpus. In data/sanders, follow the README instructions. Make sure the final csv downloaded is named `final_corpus.csv`. This will take about 10 hours to follow the Twitter API's rate-limits.

Second, we'll download Sentiment140's train and test dataset. When reading these csv's in `LSTM.ipynb`, make sure the names of the files align (maybe Sentiment140 will change the names, we're unsure).

Third deals with GloVe's word embeddings. The notebook handles this with `wget`.

If you would like to use the Bay Area twitter data in the blog, you don't have to download anymore. However, if you would like new data, I have provided 2 notebooks that do it. `data/grab_tweets.ipynb` will gather as many tweets as you want from within the Bay Area. You will have to keyboard interrupt the notebook to stop. It takes about a day to gather almost a million tweets. `data/clean_tweets.ipynb` will only take tweets from user's whose location is a city in the Bay Area.

## Running the Analysis
Once the data is downloaded, you can run everything in `LSTM.ipynb`! It includes everything from the blog.

** All sources can be found in the blog post linked above **
