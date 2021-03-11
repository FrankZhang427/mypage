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

This project aims to perform a classification task on the modified figures based on the MNIST dataset. Each figure contains two digits and an operator indicated by the first letter of the operation, i.e. ‘A’ or ‘a’ for addition and ‘M’ or ‘m’ for multiplication. Our task is to build a model that correctly predicts the result of the mathematical operation on each input figure. For this purpose, we have implemented a baseline logistic regression classifier, two fully connected feedforward neural networks and a convolutional neural network (CNN). Other techniques have also been attempted to boost the performance including cost-sensitive learning and data augmentation.