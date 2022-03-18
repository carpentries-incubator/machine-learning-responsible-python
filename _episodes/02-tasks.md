---
title: "Tasks"
teaching: 20
exercises: 10
questions:
- "Which tasks are appropriate for machine learning?"
- "What are the principles of ethical machine learning?"
objectives:
- "Become familiar with principles for ethical research."
- "Consider whether tasks are appropriate for machine learning."
keypoints:
- "Not all applications of machine learning are for the public good."
---

## Tackling the right tasks

Machine learning is a rapidly advancing, powerful technology that is helping to drive innovation. Before embarking on a machine learning project, we need to consider the task carefully. Many machine learning efforts are not solving problems that need to be solved. Worse, many applications of machine learning are not for the public good. 

The [NIH Guiding Principles for Ethical Research](https://www.nih.gov/health-information/nih-clinical-research-trials-you/guiding-principles-ethical-research) provide a useful set of considerations for any project. A condensed version of these principles is outlined below:

- Social and clinical value: Does the social or clinical value of developing and implementing the model outweigh the risk and burden of the people involved?
- Scientific validity: Once created, will the model provide valid, meaningful outputs?
- Fair subject selection: Are the people who contribute and benefit from the model selected fairly, and not through vulnerability, privilege, or other unrelated factors?
- Favorable risk-benefit ratio: Do the potential benefits of of developing and implementing the model outweigh the risks?
- Independent review: Has the project been reviewed by someone independent of the project, and has an Institutional Review Board (IRB) been approached where appropriate? 
- Informed consent: Are participants whose data contributes to development and implementation of the model, as well as downstream recipients of the model, kept informed?
- Respect for potential and enrolled subjects: Is the privacy of participants respected and are steps taken to continuously monitor the effect of the model on downstream participants?

What kind of tasks should we be trying to tackle? How much should we worry about technology being misused several years down the line? The answers are not always clear. Here we explore some cases that have raised concerns relating to discrimination, misinformation, and privacy.

## Identifying genetic disorders

In 2019, Nature Medicine [published a paper](https://www.nature.com/articles/s41591-018-0279-0.epdf) that described work to develop a model that could identify genetic disorders from a photograph of a patient's face. The abstract of the paper is copied below:

> Syndromic genetic conditions, in aggregate, affect 8% of the population1. Many syndromes have recognizable facial features that are highly informative to clinical geneticists3–5. Recent studies show that facial analysis technologies measured up to the capabilities of expert clinicians in syndrome identification. However, these technologies identified only a few disease phenotypes, limiting their role in clinical settings, where hundreds of diagnoses must be considered. Here we present a facial image analysis framework, DeepGestalt, using computer vision and deep-learning algorithms, that quantifies similarities to hundreds of syndromes. DeepGestalt outperformed clinicians in three initial experiments, two with the goal of distinguishing subjects with a target syndrome from other syndromes, and one of separating different genetic sub-types in Noonan syndrome. On the final experiment reflecting a real clinical setting problem, DeepGestalt achieved 91% top-10 accuracy in identifying the correct syndrome on 502 different images. The model was trained on a dataset of over 17,000 images representing more than 200 syndromes, curated through a community-driven phenotyping platform. DeepGestalt potentially adds considerable value to phenotypic evaluations in clinical genetics, genetic testing, research and precision medicine.

- What is the proposed value of the algorithm?
- What are the potential risks?
- Are you supportive of this kind of research?

This technology underpins a phone app called Face2Gene, which is able to report on genetic conditions at the snap of a person's face. Media reports on the technology generally favourably, for example reporting on the [excitement of clinicians at this technology](https://www.genengnews.com/insights/a-i-gets-in-the-face-of-rare-genetic-diseases/):

> In a room full of clinical geneticists, he projected many faces of people who had been diagnosed with varying dysmorphic diseases and asked the physicians to assign a genetic disorder to each face. Suffice it to say, the physicians performed poorly—far worse than the computer...One of the most exciting aspects of the program ... is its ease. After asking just one question to a patient, “is it ok if I take a picture?” and snapping a quick photo, the program offers results back within seconds.

<!-- >
https://www.nature.com/articles/d41586-019-00027-x

- "Face2Gene’s recognition rate for Down syndrome was 80% among white Belgian children, it was just 37% for black Congolese children" affect your view?
-->


## "Reading" a person's face

There is a long history of physiognomy, the "science" of trying to read someone's character from their face. With the advent of machine learning, this discredited area of research has made a comeback. There have been numerous studies attempting to guess characteristics such as trustworthness, criminality, and political and sexual orientation.

In 2018, for example, researchers [suggested that](https://www.gsb.stanford.edu/faculty-research/publications/deep-neural-networks-are-more-accurate-humans-detecting-sexual) neural networks could be used to detect  sexual orientation from facial images. The abstract is copied below:

> We show that faces contain much more information about sexual orientation than can be perceived and interpreted by the human brain. We used deep neural networks to extract features from 35,326 facial images. These features were entered into a logistic regression aimed at classifying sexual orientation. Given a single facial image, a classifier could correctly distinguish between gay and heterosexual men in 81% of cases, and in 74% of cases for women. Human judges achieved much lower accuracy: 61% for men and 54% for women. The accuracy of the algorithm increased to 91% and 83%, respectively, given five facial images per person. Facial features employed by the classifier included both fixed (e.g., nose shape) and transient facial features (e.g., grooming style). Consistent with the prenatal hormone theory of sexual orientation, gay men and women tended to have gender-atypical facial morphology, expression, and grooming styles. Prediction models aimed at gender alone allowed for detecting gay males with 57% accuracy and gay females with 58% accuracy. Those findings advance our understanding of the origins of sexual orientation and the limits of human perception. Additionally, given that companies and governments are increasingly using computer vision algorithms to detect people’s intimate traits, our findings expose a threat to the privacy and safety of gay men and women.

- What is the proposed value of the algorithm?
- What are the potential risks?
- Are you supportive of this kind of research?

A [response from GLAAD](https://www.glaad.org/blog/glaad-and-hrc-call-stanford-university-responsible-media-debunk-dangerous-flawed-report), a leading LGBTQ media advocacy organization described the work as dangerous and flawed. Meanwhile an [article in Scientific American](https://blogs.scientificamerican.com/observations/can-we-read-a-persons-character-from-facial-images/) notes that:

> This is precisely the kind of “scientific” claim that can motivate repressive governments to apply AI algorithms to images of their citizens. And what is it to stop them from “reading” intelligence, political orientation and criminal inclinations from these images?

<!--

## Reflection.

TODO: there should be a reflection here. What is an appropriate task. What is an ethical consideration? Say a few words. Who makes the decision and based on what. REFLECTION. 1. Regulation 2. Social 3. 

## Imitation

<!-- TODO: 

https://economictimes.indiatimes.com/magazines/panache/deep-nostalgia-new-online-ai-tool-brings-portraits-of-dead-relatives-to-life-some-call-it-spooky/articleshow/81245242.cms?from=mdr

https://www.theverge.com/a/luka-artificial-intelligence-memorial-roman-mazurenko-bot

Deep fakes.

## Surveillance and privacy

<!-- TODO: 

https://blogs.microsoft.com/on-the-issues/2018/12/06/facial-recognition-its-time-for-action/

https://www.nature.com/articles/d41586-020-03188-2

http://www.policingethicspanel.london/uploads/4/4/0/7/44076193/live_facial_recognition_final_report_may_2019.pdf

https://www.adalovelaceinstitute.org/report/beyond-face-value-public-attitudes-to-facial-recognition-technology/

https://blogs.microsoft.com/on-the-issues/2018/12/06/facial-recognition-its-time-for-action/

-->

{% include links.md %}