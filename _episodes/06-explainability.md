---
title: "Explainability"
teaching: 20
exercises: 10
questions:
- "What is explainability?"
- "Is explainability necessary?"
objectives:
- "Understand the concepts of explainability and interpretability."
- "Understand how saliency maps can help us to explain a model."
keypoints:
- "The importance of explainability is a matter of debate."
- "Saliency maps highlight regions of data that most strongly contributed to a decision."
---

## Interpretability and explainability

"Interpretable" and "explainable" are terms that are often used interchangeably to describe the characteristic of a machine learning model to be understood. In recent literature, however, interpretable is perhaps more often used to refer to models with limited complexity and predictable behaviour. For example, a decision tree may be inherently interpretable:

![Decision tree and boundaries.](../fig/decision-tree.png)

If we can look at our model and predict what will happen to our prediction if input values change, then we can say that the model is interpretable. Often, however, data and models are too complex and high-dimensional to be easily understood. They cannot be explained by a simple relationship between inputs and outputs.

For these complex models there is typically a focus on attempting to dissect the model's decision making procedure. This insights lead us to explainability: our ability to gaze into a complex model and explain its behaviour.

## The necessity of interpretability and explainability

If a model is making a prediction, many of us would like to know how the decision was reached. With this understanding, we gain trust. [Doshi-Velez and Kim](https://arxiv.org/pdf/1702.08608.pdf) suggest that interpretablity (/explainablity) can assist in ascertaining presence of desired features such as fairness, privacy, reliability, robustness, causality, usability and trust:

- Fairness: that groups are not discriminated against. 
- Privacy: that sensitive information is not revealed. 
- Reliability and robustness: that models reach certain levels of performance despite parameter or input variation. 
- Causality: that predicted changes in output due to a perturbation will occur as expected. 
- Usability: that methods provide information that assist users to accomplish a task.

In machine learning in health, it has been argued that explainable AI is necessary to gain trust with the health-care workforce, provide transparency into decision making processes, and to mitigate bias. As a counterpoint, [Ghassemi and colleagues](https://doi.org/10.1016/S2589-7500(21)00208-9) argue that urrent explainability methods are unlikely to achieve these goals for patient-level decision support.

Instead, they advocate for "rigorous internal and external validation of AI models as a more direct means of achieving the goals often associated with explainability", and "caution against having explainability be a requirement for clinically deployed models".

## Saliency maps

Saliency maps - and related approaches - are popular form of explainability for imaging models. Saliency maps use color to illustrate the extent to which a region of an image contributes to a given decision. For example, when building neural network models to predict lung conditions (pleural effusion) we can see the model pays particular attention to certain areas of an image.

![Saliency map for chest X-ray model](../fig/saliency.png)

While saliency maps may be useful, they are also [known to be problematic](https://arxiv.org/abs/1810.03292) in many cases. Displaying a region of importance leaves us to decide what the explanation might be. The human tendency is to assume that the feature we would find important is the one that was used (this is an example of a famously harmful cognitive error called confirmation bias). 

This problem is well summarised by computer scientist Cynthia Rudin: “You could have many explanations for what a complex model is doing. Do you just pick the one you 'want’ to be correct? The ability of localisation methods to mislead human users is compellingly demonstrated by [Adebayo and colleagues](https://arxiv.org/abs/1810.03292), who show that even untrained networks can produce saliency maps that appear reassuring.

<!--  TODO:

## Shapley values

In "Stop Explaining Black Box Machine Learning Models for High Stakes Decisions and Use Interpretable Models Instead", Cynthia Rudin

These concerns also extend to other well known post-hoc explanation methods such as locally interpretable model-agnostic explanations (LIME)27 and Shapley values (SHAP).28 LIME seeks to understand decisions at the individual level by permuting the input example (altering it in minor ways) and identifying which alterations were most likely to change the decision. In the case of image analysis, this is done by occluding parts of the image, the explanation consisting of a heat map that indicates the image components that were most important for the decision. Such explanations suffer from interpretability gaps in the same way as saliency mapping. Methods such as LIME and SHAP are generic and not specific to images and are routinely used on a wide variety of health-care data, including structured data from electronic health-care records29 and electroencephalogram waveform data.30

-->

> ## Explainability Algorithms Aren't Perfect
>
> When we make a machine learning model, we are trying to use a mathematical framework to recreate a system as faithfully as we can. Explainability algorithms then try and analyse these frameworks to understand how changes in the input variables will affect the predictions. There are many issues to consider when picking an explainability algorithm as **different algorithms can give different explanations of the same system**. In general 'simpler' models have more obvious methods of explainability and this is one of the reasons why they are favoured over 'more complex' models.
>
> There are more issues to consider than this though. We have to remember that as our models are sensitive to the training data our explainability algorithms will be too. Linear regression is generally considered to be the most explainable of all the machine learning algorithms. To explore the effect that small changes in input data can have, the [Boston Housing Data](https://www.kaggle.com/code/prasadperera/the-boston-housing-dataset/notebook) was taken, it was centered, scaled and bootstrapped 25,000 times. On each of these 25,000 resamples a linear regression model was trained and the coefficients for each predictor were saved (the larger the size of the coefficient, the 'more important' that variable is and whether it is positive or negative indicates whether it has a positive or negative effect on the model).
>
> ![LinRegExample](../fig/lin_reg_example.png)
>
> The left plot above shows the range of values of the coefficients for each predictor. Not only can you see that the value of the estimate varies alot, but there are variables (like `crim`) that are mainly negative but there are many variables where the coefficient is positive. This becomes obviously ludicrous because the real world interpretation of this would be *'the median value of owner-occupied homes in boston **increases** with the per capita crime rate of the town it is in'*.
>
> Not only does the value of the coefficients change, but the order of importance of the variables changes. Each predictor was ranked by importance for each model and the number of times a predictor appears in each position is shown in the histogram on the right above. You can see that how important variables are compared to one another can vary wildly, like the predictor `rm`, representing the average number of rooms per property in the town, is very sensitive to small changes in the collected data.
>
> All of this is to say, that just like you have to choose and evaluate your models carefully, so do you have to choose and evaluate your explainability algorithms carefully.
{: .callout}

## Explainability of machine learning models

The requirement for explainability is even making its way into legal governance. The European Union General Data Protection (GDPR)) for example, states that "[the data subject should have] the right ... to obtain an explanation of the decision reached".

If our doctor or nurse recommends paracetamol (acetaminophen) for pain management, most of us would accept the suggestion without question. This is despite the action of paracetamol at a molecular level [being unclear](https://pubmed.ncbi.nlm.nih.gov/15662292/). Are we holding machine learning models to a higher standard than humans? 


{% include links.md %}
