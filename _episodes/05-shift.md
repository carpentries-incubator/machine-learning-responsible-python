---
title: "Dataset shift"
teaching: 20
exercises: 10
questions:
- "What is dataset shift?"
- "What are examples of dataset shift?"
- "What are the implications of dataset shift?"
objectives:
- "Recognise causes of dataset shift."
- "Understand the potential outcomes of dataset shift."
keypoints:
- "Dataset shift can result from changes in technology, population, and behaviour."
- "Dataset shift can lead to deterioration of models after deployment."
- "Dataset shift is a major issue in terms of deployment of machine learning models."
---

## Dataset shift

Machine learning models often face major challenges when applied in real-life settings. The tightly-controlled conditions under which models are trained are often very different to conditions "in the wild". Dataset shift is a term that is used to describe the nature of changing data conditions in the context of machine learning.

In their paper on [The Clinician and Dataset Shift in Artificial Intelligence](https://www.nejm.org/doi/full/10.1056/NEJMc2104626), Finlayson et al explore different causes of dataset shift within hospitals, suggesting policies for recognising these changes as well as strategies for mitigation. 

While the article itself is paywalled, there is an [openly available summary](https://sgfin.github.io/assets/dataset_shift/NEJM_DS_Supplement.pdf) of the key points raised in the article. The authors suggest that dataset shift occurs in a clinical setting as a result of three broad categories of change: Changes in Technology; Changes in Population and Setting; and Changes in Behavior.

<!-- - Changes in Technology: for example, introduction of a new data acquisition device.
- Changes in Population and Setting: for example, a change in patient demographics.
- Changes in Behavior: for example, a change in clinical practice. -->

## Changes in technology

The International Classification of Diseases (ICD) system is a globally used set of disease codes maintained by the World Health Organisation (WHO), revised periodically. When revisions are introducted, this can affect the clinical prediction models that are built upon them. 

For example, [study that examined insurance claims](https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2764197) for >18 million adults and children in the US from 2010 to 2017 found that the transition from ICD-9 to ICD-11 led to instantaneous increases or decreases of 20% or more in the prevalence of many diagnostic categories.

Finlayson and colleagues suggest that fixing such an issue might require mapping of concepts, or even retraining of models. Referring to the [Finlayson paper](https://sgfin.github.io/assets/dataset_shift/NEJM_DS_Supplement.pdf), what is is another example of a technology change that might lead to dataset shift, and how might it be addressed? 

## Changes in population and setting

In [The Parable of Google Flu: Traps in Big Data Analysis](https://gking.harvard.edu/files/gking/files/0314policyforumff.pdf) Lazer and colleagues discuss Google Flu Trends, a product developed
to predict U.S. flu burden:

> The initial version of GFT was a particularly problematic marriage of big and small data. Essentially, the methodology was to find the best matches among 50 million search terms to fit 1152 data points. The odds of finding search terms that match the propensity of the flu but are structurally unrelated, and so do not predict the future, were quite high. GFT developers, in fact, report weeding out seasonal search terms unrelated to the flu but strongly correlated to the CDC data, such as those regarding high school basketball. This should have been a warning that the big data were overfitting the small number of cases — a standard concern in data analysis. This ad hoc method of throwing out peculiar search terms failed when GFT completely missed the nonseasonal 2009 influenza A–H1N1 pandemic. In short, the initial version of GFT was part flu detector, part winter detector. 

Looking again a the [Finlayson paper](https://sgfin.github.io/assets/dataset_shift/NEJM_DS_Supplement.pdf), what is another example of a change in population or setting that could affect the performance of a model? How might the effects of this change be mitigated?

## Changes in behaviour

Laboratory tests are often important predictors in clinical models. [Research has found](https://www.bmj.com/content/361/bmj.k1479) that in many cases the timing of laboratory tests is as important, or more important, than the results of the tests themselves:

> The presence of a laboratory test order, regardless of any other information about the test result, has a significant association (P<0.001) with the odds of survival in 233 of 272 (86%) tests. Data about the timing of when laboratory tests were ordered were more accurate than the test results in predicting survival in 118 of 174 tests (68%).

Minor changes in clinical practice - for example, a change in the routine of ordering a particular laboratory test - may therefore have unintended side-effects in terms of the performance of machine learning models trainined on laboratory data. 

{% include links.md %}
