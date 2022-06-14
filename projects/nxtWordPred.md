---
layout: project
type: project
image: img/nextWordPred/nxtWordPrediction-square.png
title: "Next Word Prediction"
# All dates must be YYYY-MM-DD format!
date: 2022
published: true
labels:
  - Natural Process Language
  - Deep Learning
  - Recurrent Neural Network
summary: "Next word prediction using NLP and LSTM neural networks."
---

I developed this project as part of the need to learn more about the NPL. This is the result of my self-study through Keras documentation, Data Science forums, and educational content on web.

Particularly, use of neural networks to analyze text draws my attention, since it opens up a world of possibilities for the analysis of data that can be found, for example, in social networks, forums, newspapers, etc. That's why I decided to venture a little into text processing with neural networks through this project. Personally, this work helped me to become more interested and involved in Deep Learning applications to solve problems with text data.

## Project Description

Through use of natural language processing and deep learning methods, I made a model that is capable of predicting the next word of a particular sentence. From the reading of the text from the book [Metamorphosis](https://www.gutenberg.org/cache/epub/5200/pg5200.txt) by Franz Kafka found in Project Gutenberg, the construction of a deep neural network was used with recurrent neural networks (LSTM).

### Data preprocessing
I start the data preprocessing taking the original text and removing extra and unnecessary information for training, saving it in a new file. Then I read the text using utf8 encoding.

{% gist 66707443fcd44b17b01cfc125d920f0a %}

I add each text lines in a list and join the lines of text removing related elements of unnecessary lines of text

{% gist 0e14342bf7a667d95a7cb6bb00134d5c %}

And I make sure I don't have repeated words

{% gist eab2fcf51f70603ad14ed6520f4fe66c %}
 
Source: <a href="https://github.com/theVacay/vacay">theVacay/vacay</a>
