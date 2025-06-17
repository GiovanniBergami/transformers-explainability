
# transformers-explainability
A multi-method explainability framework for transformer-based text classification models.

## Table of Contents
* [General Info](#general-info)
* [Some results](#some-results)
* [Models](#models)
* [Datasets](#datasets)
* [Explanability Methods](#explainability-methods)
* [Technologies](#technologies)
* [Setup](#setup)
* [Authors](#authors)
* [Appendix](#appendix)


## General info
This project is about explaining the choices made by text-classificators.
It includes a complete pipeline:

- Downloading datasets from Huggingface (sentiment classification on movie reviews and outcome and NORP classification from legal text datasets)
- Cleaning and preparing the datasets
- Fine-Tuning BERT and RoBERTa on the tasks
- Applying the XAI methods to the classifications
- Comparing the explanation with the human annotated ground truth and against already existing explanaiblity methods (SHAP,LIME) and rationales (part of the text annotated as relevant for the sake of the classification)
- Producing visual plots of the explanations

Different methods to explain the choices of the model are implemented.
More on that on the paper: (TODO add paper link)

## Some results

## Models
The models used are BERT and RoBERTa:

- [BERT](https://huggingface.co/docs/transformers/model_doc/bert)
- [RoBERTa](https://huggingface.co/docs/transformers/model_doc/roberta)

## Datasets
The datasets are:

- [sentiment1](https://www.kaggle.com/datasets/madhavkumarchoudhary/sentiment-prediction-on-movie-reviews): a movie-reviews sentiment prediction dataset (positive/negative)
- [sentiment2](https://www.kaggle.com/datasets/thedevastator/unlocking-the-human-perspective-on-movie-reviews): a movie-reviews sentiment prediction dataset (positive/negative) with rationales (human-annotated parts of the review that are regarded as relevant for the sake of the classification)
- [asylex](https://huggingface.co/datasets/clairebarale/AsyLex/tree/main): a legal text dataset that contains:
    - legal court decision about:asylum requests: from this, the **asylex-outcome** dataset has been created. It is binary classification (accepted/rejected)
    - The annotated Nationality/Ethnicity/religion of the requester: from this,the **asylex-norp** dataset has been created. It is a multi label classification between different features of the requester

## Explainability Methods

Already existing methods:

- [SHAP](https://shap.readthedocs.io/en/latest/)
- [LIME](https://github.com/marcotcr/lime)

New methods:

- Persistent Homology (Angular Distance) and other Persistent Homology based methods
- Thresholded Cosine Similarity Masking and other Cosine Similarity based methods


## Technologies

This project runs using: mettere tutte le librerie?

## Setup

You can clone the repo as it is, and then run the different .jpynb in the following order:

- dataset_creator, to create the desired datasets.
- train_and_test, to train the classification model
- XAI, to use the different XAI methods and plot the heatmaps.

#### Example:
Given a dataset, a model and a XAI method, you should run:

```
prova
```
inside the main function.

## Authors

- [@GiovanniBergami](https://www.github.com/GiovanniBergami)

## Appendix



