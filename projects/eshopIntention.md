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

The importance of data analysis in companies has become crucial to improve sales and understand customers, to this has been added the power to have statistical information on our websites and with them improve the customer experience. In this project, I have analyzed through these data about the online purchase intention of people.

## Project Description

From a dataset that consists of statistical characteristics of about 12,000 sessions on online sales websites, I carried out an analysis of the purchase intention that a person could have in a virtual way and how we could predict the behavior of users. This [dataset](https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset) was created and hosted in the UCI Machine Learning Repository.

### Data exploration
I start the data exploration reading the dataset, then I looked for missing values. Finally I took related bounce rates of customers.

{% gist e28d7a082e0a5378020f436875f18ac1 %}

### Machine Learning algorithms

Next I used K-elbow method to determine clusters

{% gist 316b60e786bfca76aeb9bd0ed23d6e36 %}

The number of optimal clustering groups for the duration of the product and the bounce rates is 2 as you can see in the next graph:

<img class="img-fluid" width="450" height="350" src="../img/eshopIntention/elbow.png">

I applied the K Means method to find the clusters

{% gist 439351a25042f723a64cd308f0903f9a %}

<img class="img-fluid" src="../img/eshopIntention/cluster.png">

Next I got predicted clustering result label and plotted the normalized and non-normalized confusion matrix for predictions

{% gist 144a1cc017d55705e2ecdcb1c33a625d %}

<img class="img-fluid" width="450" height="350" src="../img/eshopIntention/confusion.png">

<img class="img-fluid" width="450" height="350" src="../img/eshopIntention/confusion_n.png">

### Final analysis

From the confusion matrix, we can see that out of 10,422 failed incomes, 9,769 are grouped into uninterested customers or 94%. However, out of 937 successful incomes, only 284 are grouped as target customers or 15%. Also, the adjusted index score is not very high.

So it is clear that I have poorly bundled many successful revenue sessions as uninterested customers, which means when the high bounce rate combined with a short product-related page duration, there are still a lot of customers. 

Thanks for reading! 😄
