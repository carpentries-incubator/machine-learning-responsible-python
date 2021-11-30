---
title: "Introduction"
teaching: 20
exercises: 10
questions:
- "What are key considerations for building and implementing models?"
objectives:
- "Understand some of the risks of machine learning."
keypoints:
- "Misuse of machine learning models can cause harm."
---

## Responsible machine learning

Like many technologies, machine learning has the potential to cause harm is applied inappropriately. With machine learning the issues can be subtle: a seemingly good model may in fact be anything but. As an emerging technology, machine learning is largely self-regulated so awareness of potential pitfalls is especially important. 

In recent years there have been important changes that have sought to introduce scrutiny and safeguards. A [2018 statement](https://web.archive.org/web/20200101022756/https://acm-fca.org/2018/03/29/negativeimpacts/) by scientists at the Association for Computing Machinery (ACM), for example, highlighted growing concerns around lack of oversight:

> "There clearly is a massive gap between the real-world impacts of computing research and the positivity with which we in the computing community tend to view our work. We believe that this gap represents a serious and embarrassing intellectual lapse. The scale of this lapse is truly tremendous: it is analogous to the medical community only writing about the benefits of a given treatment and completely ignoring the side effects, no matter how serious they are."

The statement called for peer reviewers of papers and proposals to require authors to "rigorously consider all reasonable broader impacts, both positive and negative.". Where projects were likely to have a net negative impact, the statement suggests that authors "be encouraged to discuss complementary technologies, policy, or other interventions that could mitigate the negative broader impacts".

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

The European Commission meanwhile is [developing a regulatory framework](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) with the goal of mitigating the risks of "artificial intelligence" across Europe and beyond. The [proposed regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:52021PC0206&from=EN) follows a risk-based approach, differentiating between uses of artificial intelligence that create (i) an unacceptable risk, (ii) a high risk, and (iii) low or minimal risk.

Systems that are deemed to have "unacceptable risk" - such as "social scoring by governments" and "toys using voice assistance that encourages dangerous behaviour" - would be banned. "High risk" systems - such as artificial intelligence assisted surgery - would be tightly regulated. The high-risk systems would, for example, be required to be trained on "high quality" datasets; to keep a log of their activity; and to be subject to human oversight.

In this lesson we look broadly at a number of topics that are important for applying machine learning ina responsible manner. We do not define "responsible machine learning", but we attempt to cover topics that a person who practices machine learning should be reasonably aware of. Topics range from choosing appropriate tasks, to awareness of sources of bias, to the susceptibility of models to manipulation.

{% include links.md %}

Hecht, B., Wilcox, L., Bigham, J.P., Schöning, J., Hoque, E., Ernst, J., Bisk, Y., De Russis, L., Yarosh, L., Anjum, B., Contractor, D. and Wu, C. 2018. It’s Time to Do Something: Mitigating the Negative Impacts of Computing Through a Change to the Peer Review Process. ACM Future of Computing Blog. https://acm-fca.org/2018/03/29/negativeimpacts/. [Available from: https://brenthecht.com/papers/FCADIscussions_NegativeImpactsPost_032918.pdf]



