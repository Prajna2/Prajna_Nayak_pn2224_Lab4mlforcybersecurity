# Prajna_Nayak_pn2224_Lab4mlforcybersecurity

# Backdoor Attacks Lab4 

## Details
Name: Prajna Ravindra Nayak  
Net ID: pn2224

## Table of Contents
1. [Overview](#overview)
2. [System Requirements](#system-requirements)
3. [Repository Structure](#repository-structure)
4. [Data](#data)
5. [Procedure](#procedure)
6. [Contributions](#contributions)
7. [Acknowledgements](#acknowledgements)

## Overview
This repository contains the code for a cutting-edge neural network backdoor detection system. The main objective of this project is to improve the security of neural networks, specifically those trained on the YouTube Face dataset and potentially compromised by malicious alterations. The project introduces an innovative model called GoodNet, designed to distinguish between legitimate and compromised inputs, classifying them into distinct categories.

## System Requirements
Execution Environment: MacBook Pro equipped with M1 chip
Interface: Google Colab Pro

## Repository Structure
In the "Dataset/" directory, you'll find two files: "valid.h5" for validation and "test.h5" for testing purposes. Additionally, there's a "Models/" directory where you can store the original model, modified models, and the advanced GoodNet model.

## Data
I have used data from the github repository https://github.com/csaw-hackml/CSAW-HackML-2020 for this lab. The data under lab3 folder has been used. The folder 'cl' contains clean test and validation data and the folder 'bd' contains poisoned test and validation data
The dataset contains images from YouTube Aligned Face Dataset. We retrieve 1283 individuals each containing 9 images in the validation dataset.

## Procedure
The primary objective of this project was to improve a machine learning model by employing various techniques, including channel pruning, model selection based on accuracy metrics, assessing potential security vulnerabilities, and creating an optimized hybrid model.

In our approach, we performed channel pruning on the conv_3 layer, guided by the average activation values from the final pooling stage in the validation dataset. We implemented a model-saving strategy at specific accuracy decline thresholds of 2%, 4%, and 10%. This resulted in the creation of models named model_X=2.h5, model_X=4.h5, and model_X=10.h5, reflecting the corresponding accuracy decreases.

A significant aspect of this project involved assessing the model's susceptibility to attacks, with a particular focus on evaluating the success rate of attacks when the accuracy dropped by 30%. Our analysis revealed a notable vulnerability rate of approximately 6.95%.

Our main goal was to merge two versions of the model: the original, potentially compromised model known as "BadNet" and the improved version post-pruning. This effort aimed to establish an advanced and resilient model named "GoodNet."

You can find all the programming code and execution steps documented in the 'pn2224_Prajna_Nayak_ML_LAB4.ipynb' notebook. This comprehensive notebook covers every aspect of the project, including model development, pruning, evaluation, vulnerability analysis, and the fusion of models to create GoodNet.

## Contributions
Feedback and contributions are highly encouraged. For proposing changes or discussing new ideas, please initiate an issue or submit a pull request.

## Acknowledgements
Extend my sincere gratitude to New York University (NYU) for their invaluable support and provision of resources that greatly facilitated the successful execution of this research project.


