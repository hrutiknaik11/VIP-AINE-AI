# README for Analysis of Email Phishing Attacks Using Deep Neural Networks

## Overview

This project aims to analyze email phishing attacks using Deep Neural Networks. 
We provide a Google Colab notebook containing the code for this analysis. 
In this README, we'll guide you on how to run the Colab notebook and provide steps to download the dataset.

## Requirements
pandas==1.3.3 <br>
scikit-learn==0.24.2 <br>
numpy==1.21.4 <br>
keras==2.6.0 <br>
nlpaug==1.1.4 <br>
matplotlib==3.4.3 <br>
tensorflow==2.6.0 <br>

## Getting Started

To run the project, you will need access to Google Colab and the dataset. Here's how you can get started:

1. Download the Dataset

	1.1 Download all the enron.tar files on your local machine
		You can use the following link to access the dataset: http://nlp.cs.aueb.gr/software_and_datasets/Enron-Spam/index.html
		We have used the .tar files of Enron-Spam in pre-processed form. There are total 6 .tar files. <br>
	1.2  Open the following .ipynb file on google colab <br>
		Link: https://colab.research.google.com/drive/1Vt71pnfdT977fJWKiXc4ChpJW8GWeOLc?usp=sharing
	1.3 Upload the 6 enron.tar files to google colab. <br>
	1.4 Run each cell one after the other on colab and you will receive a email_dataset.csv file <br>
	1.5 Make sure to download this dataset to your local machine. <br>

	OR

	1.1 You can download the already unzipped, and merged dataset from our drive link:
		Link: https://drive.google.com/file/d/1BXxLuwul-oxK2A0ujezi-KhEPGbwgv-L/view

	a. Dataset Description  <br>
		We have used the Enron Spam Dataset for our project which consists of around 30K data points on which training takes place.

3. Spam Detection Google Colab <br>
	2.1 Go to Google Colab and sign in to your Google account if you're not already logged in. <br>
	2.2 Open the following .ipynb file on google colab  <br>
		Link: https://colab.research.google.com/drive/1t3nhLppJ-1VsrjFRUYiv7SjSjzUo8YBd#scrollTo=cJm0O8NngHck <br>
	2.3 Once you have opened the notebook uplaod your downloaded email_dataset.csv to the notebook <br>
	2.4 Now that you have the dataset in your Colab workspace, you can run the notebook. Here's how to do it: <br>
		Run all the cells by clicking "Runtime" in the top menu and selecting "Run All." <br>

4. Monitor the Execution  <br>
The notebook will start running the code. You can monitor the execution in real-time and observe the results.

5. Interact with the Results  <br>
Once the code execution is complete, you can interact with the results, review visualizations, and explore the analysis.

## Limitations

1. Potential Limitations of the Dataset <br>
Limited Diversity in Email Content: The dataset might not encompass the full spectrum of phishing emails, such as those with different linguistic styles, formatting, or emerging phishing techniques. This could lead to models being less effective against novel or less common phishing attempts.
Time-Bound Data: If the dataset primarily consists of emails from a specific period, it may not capture the evolving nature of phishing attacks, rendering the model less adaptive to newer threats.
Size and Depth of Dataset: The depth (detailed features of each email) and the size of the dataset could limit the model's ability to learn complex patterns effectively, potentially impacting its generalization capabilities.
2. Biases in the Dataset  <br>
Sampling Bias: If the dataset is sourced from a particular email provider or user demographic, it might not represent the wide variety of phishing attacks targeting different groups.
Label Bias: The accuracy of the labels (phishing or not phishing) is crucial. If the labeling process was flawed or biased (e.g., some benign emails wrongly labeled as phishing), the models would learn from incorrect examples, leading to poorer performance in real-world scenarios.
Preprocessing and Augmentation Effects: The preprocessing steps (like removing punctuation, numbers, hyperlinks) and text augmentation could inadvertently filter out or alter critical features of phishing emails, leading to a potential bias in how the models interpret and learn from the data.
3. Impact of Limitations and Biases on Analysis Results  <br>
Model Performance and Reliability: The limitations and biases mentioned can lead to a decrease in model performance, especially in real-world scenarios where phishing attacks may not align perfectly with the dataset's characteristics.
False Positives/Negatives: Biases in the dataset could lead to higher false positives or negatives. For instance, if the dataset lacks variety, the model might fail to identify phishing emails that deviate from the dataset's norm.
Generalization and Adaptability: The model's ability to generalize and adapt to new, unseen phishing threats might be compromised due to the dataset's limitations. This could result in a need for frequent retraining or updates to maintain efficacy
