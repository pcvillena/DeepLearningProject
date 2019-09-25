# CoE 197-Z Deep Learning Project
### [IEEE-CIS Fraud Detection](https://www.kaggle.com/c/ieee-fraud-detection/overview)
##### Can you detect fraud from customer transactions?

Datasets can be found [here](https://drive.google.com/open?id=1JWhnL8gI-imOe4KV9CY6TsKASStvj8G4).

## I. Overview
Imagine standing at the check-out counter at the grocery store with a long line behind you and the cashier not-so-quietly announces that your card has been declined. In this moment, you probably aren’t thinking about the data science that determined your fate.

Embarrassed, and certain you have the funds to cover everything needed for an epic nacho party for 50 of your closest friends, you try your card again. Same result. As you step aside and allow the cashier to tend to the next customer, you receive a text message from your bank. “Press 1 if you really tried to spend $500 on cheddar cheese.”

While perhaps cumbersome (and often embarrassing) in the moment, this fraud prevention system is actually saving consumers millions of dollars per year. Researchers from the [IEEE Computational Intelligence Society](https://cis.ieee.org/) (IEEE-CIS) want to improve this figure, while also improving the customer experience. With higher accuracy fraud detection, you can get on with your chips without the hassle.

IEEE-CIS works across a variety of AI and machine learning areas, including deep neural networks, fuzzy systems, evolutionary computation, and swarm intelligence. Today they’re partnering with the world’s leading payment service company, [Vesta Corporation](https://trustvesta.com/), seeking the best solutions for fraud prevention industry, and now you are invited to join the challenge.

In this competition, you’ll benchmark machine learning models on a challenging large-scale dataset. The data comes from Vesta's real-world e-commerce transactions and contains a wide range of features from device type to product features. You also have the opportunity to create new features to improve your results.

If successful, you’ll improve the efficacy of fraudulent transaction alerts for millions of people around the world, helping hundreds of thousands of businesses reduce their fraud loss and increase their revenue. And of course, you will save party people just like you the hassle of false positives.

## II. Data Description 
In this competition you are predicting the probability that an online transaction is fraudulent, as denoted by the binary target `isFraud`.

The data is broken into two files `identity` and `transaction`, which are joined by `TransactionID`. Not all transactions have corresponding identity information.

### Categorical Features - Transaction
- `ProductCD`
- `card1 - card6`
- `addr1, addr2`
- `P_emaildomain`
- `R_emaildomain`
- `M1 - M9`

### Categorical Features - Identity
- `DeviceType`
- `DeviceInfo`
- `id_12 - id_38`

### Files
- **train_{transaction, identity}.csv** - the training set
- **test_{transaction, identity}.csv** - the test set (you must predict the isFraud value for these observations)
- **sample_submission.csv** - a sample submission file in the correct format
