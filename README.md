This repository contains the implementation for CSE 676: Deep Learning. The task focuses on sentiment analysis of the Amazon Product Reviews dataset, where product reviews are labeled by sentiment (positive/negative).

The workflow includes:

Data Exploration & Preprocessing

Baseline LSTM Model

Improved Model with Enhancements

Performance Comparison & Discussion

Dataset Setup

Unpack the dataset:

# If .gz format
gunzip train.ft.txt.gz
gunzip test.ft.txt.gz

# If .zip format
unzip amazon_reviews.zip -d data/


After extraction, you should have the following files:

data/
├── train.ft.txt
└── test.ft.txt

