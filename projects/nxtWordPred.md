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

I developed this project as part of the need to learn more about the NPL. This is the result of my self-study through Keras documentation, Data Science forums, and educational content on the web.

Particularly, use of neural networks to analyze text draws my attention, since it opens up a world of possibilities for the analysis of data that can be found, for example, in social networks, forums, newspapers, etc. That's why I decided to venture a little into text processing with neural networks through this project. Personally, this work helped me to become more interested and involved in Deep Learning applications to solve problems with text data.

## Project Description

Through the use of natural language processing and deep learning methods, I made a model that is capable of predicting the next word of a particular sentence. From the reading of the text from the book [Metamorphosis](https://www.gutenberg.org/cache/epub/5200/pg5200.txt) by Franz Kafka found in Project Gutenberg, the construction of a deep neural network is used with recurrent neural networks (LSTM).

### Data preprocessing
Empiezo el preprocesamiento de datos tomando el texto original y eliminándole información extra e innecesaria para el entrenamiento, guardándolo en un archivo nuevo. Luego leo el texto usando el utf8 encoding.
{% gist c71de7e84739b0ca1fbdd26fe142c2d0 %}
 
Source: <a href="https://github.com/theVacay/vacay">theVacay/vacay</a>
