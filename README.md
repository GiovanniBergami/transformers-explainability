
# transformers-explainability
A multi-method explainability framework for transformer-based text classification models.

## Table of Contents
* [General Info](#general-info)
* [Examples and Results](#examples-and-results)
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
- Comparing the explanation with the human annotated ground truth and against already existing explanaiblity methods (SHAP,LIME)
- Producing visual plots of the explanations

Different methods to explain the choices of the model are implemented.
More on that on the paper: (TODO add paper link)

## Examples and Results

## Models
The models used are BERT and RoBERTa:

- link
- link

## Datasets
The datasets are:

- sentiment1: 
- sentiment2:
- asylex:

## Explainability Methods

Already existing methods:

- SHAP
- LIME

New methods:

- Persistent Homology (Angular Distance) and other Persistent Homology based methods
- Thresholded Cosine Similarity Masking and other Cosine Similarity based methods


## Technologies

This project runs using:

## Setup

```
$ cd ../lorem
$ npm install
$ npm start
```

## Authors

- [@octokatherine](https://www.github.com/octokatherine)

## Appendix

Any additional information goes here

