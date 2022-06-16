---
layout: project
type: project
image: img/eshopIntention/eshopIntention.png
title: "E-Shop Intention"
# All dates must be YYYY-MM-DD format!
date: 2022
published: true
labels:
  - Machine Learning
  - K-means Clustering
  - K-Elbow method
summary: "Online shopping intention analysis with Machine Learning."
---



## Project Description

Through use of natural language processing and deep learning methods, I made a model that is capable of predicting the next word of a particular sentence. From the reading of the text from the book [Metamorphosis](https://www.gutenberg.org/cache/epub/5200/pg5200.txt) by Franz Kafka found in Project Gutenberg, the construction of a deep neural network was used with recurrent neural networks (LSTM).

### Data exploration
I start the data preprocessing taking the original text and removing extra and unnecessary information for training, saving it in a new file. Then I read the text using utf8 encoding.

{% gist 66707443fcd44b17b01cfc125d920f0a %}

I add each text lines in a list and join the lines of text removing related elements of unnecessary lines of text

{% gist 0e14342bf7a667d95a7cb6bb00134d5c %}

And make sure I don't have repeated words

{% gist eab2fcf51f70603ad14ed6520f4fe66c %}

### Machine Learning algorithms
