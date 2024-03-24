# Text Prompt(UNDER PROGRESS)

## Project Overview
This project contains code for training a language model using text data from the gutenberg Project. It preprocesses the text, tokenizes it, and trains a Long Short-Term Memory (LSTM) Recurrent Neural Network (RNN) model using TensorFlow and Keras.

## Folder Structure
- **gutenberg**: This folder contains data for model training.
- **generative-text-model.ipynb**: The notebook file contains code for preprocessing the text data, training the LSTM RNN model, and saving the preprocessed corpus.

## Code Overview
The provided Jupyter Notebook (`generative-text-model.ipynb`) performs the following tasks:
1. **Data Preprocessing**:
   - Imports necessary libraries including NLTK and TensorFlow.
   - Defines a function to preprocess text data, removing stopwords and tokenizing the text.
   - Loads text data from specified files, preprocesses it, and combines it into a single corpus.
   - Saves the preprocessed corpus into a text file named `preprocessed_corpus.txt`.

2. **Model Training**:
   - Imports TensorFlow and Keras modules for building and training the LSTM RNN model.
   - Tokenizes the preprocessed corpus using the Keras Tokenizer.
   - Creates input sequences using a sliding window approach.
   - Pads sequences to have uniform length for all data.
   - Divides data into predictors and labels, and converts labels to one-hot encoding.
   - Builds an LSTM RNN model with embedding layers and a final dense layer.
   - Compiles and trains the model on the predictors and labels with specified epochs.

## Instructions
1. Ensure that the necessary dependencies are installed, including NLTK, TensorFlow, and Keras.
2. Place the text data for training in the `gutenberg` folder.
3. Execute the code in the provided Jupyter Notebook (`generative-text-model.ipynb`).
4. The preprocessed corpus will be saved as `preprocessed_corpus.txt`.
5. The LSTM RNN model will be trained using the preprocessed corpus data.

## Dependencies
- NLTK
- TensorFlow
- Keras
