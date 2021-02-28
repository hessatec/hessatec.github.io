---
layout: post
title: AML and Azure Synapse Project Introduction (Part 1)
author: Siri
tags: ML Synapse Azure
---

2021 has already been an eventful year for a number of reasons. One of those reasons is the market fluctuations that have come about as a result of the Reddit Gamestop saga in which we saw the price of $GME skyrocket in a bid to play hedge funds and the practice of short selling, which bets on the price of a certain stock falling. 

Now Sai and I were recently discussing the many applications of Azure Synapse Analytics and wanted to see if we can apply it to our own lives and build a end-to-end data and AI solution. Because we were both so intrigued by what the implications of the Gamestop saga we wanted to return to the roots of the stock exchange - the S&P 500 index. This index is an aggregate of the 500 highest market cap companies in the stock exchange, and represents the overall "health" and direction of the stock market. 

What does this look like? Our solution uses a dataset of S&P 500 index with nearly a hundred years of S&P data to train an RNN model. This model is then used to score a testing dataset which is loaded into an Azure Synapse Analytics dedicated pool through a pipeline. By doing this, and comparing to other models (such as an ARIMA, linear regression) we hope to evaluate and predict S&P index in the future. 

In the next few blog posts, we will outline the steps we take to complete this exercise. Join us! 
