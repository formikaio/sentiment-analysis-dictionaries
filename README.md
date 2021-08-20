# Sentiment analysis root dictionaries

[![Buy us a tree](https://img.shields.io/badge/Treeware-%F0%9F%8C%B3-lightgreen)](https://plant.treeware.earth/formikaio/sentiment-analysis-dictionaries)

My [TvSeriesTweet](http://www.whiletrue.it/tvseriestweet/) app collects popular tweets from the best Tv Series. I’ve recently added a Sentiment Analysis tab, to provide info about how the Tv Series communication on Twitter is polarized (positive, negative or neutral content) and what type of content best suits the followers. Unlike other analysts, I like to study the communication of the Twitter influencers instead of the sentiments of the users reacting to them.

After having studied and tried the best current approaches to Sentiment analysis (syntactic-semantic grammar rules, heuristic methods, combined methods), I decided to develop a different solution to better address the Twitter user content.

Twitter users tend to use a lot of hashtags and aggregated words, so a classic dictionary based algorithm wouldn’t correctly recognize a lot of words. I created a new dictionary, using only the root of every word (e.g. the root “alert” for the words: alerts, alerting, alerted) and used it to look for the roots inside every word of a given tweet (so that the root gets recognized within the #spoileralert hashtag).

The roots dictionary is derived from the AFINN-111 file. It’s a text file, every row contains the root of a word, and a positive or negative score (in the range -5/+5) separated by comma.

The English and Italian dictionaries are provided.

More info here: http://www.whiletrue.it/sentiment-analysis-approach/

## Licence 🌳           

This package is [Treeware](https://treeware.earth). If you use it in production, then we ask that you [**buy the world a tree**](https://plant.treeware.earth/formikaio/sentiment-analysis-dictionaries). And why wouldn't you? By contributing to the Treeware forest you’ll be creating employment for local families and restoring wildlife habitats.
