# Malaria Cell Image Classification

### Neural network image classifier to detect malaria infected red blood cells

<img src="https://www.news-medical.net/image.axd?picture=2020%2f2%2f%40shutterstock_1521138356.jpg&ts=20200219064042&ri=674" width="100%"/>

## Motivation

There are a lot of images in the medical field that can benefit from image classifiers and object detection. I would love to contribute in any way I can to the medical field because it is essential and beneficial to everyone. Moreover, I wanted to learn how to perform an image classification end-to-end project using TensorFlow2 to gain more experience in TensorFlow.

## Dataset Description

Malaria is a mosquito-borne infectious disease that affects humans and other animals. The symptoms  range from tiredness, vomitting, and headacches to siezures, comas, and even death. Like any disease, being able to detect if a patient is infected is desireable. The Malaria dataset is a repository of segmented cells from the thin blood smear slide images from the Malaria Screener research activity. The Giemsa-stained thin blood smear slides from 150 P. falciparum-infected and 50 healthy patients were collected and photographed at Chittagong Medical College Hospital, Bangladesh.

[https://ceb.nlm.nih.gov/malaria-datasets](Malaria Dataset Source)

## Summary Results

A batch of 32 cell images can be seen below. The images display red blood cells that are both infected and not infected.

<img src="https://imgur.com/takpjDc.jpg" width="100%"/>

The training and validation curves of selected plots are shown below.

<img src="https://imgur.com/bH4dUHm.jpg" width="100%"/>

When evaluated on the test set, the model seems to perform well.

<p align="center">
  <img src="https://imgur.com/asczJHF.jpg" width="30%"/>
<p align="center">
  
An AUC score of 1 indicates a perfect classifier while 0.5 indicates a truly random classifier, so a ROC AUC score of 98.6% is excellent. It's important to note that accuracy it not necessarily a good metric to score classifiers. We have 97.3% chance to identify all relevant instances indicated by recall and a 94.3% chance for the model to return only relevant instances indicated by precision.
