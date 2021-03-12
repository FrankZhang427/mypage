---
title: "Classification on Modified MNIST Digits"
description: "Project for applied machine learning course"
code: "ModifiedMNIST"
tags: ["Machine Learning", "CNN", "python", "tensorflow", "keras"]
weight: 3
report: true
draft: false
---

## Abstract

This project aims to perform a classification task on the modified figures based on the MNIST dataset. Each figure contains two digits and an operator indicated by the first letter of the operation, i.e. ‘A’ or ‘a’ for addition and ‘M’ or ‘m’ for multiplication. Our task is to build a model that correctly predicts the result of the mathematical operation on each input figure. For this purpose, we have implemented a baseline logistic regression classifier, two fully connected feedforward neural networks and a convolutional neural network (CNN). Other techniques have also been attempted to boost the performance including cost-sensitive learning and data augmentation. [Here is the link for Kaggle competition page](https://www.kaggle.com/c/comp551-modified-mnist). Our team, called "Definitely need a Titan X", has achieved the first place on the leaderboard with 98.8% accuracy.


## Data

Here are some samples of training data. The data is stored in pixel value of 0 - 255. The labels of training data are the numerical results of addition or multiplication.

![Sample inputs](/pic/modified_mnist/train/train_1.png)
![Sample inputs](/pic/modified_mnist/train/train_2.png)
![Sample inputs](/pic/modified_mnist/train/train_3.png)
![Sample inputs](/pic/modified_mnist/train/train_4.png)
![Sample inputs](/pic/modified_mnist/train/train_5.png)
![Sample inputs](/pic/modified_mnist/train/train_6.png)
![Sample inputs](/pic/modified_mnist/train/train_7.png)
![Sample inputs](/pic/modified_mnist/train/train_8.png)
![Sample inputs](/pic/modified_mnist/train/train_9.png)
![Sample inputs](/pic/modified_mnist/train/train_10.png)
