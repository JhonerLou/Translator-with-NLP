# Translator-with-NLP

English to Spanish Translator with a Transformer Model
This project implements a sequence-to-sequence (Seq2Seq) Transformer model to translate text from English to Spanish. The model is built from scratch using TensorFlow and Keras.

Project Overview
The goal of this project is to create a neural machine translation system. The notebook covers all the steps required, including:

Downloading and preparing the dataset.

Vectorizing the English (source) and Spanish (target) text.

Building a Transformer model with Encoder, Decoder, and Positional Embedding layers.

Training the model on the prepared data.

Evaluating the translation performance using the BLEU score.

Dataset
The model is trained on a dataset of English-Spanish sentence pairs.

Source: The data is from www.manythings.org/anki.

Preprocessing: The text is cleaned, standardized to lowercase, and tokenized. Special [start] and [end] tokens are added to the target Spanish sentences to aid the decoding process.

Model Architecture
The core of this project is the Transformer model, which consists of:

Positional Embedding Layer: To encode word order information.

Transformer Encoder: Processes the input English sequence. It uses Multi-Head Attention and a feed-forward network.

Transformer Decoder: Generates the output Spanish sequence by paying attention to both the encoder's output and its own previously generated tokens.

The entire model is an end-to-end network that takes English and Spanish sequences as input and outputs the probability distribution for the next token in the translated sequence.

How to Use
Clone the repository:

Bash

git clone https://github.com/JhonerLou/Translator-with-NLP.git
cd Translator-with-NLP
Install dependencies: Ensure you have Python and the required libraries installed.

Bash

pip install tensorflow numpy matplotlib nltk
Run the Jupyter Notebook: Launch Jupyter Notebook and open the Salinan transformers-language-translator-eng-to-spanish-task.ipynb file.

Bash

jupyter notebook "Salinan transformers-language-translator-eng-to-spanish-task.ipynb"
Execute the cells in order to download the data, build the model, train it, and test its translation capabilities.
