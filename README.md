# BloodMNIST Classification

## Project Overview

This project explores multiclass classification of blood-cell microscopy images from the BloodMNIST dataset. The goal is to assess, optimise and compare various classical machine learning (ML) and deep learning approaches, to understand their strengths and limitations for image classification.

## Personal Motivation

As part of a broader effort to drive my transition from bioinformatics toward applying ML to biological data, I aim to apply my learnings from the book "Hands-On Machine Learning with Scikit-Learn and TensorFlow" by Geron Aurelien and the Coursera/DeepLearning.AI Specializations on "Deep Learning" by Andrew Ng and "Mathematics for ML and Data Science" by Luis Serrano. 

With a background in biomedical science and bioinformatics (and biobusiness), I am not entirely unfamiliar with the data science in biology. My work primarily revolved around genomic and transcriptomic sequencing, and some image analysis in a spatial omics context. 

But this will be my first dedicated ML project and a genuine foray into the field of artificial intelligence (AI), where I expect to tread unknown waters on my own and (hopefully) find my footing as a new 'AI initiate'. Through this exercise, I should develop a more fundamental understanding of ML by implementing and comparing different model families on a biomedical image classification problem. 

## Dataset

BloodMNIST is part of the MedMNIST collection and contains 28 × 28 RGB images from eight blood-cell classes. The dataset consists of a total of 17,092 samples, of which 11,959 (70%) belong to the training set, 1,712 (10%) belong to the validation set and 3,421 (20%) belong to the test set.

## Planned Analysis

- Exploratory data analysis
- Linear models
- Support vector machines (SVMs)
- Decision trees and random forests
- Ensemble methods
- Dimensionality reduction
- Multilayer perceptrons (MLPs)
- Convolutional neural networks (CNNs)

## Strategy 

1. Train models on training data using default model parameters (baseline models)
2. Evaluate each model's performance on the validation data
3. Perform 10-fold cross-validation of baseline models on training set
4. Evaluate each model's performance on each fold of the training data
5. Compare baseline model performances and eliminate clearly unsuitable models
6. Fine-tune promising model families using CV hyperparameter search methods on the training data
7. Evaluate each model's performance on the validation data (since they have been fine-tuned on the training data)
8. Compare fine-tuned model performances and choose the best model
9. Re-train the chosen model using the fine-tuned hyperparameters on the combined training and validation set
10. Final evaluation of the re-trained, chosen model on the test data

## Model Evaluation Metrics
1. Accuracy
2. Precision
3. Recall
4. F1 Score