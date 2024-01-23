---
layout: post
title: Evaluating Fairness of Ranking Algorithms
categories: projects
permalink: projects/fairness-in-ranking-algorithms
authors: Zainab Iftikhar
---
    
<p> Mitigating bias in hiring algorithms: A Fairness Analysis. 
<em>exploreCSR 2022 </em></p>

----

## Abstract

<p> Existing hiring algorithms often claim to be "unbiased" but typically aim to meet basic Equal Employment Opportunity Commission (EEOC) requirements. Even when they meet these standards, they may still exhibit discriminatory behavior when interacting with hiring managers. This study investigates the inherent biases in hiring algorithms, with a focus on the efficacy of mitigating bias by removing gender, race, and class identifiers from the ranking process. Two forms of discrimination are assessed: disparate treatment and disparate impact, commonly measured by the "4/5" rule. <!-- Current approaches to mitigating bias in ranking algorithms fall into two categories: in-processing, which involves data cleaning and ranking without machine learning, and post-processing, which includes data cleaning, ranking, evaluation, and potentially multiple rounds of reranking, typically employing machine learning techniques.--> </p>

<p> In this research, four ranking algorithms are analyzed, with a specific focus on <b> Themis-ml: a fairness-aware post-processing machine learning algorithm </b>. Four training models are evaluated using Themis-ml, employing a protected attribute (gender) and training data from the German Credit Score dataset. These models include a Baseline (B) classifier trained on all input variables, a Remove Protected Attribute (RPA) classifier that excludes protected attributes, a Reject-Option Classification (ROC) classifier, and an Additive Counterfactually Fair Model (ACF) classifier. </p>

<p> We compared the percentage of men and women classified as low-risk for a loan and examines the utility effectiveness by checking if the AUC value remains constant. The findings indicate that men (the unprotected group) are 12% more likely to be labeled as low risk. Notably, PRA and B models show no significant change in the distribution between gender groups. However, the ACF model reduces the disparity between gender groups, while the ROC model surprisingly favors women being labeled as low risk.</p>

<p> All four training models maintain the utility AUC value, ensuring that fairness improvements do not compromise the algorithms' effectiveness. However, we found that <b> merely removing identifiers associated with attributes like gender, race, or class does not suffice to improve the fairness of ranking results</b>. The research emphasizes the need for real-life evaluations to achieve better representation for marginalized groups. <!--Future work should also address the broader social and systemic dimensions of ranking and hiring algorithms. Importantly, all four training models maintain the utility AUC value, ensuring that fairness improvements do not compromise the algorithms' effectiveness.--> </p>

----

## Poster

<embed src="/assets/projects/fairness_hiring_exploreCSR.pdf" type="application/pdf" width="100%" height="500px" />


[Click here for a full-screen view.](/assets/projects/fairness_hiring_exploreCSR.pdf)

---
