# Jigsaw-NLP

## Overview
This is a repo dedicated to the [Jigsaw Unintended Bias in Toxicity Classification Kaggle competition](https://www.kaggle.com/c/jigsaw-unintended-bias-in-toxicity-classification/). This is the second competition the Conversation AI team, founded by Jigsaw and Google, have released and it was held in 2018. The goal of this competition is to build a model that recognizes toxicity and minimizes unintended bias with respect to mentions of identities. The motivation for such a task is the following: models usually predict a high likelihood of toxicity for comments containing frequently attacked identities (e.g. "gay"), even when those comments are not actually toxic (such as "I am a gay woman"). This happens because training data is pulled from available sources where unfortunately, certain identities are overwhelmingly referred to in offensive ways.

The model consists of Bi-directional LSTMs with pre-trained embeddings and it has score of 0.96 AUC on the validation set (15% hold-out data = 270732 comments). The embeddings used are 300 dimensional vectors from GloVe and fastText.


## Files

**main.ipynb**: Jupyter notebook with the main code

**utils.py**: Helper script

