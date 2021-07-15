#  Project: Build a Model with Google AutoML

## Table of Contents 

- [Overview](#overview)
- [The Data](#data)
- [The Four Parts of the Project](#parts)
- [Project Structure](#structure)
- [Notes](#notes)
- [References](#references)

## Overview  <a name="overview"/>

In the [previous project](https://github.com/ErkanHatipoglu/AI-Product-Manager-Nanodegree-Program/tree/main/1-%20Create%20a%20Medical%20Image%20Annotation%20Job), We have created the instructions needed to build a labeled dataset that distinguishes between healthy and pneumonia x-ray images and filled the project proposal document. 

This dataset would later be used to build a product that helps doctors quickly identify cases of **pneumonia in children**. The goals of this product are to:

- Help flag serious cases,
- Quickly identify healthy cases,
- And, generally, act as a diagnostic aid for doctors.

In this project, we are going to take the next step and build the classification model that would serve as the backbone of this product. For this task, we will use [Google AutoML](https://cloud.google.com/automl/). To see how the training data impact the models, we will build models with 4 variants of the dataset.

## The Data  <a name="data"/>

We'll be using the same Kaggle [Chest x-ray dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) that we used in the [previous project](https://github.com/ErkanHatipoglu/AI-Product-Manager-Nanodegree-Program/tree/main/1-%20Create%20a%20Medical%20Image%20Annotation%20Job). We will use the original labels supplied with the data on [Kaggle](https://www.kaggle.com).

## The Four Parts of the Project <a name="parts"/>

We will train four different models using four variants of the [pneumonia dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia). Recall that the dataset contains childrens' chest x-ray images, and that they are classified into two classes, "normal" and "pneumonia". The following sections describe the steps we must take to create each model.

### Create a binary classifier to detect pneumonia using chest x-rays

We'll start by training a model simply using 100 images from the **'normal'** class and 100 images from the **'pneumoni'** class. We will evaluate the following:

- Train/test split: How much data is used for training and how much is used for testing?
- Confusion matrix: What do each of the cells in the confusion matrix describe?
- Precision & recall: What do these measure and how are they calculated?

### Create an unbalanced binary classifier
Next, we will use 100 images from the **'normal'** class, and add 200 more **'pneumonia'** class images. At this moment, the total count of images must be:

- **'normal'** class = 100
- **'pneumonia'** class = 300

## Project Structure <a name="structure"/>

- *Build_a_model_project_files* directory is the root directory. 
- *images* folder is for example images, 
- *data* folder is for data,
- *automl-modeling-report.docx* is the report document filled by me.

## Notes <a name="notes"/>
- Most of the parts of this README are directly copied from the Udacity project instructions.

## References <a name="references"/>

- [AI Product Manager Program - Udacity](https://www.udacity.com/course/ai-product-manager-nanodegree--nd088)
- [Create a Medical Image Annotation Job](https://github.com/ErkanHatipoglu/AI-Product-Manager-Nanodegree-Program/tree/main/1-%20Create%20a%20Medical%20Image%20Annotation%20Job)
- [Kaggle](https://www.kaggle.com)
- [Chest x-ray dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)