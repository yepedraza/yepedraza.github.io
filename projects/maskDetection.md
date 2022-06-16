---
layout: project
type: project
image: img/faceMask/face_mask_square.png
title: "Mask detection"
# All dates must be YYYY-MM-DD format!
date: 2022
published: true
labels:
  - Image Classification
  - Convolutional Neural Networks
  - Computer Vision
summary: "Face mask detection using CNN"
---
With the advances that neural networks have had lately and specifically convolutional neural networks, and the situation that the planet has been presenting; I have realized the importance of the field of computer vision to apply it to the specific detection of "something". In this case, that something is the mask, a vital element today, that detection could be very useful from now on.

## Project Description
Through the use of convolutional neural networks, I made a model that it's capable of detecting by reading an image if a person is wearing a face mask or not. The database I'm using contains about 6400 images of people. Each of these images also has a JSON type file that indicates many of its characteristics, being "class_name" the one that indicates the types of accessories that the people in the image are wearing (where we're going to classify if they're wearing a mask or not). The objective of this project is to apply CNN for a possible tool that uses computer vision and artificial intelligence to prevent infections in closed spaces.

{% gist 9defa1fb3f4eb593ba5fa9eacedca960 %}
 
Source: <a href="https://github.com/theVacay/vacay">theVacay/vacay</a>
