---
title: "Dataset leakage"
teaching: 0
exercises: 0
questions:
- "What is dataset leakage?"
objectives:
- "Understand how leakage can lead to over-optimistic expectations of performance."
keypoints:
- "Leakage occurs when training data is contaminated with information that is not available at prediction time."
---

## Dataset leakage

Dataset leakage is the mistaken use of information in the model training process that in reality would not be available at prediction time. The result of data leakage is overly optimistic expectations and poor performance in out-of-sample datasets.

An extreme example of data leakage would be accidentally including a prediction target in a training dataset. In this case our model would perform very well on training data. The model would fail, however, when moved to a real-life setting where the outcome was not available at prediction time.

![Dataset leakage](../fig/placeholder.png){: width="600px"}

In most cases information leakage is much more subtle than including the outcome in the training data, and it may occur at many stages during the model training process. 

## Imputation prior to train-test split

One common practice that leads to data leakage is choosing to impute missing values *prior* to creating train and test splits. The result - while minor - is likely to be overestimated performance on the test set. A similar issue may occur if scaling a dataset prior to creating the train and test splits.

```python
# TODO: demonstrate effect of filling missing data prior to splitting.
```

## Non-independence across train-test split

Another issue that can lead to data leakage is to not account for grouping within a dataset when creating train-test splits. Let's say, for example, that we are trying to use chest x-rays to predict which patients have cardiac disease. If the same patient appears multiple times within our dataset and this patient appears in both our training and test set, this may be cause for concern.

![Dataset leakage](../fig/x-ray-split.png){: width="600px"}

## Accessing future information

Another common cause of leakage is to mistakenly use information from the future when making a prediction. This is especially easy to do when working with retrospective data archived in relational databases, where the temporal aspects of data may be unclear. 

In [Data Leakage in Health Outcomes Prediction With Machine Learning](https://www.jmir.org/2021/2/e10969/PDF) Chiavegatto Filho et al reflect [on a study](https://www.jmir.org/2018/1/e22/PDF) that describes a machine learning model for prediction of hypertension in patients using electronic health record data.

<!--  
Task: read section X and answer questions.
-->

{% include links.md %}
