---
title: "Tools"
description: "We provide tools to streamline the processing of EEG for the task of automated seizure detection."
---

We provide certain tools to encourage reproducibility and consistency of results reported in the field of automated seizure detection algorithm.

## timescoring

{{< github repo="esl-epfl/timescoring" >}}

We built a library that provides different scoring methodologies to compare a reference time series with binary annotation (ground-truth annotations of the neurologist) to hypothesis binary annotations (provided by a machine learning pipeline). These different scoring methodologies provide a count of correctly identified events (True Positives) as well as missed events (False Negatives) and wrongly marked events (False positions)

In more details, we measure performance on the level of:

- Samples : Performance metric that threats every label sample independently.
- Events (e.g. cough) : Classifies each event in both reference and hypothesis based on overlap of both.

Both methods are illustrated in the following figures :

![Illustration of sample based scoring.](https://user-images.githubusercontent.com/747240/248309097-b7f76fde-c87a-41df-812d-9821375b640e.png)

![Illustration of event based scoring.](https://user-images.githubusercontent.com/747240/248308898-64b4ae39-d02f-4f06-9b10-f07aaf6110d1.png)


## Cough signal manipulation tools

To accompany the cough counting dataset, we developed the following Git repository: https://github.com/esl-epfl/edge-ai-cough-count/

The repository contains code for:
* Easily iterating through the file structures of the dataset
* Data segmentation
* Data augmentation
* Applying the event-based framework to test model predictions

## Cough-E

The Cough-E model is an open-source example of a cough detection model that was trained and evaluated using our cough counting dataset and evaluation framework. The model training code and embedded C implementation can be found here: https://github.com/esl-epfl/Cough-E