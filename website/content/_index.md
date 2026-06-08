---
title: "Respiratory Open Access Research (ROAR)"
description: "Guidelines and tools for fair evaluation of automatic respiratory event detection algorithms"
---

## The need for automatic respiratory event detection tools

Chronic cough and cough hypersensitivity disorders are globally prevalent conditions that significantly impair patients’ quality of life. These conditions are difficult to treat due to the difficulty in identifying causes, including individual triggers and underlying pulmonary disorders. Current clinical practice assesses severity and treatment efficacy through patient questionnaires, which are only moderately correlated to actual cough counts. Hence, there is significant interest in using smart wearable devices to automatically
provide objective daily cough counts as a more accurate, unbiased means of assessment. 

## The problems

While efforts are being made to develop wearables to automatically detect and quantify cough events, such monitoring devices have not yet been incorporated into routine clinical practice due to lack of consistency in their validation resulting in slow progress and lack of trust on reported results. There are three main reasons for this heterogeneity: 
1) The clinical definition of different cough events lacks standardization.
2) The data used is typically private or unlabeled.
3) Methodologies to assess the accuracy of event detection are different between research groups and often inappropriate.

## ROAR mission statement

The goal of the ROAR is to contribute Open Research Data (ORD), community guidelines, and standards to propose a unified framework for validating cough event detection algorithms. The main objective is the development of standards to unify the workflow for the validation of respiratory events detection algorithms to make data adhere to the principles of Findable, Accessible, Interpretable, and Reusable (FAIR) data. This website serves as a central hub and reference for standardizing clinical definitions and methodologies, setting best-practice standards for reasearch and industry teams developing tools for automatic cough detection. Furthermore, we contribute the first publicly accessible cough counting dataset, including real-world noise scenarios, multimodal biosignal recordings, and fine-grained cough event labels following our best practice guidelines.

## Website structure

- [Cough event definition]({{< ref "/definition" >}}): 
    - Information about the physiological mechanism behind cough, which informs our data labeling, annotation, and evaluation standards
- [Open data for cough counting]({{< ref "/dataset" >}}): 
    - Description of an open dataset for cough detection, including its content and structure. 
- [Data labeling, annotation, and validatio framework]({{< ref "/framework" >}}): 
    - Description of an open dataset for cough detection, including its content and structure. 
- [Tools]({{< ref "/tools" >}}):
    - Tools for implementing the ROAR methodology for cough event detection

## Credits

If you use the ROAR methodology in one of your scientific studies, please make sure to credit one of the following works.

Open dataset: 
1. [Orlandic L, Thevenot J, Teijeiro T, Atienza D. “A Multimodal Dataset for Automatic Edge-AI Cough Detection”. *IEEE /nternational Engineering in Medicine and Biology Conference (EMBC).* 2023.](https://ieeexplore.ieee.org/abstract/document/10340413)

ROAR annotation and evaluation methodology:

2. [Orlandic L, Dan J, Thevenot J, Teijeiro T, Sauty A, Atienza D. How to count coughs: an event-based framework for evaluating automatic cough detection algorithm performance”. *IEEE International Conference on Body Sensor Networks (BSN)*.2024](https://ieeexplore.ieee.org/abstract/document/10780617)

An example of ROAR used to develop a cough detection algorithm: 

3. [Albini S, Orlandic L, Dan J, Thevenot J, Teijeiro T, Atienza D. “Cough-E: A multimodal, privacy-preserving cough detection algorithm for the edge”. *IEEE Journal of Biomedical Health Informatics (JBHI)*. 2025.](https://ieeexplore.ieee.org/abstract/document/11027535)
