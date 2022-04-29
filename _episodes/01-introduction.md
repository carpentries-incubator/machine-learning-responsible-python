---
title: "Introduction"
teaching: 20
exercises: 10
questions:
- "What do we mean by responsible machine learning?"
- "What types of harm may result from development and deployment of machine learning models?"
- "What steps are being taken to mitigate the risks of harm?"
objectives:
- "Understand what is meant by responsible machine learning."
- "Recognise the types of harm that may be a consequence of machine learning"
- "Recognise the current state of oversight and regulation of machine learning"
keypoints:
- "There is potential for machine learning models to cause harm."
- "Researchers are increasingly required to reflect on the impact of their work."
- "Regulation and oversight are in their infancy."
---

## Responsible machine learning

<!-- 

TODO: reduce length of abstracts? Or avoid reading them and ask to read them.


TODO: 
# Guidelines and quality criteria for artificial intelligence-based prediction models in healthcare
https://www.nature.com/articles/s41746-021-00549-7

-->

Like many technologies, machine learning has the potential to cause harm is applied inappropriately. With machine learning the issues can be subtle: a seemingly good model may in fact be anything but. As an emerging technology, machine learning is largely self-regulated so awareness of potential pitfalls is especially important. 

In this lesson we look broadly at a number of topics that are important for applying machine learning in a responsible manner. We do not attempt to define "responsible machine learning", but we cover topics that a person who practices machine learning should be aware of. Topics range from choosing appropriate tasks, to awareness of sources of bias, to the susceptibility of models to manipulation.

Given that "Artificial Intelligence" (or "A.I.") has largely become a synonym for machine learning, especially in popular culture, we will use these terms interchangeably.

<!-- Are concerns about the risks of machine learning warranted? We believe so. Machine learning models have quickly become part of everyday life. Models have caused physical harm (think autonomous driving and automated medical diagnosis) 

https://www.antidiskriminierungsstelle.de/EN/homepage/_documents/download_diskr_risiken_verwendung_von_algorithmen.pdf?__blob=publicationFile&v=1
-->

## Potential harm

What are some examples of machine learning systems that are already in active public use? What kinds of harm could result from the application of machine learning systems? Should we be concerned or are these risks overhyped?

In their [guide to Understanding artificial intelligence ethics and safety](https://www.turing.ac.uk/sites/default/files/2019-08/understanding_artificial_intelligence_ethics_and_safety.pdf) The Turing Institute highlight examples of the kind of harm that may result from application of machine learning system.  Take a look at the table on pages 5-6 of the Turing Report. How many categories of harm are highlighted? 

> ## Exercise
> Match the following sentences to one of the categories of harm highlighted in the report.
> 
> A) Situations may arise where such individuals are unable to hold the parties responsible for outcomes directly accountable.
> 
> B) Data capture is often invasive, revealing personal information. Deployment of models may infringe upon the ability of individuals to lead a private life.  
> 
> C) Irresponsible data management, negligent design and production processes, and questionable deployment practices can, each in their own ways, lead to the implementation and distribution of AI systems that produce unreliable, unsafe, or poor-quality outcomes.
> 
> D) Technologies can reproduce, reinforce, and amplify the patterns of marginalisation, inequality, and discrimination that exist in these societies.
> 
> E) Excessive automation might reduce the need for human-to-human interaction. Hyper-personalisation may limit our exposure to world views. Well-ordered and cohesive societies are built on relations of trust, empathy, and mutual understanding. As technologies become more prevalent, it is important that these relations be preserved.   
> 
> F) The reason for algorithmic decisions may remain opaque to its subjects. Where the model harbours traces of discrimination, bias, inequity, or unfairness, this opaqueness may be deeply problematic. 
> 
> > ## Solution
> > A) Denial of Individual Autonomy, Recourse, and Rights  
> > 
> > B) Invasions of Privacy
> > 
> > C) Unreliable, Unsafe, or Poor-Quality Outcomes
> > 
> > D) Bias and Discrimination
> > 
> > E) Isolation and Disintegration of Social Connection
> > 
> > F) Non-transparent, Unexplainable, or Unjustifiable Outcomes
> > 
> {: .solution}
{: .challenge}


## Need for oversight

In recent years there have been important changes that have sought to introduce scrutiny and safeguards to the development and application of machine learning. A [2018 statement](https://web.archive.org/web/20200101022756/https://acm-fca.org/2018/03/29/negativeimpacts/) by scientists at the Association for Computing Machinery (ACM), for example, highlighted growing concerns around lack of oversight:

> "There clearly is a massive gap between the real-world impacts of computing research and the positivity with which we in the computing community tend to view our work. We believe that this gap represents a serious and embarrassing intellectual lapse. The scale of this lapse is truly tremendous: it is analogous to the medical community only writing about the benefits of a given treatment and completely ignoring the side effects, no matter how serious they are."

Take a few moments to [read the ACM statement](https://web.archive.org/web/20200101022756/https://acm-fca.org/2018/03/29/negativeimpacts/). 

> ## Exercise
> A) What are some of the negative impacts of research reported in the article?
> 
> B) What "small change" do the authors suggest could have a big impact?
> 
> > ## Solution
> > A) Points include: Disruption of careers; Generated audio and video might threaten democracy; Decline in privacy rights; Spread of false information, conspiracy theories, and propaganda.
> > 
> > B) "Peer reviewers should require that papers and proposals rigorously consider all reasonable broader impacts, both positive and negative." Where projects were likely to have a net negative impact, the statement suggests that authors "be encouraged to discuss complementary technologies, policy, or other interventions that could mitigate the negative broader impacts".
> {: .solution}
{: .challenge}

## Impact statements

In 2020, for the first time the [call for papers](https://neurips.cc/Conferences/2020/CallForPapers) for the Conference and Workshop on Neural Information Processing Systems (NeurIPS), one of the largest machine learning conferences, introduced a requirement for authors to reflect on potential positive and negative consequences of their work with a statement on "broader impact":

>  In order to provide a balanced perspective, authors are required to include a statement of the potential broader impact of their work, including its ethical aspects and future societal consequences. Authors should take care to discuss both positive and negative outcomes.

While questions remain about the effectiveness of this policy change, it demonstrates growing recognition of the importance of responsible machine learning and it is a step towards the oversight that many believe is needed. An [analysis of the statements](https://arxiv.org/pdf/2105.04760.pdf) that were submitted to the 2020 conference found that the broader impact statements raised concerns in areas such as:

- Privacy: impact around personal data and surveillance.
- Labor: impact on employment and productivity.
- Environment: impact on the environment, including the carbon footprint of training models.
- Media: impact in the media, particularly around fake news and misinformation.
- Bias: impact in terms of fairness and discrimination.
- Reliability: impact of models that failed to meet expectations.
- Interpretability: impact of the opaqueness of models and the "black box problem".

## Regulation

The European Commission meanwhile is [developing a regulatory framework](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) with the goal of mitigating the risks of "artificial intelligence" across Europe and beyond. The [proposed regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:52021PC0206&from=EN) follows a risk-based approach, differentiating between uses of artificial intelligence that create (i) an unacceptable risk, (ii) a high risk, and (iii) low or minimal risk.

Systems that are deemed to have "unacceptable risk" - such as "social scoring by governments" and "toys using voice assistance that encourages dangerous behaviour" - would be banned. "High risk" systems - such as artificial intelligence assisted surgery - would be tightly regulated. The high-risk systems would, for example, be required to be trained on "high quality" datasets; to keep a log of their activity; and to be subject to human oversight.

{% include links.md %}
