# H&M Personalized Fasion Recommendation
## Introduction

This challenge is about creating an fasion clothing recommendation system. The data contains information about the customers, records of customers’ purchases, and information about the products including their images and text description.


## Research Question

The Aim of this project is to predict the next 12 purchases for each customer based on their past purchases and the product metadata.

## Method

I will be sampling the data into users who have more than 30 pruchases (Active users), and people who have 30 pruchases or less (Cold users). Thhis is becuase some neural networks will be computationally expensive for users who don't have much data. These algorithms use cotent-base filtering which works only if there is a sufficient amout of data.

For Active users I will be using:

GRU: an RNN that uses the structural embedding of the product data.
GRUF: an RNN that uses the visual embedding of the product data.
For Cold users, I will be using:

NPU: an RNN desgned for the cold user problem.
ALS: a matrix factorization technique, which counts as a colaborative filtering model.
Trending products: using the trending products that week. This will be very useful for attracting cold users.

Link to the Competition: https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations
