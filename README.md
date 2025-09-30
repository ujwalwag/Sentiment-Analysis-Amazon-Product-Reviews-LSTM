This repository contains the implementation for CSE 676: Deep Learning. The task focuses on sentiment analysis of the Amazon Product Reviews dataset, where product reviews are labeled by sentiment (positive/negative).

The workflow includes:
Dataset Setup

The dataset files (train.ft.txt.zip and test.ft.txt.zip) are already included in this repository.
You just need to unpack them before running the notebook:

Unzip the dataset files:

unzip train.ft.txt.zip -d data/
unzip test.ft.txt.zip -d data/


After extraction, the structure should look like this:

project_root/
├── a2_part1_ujwalwag.ipynb
├── requirements.txt
├── train.ft.txt.zip
├── test.ft.txt.zip
└── data/
    ├── train.ft.txt
    └── test.ft.txt


Make sure the notebook points to the correct file paths:

train_path = "data/train.ft.txt"
test_path  = "data/test.ft.txt"

Requirements

Install dependencies:

pip install -r requirements.txt


Key libraries:

torch, torchtext, torchinfo

nltk

sklearn

seaborn, matplotlib

wordcloud

Usage

Run the Jupyter Notebook:

jupyter notebook a2_part1_ujwalwag.ipynb

Using GloVe Pre-trained Embeddings

Download GloVe (e.g., 6B tokens, 100 dimensions):

wget http://nlp.stanford.edu/data/glove.6B.zip
unzip glove.6B.zip -d embeddings/


Common options: glove.6B.50d.txt, glove.6B.100d.txt, glove.6B.200d.txt, glove.6B.300d.txt.


Steps inside the notebook:

Load and explore the Amazon Product Reviews dataset.

Preprocess text (tokenization, vocabulary, padding).

Train and evaluate the baseline LSTM model.

Train and evaluate the improved LSTM model.

