---
title: "Biased data"
teaching: 0
exercises: 0
questions:
- "How are biases in data reflected in models?"
objectives:
- "Consider sources of bias in data."
keypoints:
- "Biases in data lead to biased models."
---

## Learning from biased data

We live in a world full of bias. Education, salaries, and healthcare are not even evenly distributed: more often than not they are a reflection of our circumstances of birth.

Models may not suffer from many of the weaknesses of humans, but they are no less susceptible to bias.

## Word models

Word embeddings - used in many natural language processing tasks - seek to capture the distance between words in a multidimensional space. The embeddings often reinforce negative aspects of our culture.

Examples, and discussion.

https://proceedings.neurips.cc/paper/2016/file/a486cd07e4ac3d270571622f4f316ec5-Paper.pdf

## Labelled data

Human annotated data is often considered the gold standard for training models. If we are training a model to detect disease in x-rays, radiologist-added labels may be the ideal. Experts labels, however, are not free from bias. This bias will be learnt by our models. 

Examples, and discussion.

https://www.itnonline.com/content/study-reveals-bias-among-doctors-who-classify-x-rays-coal-miners-black-lung-claims

https://www.atsjournals.org/doi/10.1513/AnnalsATS.202010-1350OC

## Hidden patterns

Ophthalmologists cannot classify the sex of a patient from a retinal scan. Radiologists cannot classify the race of a patient from a chest x-ray. In both cases, it appears that machine learning models can.

Examples, and discussion.

https://www.nature.com/articles/s41598-021-89743-x

https://arxiv.org/pdf/2107.10356.pdf

{% include links.md %}