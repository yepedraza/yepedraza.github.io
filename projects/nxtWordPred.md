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

And make sure I don't have repeated words

{% gist eab2fcf51f70603ad14ed6520f4fe66c %}

### Tokenization
I use Tokenizer to vectorize the text and then transform it into a sequence of numbers

{% gist e66c897bf4500338dcc175a109120d48 %}

Then I find the size of the *word index* to later use it as a criterion to convert the output data into categorical variables and next I create the input and output data of the model with the text sequences before the creation of data sequences

{% gist 46192b0bcf326e836715b6b5e9728a2a %}

Finally I convert the output data to categorical variables

{% gist 180b84bd2e30e1055053f4bdc89f1ab6 %}

### Model Creation
The model architecture is the following:
  * Input Embedding layer
  * Two LSTM layers
  * A fully connected layer and,
  * An output layer

The model has 15,7M training parameters aprox and you can download it [here](https://drive.google.com/file/d/1hPjFniCR8w5yUMrN1-oRjmRPusC7yJfD/view?usp=sharing)
Finally, I obtained a model with 57% accuracy in prediction and with a categorical error of 0.6163. You can see detaily the codes and documentation in this [Repo](https://github.com/yepedraza/nextword-predict). For the prediction of the model I created a [notebook](https://github.com/yepedraza/nextword-predict/blob/80307bdc413d959ab60544853bc9f9044ca28872/predScript.ipynb) that has the following characteristics:
  * Model and tokenizer file uploading
  * Use tokenizer for the input sentences for which we should make the predictions on
  * Make predictions on the input sentence by using the saved model

