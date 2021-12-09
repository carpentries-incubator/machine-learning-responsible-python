---
title: "Changing data"
teaching: 0
exercises: 0
questions:
- "What are data leakage and data shift?"
objectives:
- "Understand how leakage and shift lead to poor models."
keypoints:
- "Leakage and shift lead to poorly performing models."
---

## Changing data

In most cases where we seek to deploy machine learning models, data is being generated continuously over time. In transactional systems, data points may be updated and changed.

When training machine learning models, we typically work with snapshots of data: static spreadsheets of predictors and outcomes that obscure temporality.

## Data leakage

Leakage happens when training data is contaminated with information that should not be available to our model. An extreme example would be including a prediction target in the training data. In reality leakage is usually much harder to spot.

https://www.jmir.org/2021/2/e10969

Examples, and discussion.

## Data shift

Dataset shift describes the issue of data changing after a model is deployed. It is not enough to train a model and then let it be. After deployment, models need to be audited and adapted.

https://static1.squarespace.com/static/59d5ac1780bd5ef9c396eda6/t/60fb3ba110343004004f24ba/1627077538209/Performance_Gap___Prospective_Validation.pdf

https://proceedings.neurips.cc/paper/2019/file/846c260d715e5b854ffad5f70a516c88-Paper.pdf

Examples, and discussion.

{% include links.md %}
