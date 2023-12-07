**Resume Screening/Filtering**

This Python script is designed to predict the categories of resumes using machine learning techniques. It involves several steps, including data exploration, text preprocessing, feature extraction, and model training. Below is an overview of the code functionality, usage, and key components.

 
**Table of Contents**
1.	Introduction


3.	Dependencies


4.	Usage

5.	Code Overview
 
		•  	Data Exploration

        •	Text Processing

        •	Data Visualization 

        •	Word Cloud	

        •	Label Encoding	

        •	Feature Extraction 

        •	Model Training	


5.	Results


6.	Conclusions


**Introduction**


The script utilizes a dataset containing resumes and their corresponding categories. It employs a Multinomial Naive Bayes classifier and One-vs-Rest strategy for multilabel classification. The accuracy of the model is evaluated on both the training and test sets.


**Dependencies**


•	NumPy


•	Pandas


•	Matplotlib


•	Seaborn


•	Scikit-learn


•	NLTK


•	WordCloud


Install the required dependencies using the following command:


		•	pip install numpy pandas matplotlib seaborn scikit-learn nltk wordcloud


**Usage**


1.	Ensure you have the required dependencies installed.


2.	Download the resume_dataset.csv file and place it in the same directory as the script.


3.	Run the script


**Code Overview**


Data Exploration


•	Loading the dataset and displaying the unique categories and their distribution.


Text Preprocessing


•	Cleaning the resumes by removing URLs, mentions, hashtags, punctuations, and extra whitespaces.


Data Visualization


•	Visualizing the distribution of resume categories using bar plots.
Word Cloud


•	Generating a word cloud to visualize the most common words in the cleaned resumes.
Label Encoding


•	Converting categorical labels (categories) into numerical format using Label Encoding.
Feature Extraction


•	Using TF-IDF (Term Frequency-Inverse Document Frequency) to convert the cleaned resumes into numerical features.
Model Training


•	Splitting the data into training and testing sets.


•	Training a KNeighbors Classifier using the One-vs-Rest strategy.


•	Evaluating the accuracy of the model on both training and test sets.


**Results**


The accuracy of the KNeighbors Classifier on the training and test sets is displayed, along with a classification report showing precision, recall, and F1-score for each category.


**Conclusion**


This script demonstrates a pipeline for text-based category prediction using machine learning. Feel free to modify the parameters, try different classifiers, or experiment with additional preprocessing techniques to further enhance the model's performance.


