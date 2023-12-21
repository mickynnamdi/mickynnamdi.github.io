---
title: "Design and Validation of a Classification Model for Parkinson’s Disease"
collection: projects
permalink: /projects/2022-Design-and-Validation-of-a-Classification-Model-for-Parkinson’s-Disease
excerpt: '<img src="/images/parki.png" alt="Logo" width="100" height="150" /> Project for Statistical Machine Learning (ECE-6254)'
categories:
  - Deep Learning
---

## Summary

Parkinson’s Disease is one of the most common movement disorders, largely affecting older populations, with progressively developing symptoms caused by a slow breakdown of cells in the nervous system. Symptoms include hand tremors, gait impairment, and slurred speech to name a few. In this report, we will describe a method for training a machine learning model to predict the likelihood of a subject being a Parkinson’s Disease (PD) patient based on a subject’s gait and demographic data. A machine learned approach to detecting Parkinson’s could assist doctors with early detection and possible mitigation of disease progression. Three different approaches were attempted: 1. Random Forest (RF) regression to achieve feature selection for training, coupled with Support Vector Classification with the reduced feature-selected dataset, 2. Convolutional Neural Network (CNN) with the entire dataset, and 3. Logistic Regression with the entire dataset. The dataset used to accomplish this is the open-source Physionet gait dataset, which includes 3 test instantiations of PD and control patients. Each patient has 8 sensors placed on the bottom of each foot, where force data may be obtained during a 2 minute walking period, hence the gait data. This data also includes demographic data of each subject, such as age, gender, walking speed, and the assessed Timed Up And Go score. The feature selection method turned out to leave out useful information for assessing PD likelihood, and therefore did not produce great results. The CNN provided a high precision of 99% for assessing high likelihood of PD in known PD patients, but a low precision of 49% for assessing that the likelihood for a control subject was low and thus performed poorly on identifying that the person does not have PD. The final assessment was that the Logistic Regression approach provided the highest accuracy when performed on test data at 87% accurate. Accuracy here is determined as correctly predicting a PD patient based on ground truth of diagnosis and/or correctly predicting that a person from the control group does not have PD.

## Dataset

[Parkinson's Progression Markers Initiative (PPMI)](https://link.springer.com/article/10.1007/s10072-018-3522-z)

## Approach 
Random Forest, SVM, Logistic Regression, Convolutional Neural Network

## Result

<img src="/images/rf.png" alt="Normal"/> 

## Report
[Design and Validation of a Classification Model for Parkinson’s Disease pdf](/files/ECE%206254%20Final%20Report.pdf)
