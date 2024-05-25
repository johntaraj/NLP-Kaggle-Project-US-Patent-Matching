# NLP Kaggle Project US Patent Phrase to Phrase Matching

![image](https://github.com/johntaraj/NLP-Kaggle-Project-US-Patent-Matching/assets/134852121/b794b676-1e56-4f82-8d0e-f3317aeb8cf9)

Link: https://www.kaggle.com/competitions/us-patent-phrase-to-phrase-matching/data

This project involves building a model to predict the semantic similarity of phrases in the context of US patents. The goal is to help improve the efficiency and accuracy of patent analysis.

## Project Overview

The project uses a dataset from Kaggle's US Patent Phrase to Phrase Matching competition. It involves the following key steps:

1. **Data Loading and Exploration**: Loading the dataset and performing exploratory data analysis (EDA) to understand its structure and basic statistics.
2. **Data Preparation**: Preprocessing the data by tokenizing and numericalizing the text data using a pretrained transformer model tokenizer.
3. **Model Training**: Training a sequence classification model to predict the similarity scores between phrases.
4. **Evaluation and Prediction**: Evaluating the model's performance and making predictions on the test set.
5. **Submission**: Preparing the submission file for the Kaggle competition.

## Code Explanation

### Data Loading and Exploration

- Import necessary libraries (`numpy`, `pandas`, `os`, `pathlib`).
- Load the dataset from the Kaggle competition and print the file paths.
- Read the training data using `pandas` and display the basic statistics and structure.

### Data Preparation

- Combine relevant columns into a single input column for the model.
- Tokenize the text data and convert tokens into numerical IDs using the tokenizer from the pretrained `microsoft/deberta-v3-small` model.
- Split the dataset into training and validation sets.

### Model Training

- Define training arguments such as batch size, number of epochs, learning rate, and evaluation strategy.
- Create a correlation function to measure the model's performance.
- Initialize the model and the trainer.
- Train the model on the training dataset and evaluate it on the validation dataset.


## Usage

To use this code, follow these steps:

1. Ensure you have the required libraries installed (e.g., `pandas`, `numpy`, `transformers`, `datasets`).
2. Insert your own Kaggle API credentials.
3. Run the script to load the data, train the model, and generate predictions.
4. Submit the generated `submission.csv` file to the Kaggle competition.

### Note

Replace `"your_username"` and `"your_key"` with your Kaggle API credentials. This script will download the data, preprocess it, train the model, and create a submission file.
