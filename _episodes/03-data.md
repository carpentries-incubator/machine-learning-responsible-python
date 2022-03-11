---
title: "Data"
teaching: 20
exercises: 10
questions:
- "How does data influence machine learning?"
- "How can we better document data?"
objectives:
- "Recognise how data influences machine learning models."
- "Learn an approach for structured documention of data characteristics."
keypoints:
- "Data is fundamental to the field of machine learning."
- "Datasheets can help us to reflect on the process of data creation and distribution."
---

## Data as a foundation

<!--
Should cover data representativeness: https://www.nature.com/articles/s41746-021-00549-7
-->

Data is crucial for the field of machine learning and it forms the foundation for the models that we build and use. When data is made available to the machine learning community, it has the ability to drive progress and shape the direction of research. Lack of available data, meanwhile, stifles and stalls progress. Despite the importance of data, its creation and sharing has often been relegated to footnotes in machine learning studies, seen as secondary to the work of model building and application.

In recent years there have been movements towards giving data greater prominence. The Conference on Neural Information Processing Systems, for example, introduced a [Dataset Track](https://neuripsconf.medium.com/announcing-the-neurips-2021-datasets-and-benchmarks-track-644e27c1e66c) for the first time in 2021 to encourage reporting "on highly valuable machine learning datasets and benchmarks" ... and to create a forum to discuss "how to improve dataset development".

## The data landscape

In **[Data and its (dis)contents: A survey of dataset development and use in machine learning research](https://arxiv.org/pdf/2012.05345.pdf)**, Paullada et al survey the research literature to explore how data has influenced the field of machine learning. Broadly, topics discussed include:

- Issues of representation, such as "glaring under-representation of darker skinned subjects ... within prominent facial analysis datasets"
- Propensity of models to make performance gains on datasets through "cheap tricks" that do not extrapolate well to out-of-distribution data.
- Risks of datasets in legitimizing problematic goals, such as the prediction of sexual preferences using social media photographs.
- Failure to recognize human annotation work as *interpretive work* that encodes subjective values and judgments, resulting in a conflation of "gold labels" with ground truth.
- Management and distribution of data, especially as it relates to privacy and risk of exploitation.

<!--  
Task: read section X and answer questions.
-->

## Data documentation

Given the fundamental role of data in machine learning, there have been calls for data sharers to provide better documention for the downstream consumers. In [Datasheets for Datasets](https://arxiv.org/pdf/1803.09010.pdf), Gebru et al call for data creators to provide "datasheets" to accompany the datasets that they share. 

The datasheets serve dual purposes: for the creator they encourage reflection on the data creation and distribution process, and for the consumer they offer details necessary to make informed decisions about using a dataset

> "We propose that every dataset be accompanied with a datasheet that documents its motivation, composition, collection process, recommended uses, and so on. Datasheets for datasets have the potential to increase transparency and accountability within the machine learning community, mitigate unwanted societal biases in machine learning models, facilitate greater reproducibility of machine learning results, and help researchers and practitioners to select more appropriate datasets for their chosen tasks

<!--  
Task: read section X and answer questions.
-->

{% include links.md %}