---
layout: project
title: Recommendation System based on Word2Vec
caption: Recommending retail items based on embeddings learned from Word2Vec
description: >
  Word2Vec was used to learn representations for every item in the dataset.
date: '2021-02-24'
image: 
  path: /assets/img/projects/word2vec-recsys-sequence.png
  # srcset: 
  #   1920w: /assets/img/projects/qwtel.jpg
  #   960w:  /assets/img/projects/qwtel@0,5x.jpg
  #   480w:  /assets/img/projects/qwtel@0,25x.jpg
links:
  - title: Link
    url: https://github.com/kev94yo/word2vec-recsys
# accent_color: '#4fb1ba'
# accent_image:
#   background: '#193747'
# theme_color: '#193747'
sitemap: true
---

This personal project was part of a research on recommendation systems that use Natural Language Processing (NLP)
methods. This was basically a follow through of this [article](https://medium.com/analytics-vidhya/building-a-recommendation-system-using-word2vec-a-unique-tutorial-with-case-study-in-python-f02357fd2486) on medium, organized into jupyter notebook.

## Motivation
1. Apply NLP methods to recommendation systems
2. Use Word2Vec to learn vector representations for items
  - Apply distributional hypothesis of words/sentences to items/purchase sequences.
  - Based on result, recommend similar items.

<p align="center">
  <img src="../../assets/img/projects/word2vec-recsys-model-architecture.jpg" alt="model" width="500">
</p>
Word2Vec model architecture.
{:.figure}

## Project Outline
- **Data Preprocessing**
  - Load online retail data with pandas, remove null values and convert all types to strings.
  - Create sequence of purchases for each customer based on customer ID, and sort by time.
- **Exploratory Data Analysis (EDA)**
  - Get an overall look of the data, and check the number of unique customers.
- **Model Training, Evaluation**
  - Split dataset into 90% train and 10% test.
  - Train using Word2Vec model in `gensim` library, to get representations for each item.
  - Visualize to see if vector representations are well generated.
- **Prediction**
  - Produce recommendations based on items with similar vector representations.
- **Presentation**: Held a talk session about the project.

<p align="center">
  <img src="../../assets/img/projects/word2vec-recsys-cluster.jpg" alt="cluster" width="600">
</p>
Visualization of final vector representations for all items.
{:.figure}

## Result
- Produced sound predictions for items.
- Found a case for utilizing NLP methods for recommendation systems.

## Languages & Tools
Here are the languages, libraries and tools used for this project.
- Python, Matplotlib, Pandas, Numpy, Gensim
- Jupyter Notebook
- Git

## Links
*  **Github**: <a href="https://github.com/kev94yo/word2vec-recsys" target="_blank">https://github.com/kev94yo/word2vec-recsys</a>