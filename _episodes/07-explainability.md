---
title: "Explainability"
teaching: 0
exercises: 0
questions:
- "Do we need explainable models?"
objectives:
- "Consider the importance of explainability in machine learning."
keypoints:
- "The importance of explainability is a matter of debate."
---

## Explainability

<!--  TODO:

- Look at: https://twitter.com/christophmolnar/status/1098604325562138624?s=11

"Interpretable" and "explainable" are terms that are often used interchangeably to describe the characteristic of a model to be understood. 

In recent literature, however, interpretable is most often used to refer to models with limited complexity and predictable behaviour. For example, a decision tree:

[TODO: figure]

Explainable, on the other hand,...

> machine learning models for which the input data are of limited complexity and clearly understandable, quantifying the relationships between these simple inputs and the outputs of the model is termed inherent explainability

If a model is making a prediction, many of us would like to know how the decision was reached. With this understanding, we gain trust. Machine learning models - in particular neural networks - are often criticised for being "black boxes". 

https://www.sciencedirect.com/science/article/pii/S2589750021002089#bib1

-->

## Saliency maps

<!--  TODO:

-->

## Shapley values

<!--  TODO:

This has led to calls for explainable models.

In "Stop Explaining Black Box Machine Learning Models for High Stakes Decisions and Use Interpretable Models Instead", Cynthia Rudin

There is a distinction

-->

## Explainability of machine learning models

The requirement for explainability is even making its way into legal governance. The European Union General Data Protection (GDPR)) for example, states that "[the data subject should have] the right ... to obtain an explanation of the decision reached".

While at face value explainability seems like something that we would want in our models, this is a topic of much debate. https://arxiv.org/pdf/1702.08608.pdf

If our doctor or nurse recommends paracetamol (acetaminophen) for pain management, most of us would accept the suggestion without question. This is despite the action of paracetamol at a molecular level being unclear [https://pubmed.ncbi.nlm.nih.gov/15662292/]. 

Some would also argue that an explainable model creates trust where it is not well founded. A model may convince us that its reasoning is sound, even where it is not.

Examples, and discussion.

{% include links.md %}
