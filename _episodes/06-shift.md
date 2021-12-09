---
title: "Dataset shift"
teaching: 0
exercises: 0
questions:
- "What is dataset shift?"
objectives:
- "Understand how dataset shift can lead to deterioration of models."
keypoints:
- "Dataset shift can lead to deterioration of models after deployment."
---

## Deployment of machine learning models

Machine learning models often face major challenges when applied in real-life settings. The tightly-controlled conditions under which models are trained are often very different to conditions "in the wild". Dataset shift is a term that is used to describe the nature of changing data conditions in the context of machine learning.

## Dataset shift

In their paper on [The Clinician and Dataset Shift in Artificial Intelligence](https://www.nejm.org/doi/full/10.1056/NEJMc2104626), Finlayson et al explore different causes of dataset shift within hospitals, suggesting policies for recognising these changes as well as strategies for mitigation. While the article itself is paywalled, there is an [openly available summary](https://sgfin.github.io/assets/dataset_shift/NEJM_DS_Supplement.pdf) of the key points raised in the article.

The authors suggest that dataset shift occurs as a result of three broad categories of change: 

- Changes in Technology: for example, introduction of a new data acquisition device.
- Changes in Population and Setting: for example, a change in patient demographics.
- Changes in Behavior: for example, a change in clinical practice.

<!--  
Task: read section X and answer questions.
-->

{% include links.md %}
