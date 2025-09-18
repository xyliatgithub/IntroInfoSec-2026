# Lab Assignment 4 - Adversarial Attacks Against Machine Learning Based Spam Filters
The learning objective of this lab is for students to gain the first-hand experience on the machine learning based spam filters and related adversarial attacks. Coding experience is recommended, so you might want to work with someone with programming backgrounds. 

## Lab Manual
The lab manual is a notebook (ipynb) file. You will find textboxes and code blocks to work on for a set of questions and task. You don't need to write a separate report for this lab. Please include all your answers and code in the lab manual for submission. Please explain clearly your ideas and steps as instructed. Remember to save regularly when you are working on the notebook.

The dataset needed for this lab is in this Git folder called messages.csv. 

## Environment Setup

For this lab, you will need to use google colab, and you need a google account to use it. If you have never used google colab or jupyter notebook before, you can go through this tutorial first: https://colab.research.google.com/github/cs231n/cs231n.github.io/blob/master/python-colab.ipynb.

### Use of Google Colab
Open the link https://colab.research.google.com/notebooks/. Then just upload the notebook file you download from the Canvas. Then you can work on the notebook file directly. 

## Introduction
Machine learning-based spam filters classify emails based on labeled training data. However, adversarial attacks can modify spam emails to evade detection by making small but strategic changes. This lab explores how TF-IDF features are manipulated using the Projected Gradient Descent (PGD) algorithm to identify "magic words," which increase the chances of spam emails bypassing an SVM classifier. Additionally, we extend this attack to large language model-based spam filters, inclluding BERT and GPT-2.

## Lab Overview  

This lab explores adversarial attacks on machine learning models, focusing on both **white-box** and **black-box** attack scenarios. The experiment is structured into two main parts:  

### 1. White-Box Attack on Traditional Machine Learning Models  
- This section employs a **Projected Gradient Descent (PGD) attack** on a **TF-IDF-based spam filter**.  
- By perturbing the model input in the feature space, we identify special **"magic words"** that can alter the classifier’s predictions.  
- These magic words are then inserted into spam emails themselves to evade detection, demonstrating the vulnerability of traditional spam filters to adversarial attacks.
- These words will also be used in the black-box attacks in Part 2. 

### 2. Black-Box Attack on Large Language Models (LLMs)  
- In this section, we extend the attack to **black-box settings**, targeting LLM-based classifiers using **BERT** and **GPT-2**.  
- Without access to model gradients, we apply the previously discovered magic words to spam emails, modifying their structure and placement.  
- By inserting these words or sentences made of them at different positions, we generate **adversarial emails** and evaluate their impact on the LLM classifiers.  

This lab provides insights into **adversarial attack vulnerabilities** in both machine learning and LLM-based spam filters, highlighting potential security risks and countermeasures.  

## Learning Objectives
By completing this lab, you will:
- Understand how SVM-based machine learning spam filters work.
- Learn how TF-IDF is used as an embedding strategy for text classification.
- Implement the PGD attack to find magic words that can fool spam filters.
- Explore the application of magic words you have found to evade BERT- and GPT-2-based spam filters.
- Deploy adversarial attacks against spam filters using magic words.

## Publication References 

(1) Q. Cheng, A. Xu, X. Li, and L. Ding, “Adversarial Email Generation against Spam Detection Models through Feature Perturbation,” The 2022 IEEE International Conference on Assured Autonomy (ICAA’22), Virtual Event, March 22-23, 2022.

(2) C. Wang, D. Zhang, S. Huang, X. Li, and L. Ding, “Crafting Adversarial Email Content against Machine Learning Based Spam Email Detection,” In Proceedings of the 2021 International Symposium on Advanced Security on Software and Systems (ASSS ’21) with AsiaCCS 2021, Virtual Event, Hong Kong, June 7, 2021.

You can download these papers at https://isi.jhu.edu/people/xyli/

## Submission Details

- Each group only needs to submit one report in ipynb format.
- Please list group members in your report explicitly.
- Only typed reports are accepted.

## Grading

- Completeness (30 pts): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
- Presentation (20 pts): The report must be clear and correct in organization and writing with adequate explanation.
