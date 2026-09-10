---
layout: page
title: Research
permalink: /research/
description: 
nav: true
nav_order: 2
---

# From Information to Intelligence: Building Relevant, Trustworthy, and Efficient AI Systems


## Introduction

The rapid evolution of artificial intelligence is fundamentally changing how information is produced, accessed, interpreted, and used for decision-making. Early information systems were primarily concerned with storing, searching, and retrieving information. The emergence of the social Web introduced a new challenge: users became both consumers and producers of massive quantities of heterogeneous and continuously evolving data. More recently, advances in machine learning, deep learning, and large language models (LLMs) have transformed information systems again—from systems that primarily retrieve and rank existing information into intelligent systems capable of learning representations, making predictions and recommendations, generating content, and interacting directly with users.

My research has evolved alongside these transformations. It lies at the intersection of **Information Retrieval (IR), Machine Learning (ML), Natural Language Processing (NLP), and Artificial Intelligence (AI)**. The central objective of my research is to develop intelligent systems that can effectively identify, rank, interpret, and act upon relevant information in complex environments. Throughout my research career, I have approached this objective from complementary perspectives, including personalized and social information retrieval [10.1145/2009916.2010075, 10.1145/2484028.2484131, 10.1145/2484028.2484130, BOUADJENEK20161], query understanding and reformulation [10.1145/2746090.2746092, 10.1145/2766462.2767801], recommender systems [10.1145/3331184.3331292, 10.1145/3597499], learning from dynamic and imperfect data [doi:10.1137/1.9781611975673.25, 10.1007/978-3-031-70381-2_7], explainable and trustworthy AI [10.1007/978-3-031-13643-6_9, 10.1007/978-3-031-28244-7_25, 10884425], and, more recently, efficient machine learning at the edge [khouas2026training].

Despite their apparent diversity, these research directions address a common question:

> *How can we design intelligent systems that exploit context, structure, prior knowledge, and computational resources to provide information and decisions that are relevant, trustworthy, and efficient?*

I organize my research around three complementary themes: **Relevant AI**, which seeks to understand what information is useful and to whom; **Trustworthy AI**, which addresses whether intelligent systems make reliable, robust, and justifiable decisions; and **Efficient AI**, which asks how these capabilities can be delivered under realistic computational constraints.

## Past and Current Research (The Foundation)

### Relevant AI: From IR to Intelligent Recommendation

My early research focused on **personalized and social information retrieval**. Traditional retrieval systems primarily model relevance as a relationship between a query and a document. I investigated how this view could be extended by incorporating information about users, their interests, social relationships, and interactions with information.

I developed approaches for personalized social query expansion [10.1145/2009916.2010075], personalized ranking through the **SoPRa** model [10.1145/2484028.2484131], and socially enriched document representations [10.1145/2484028.2484130]. These contributions were integrated into **LAICOS**, an open-source platform for personalized social Web search [10.1145/2487575.2487705], and later extended through **PerSaDoR**, which incorporates social context directly into personalized document representations [BOUADJENEK2016614]. This body of work also led to a broader survey and taxonomy of **Social Information Retrieval** [BOUADJENEK20161].

A central principle emerged from this research: **relevance is contextual**. An intelligent system should model not only the information being processed, but also the user and the environment in which that information is consumed.

I subsequently explored this principle in specialized retrieval and recommendation problems. In patent prior-art search, I studied query expansion and reduction for partial patent applications, demonstrating that retrieval strategies should adapt to the structure and length of the available patent information [10.1145/2746090.2746092]. In biomedical information retrieval, I investigated multi-field query expansion and the use of scientific literature to assess the quality and consistency of biological database records [10.1093/database/bax062].

My research then extended from search to **recommender systems**. I have worked on collaborative filtering using multiple data sources [bouadjenek2018dbkda], generative recommendation models [10.1145/3331184.3331292], and diversification [10.1145/3477495.3531890]. More recently, I have investigated **conversational recommendation**, including how user preferences evolve through interaction [10.1145/3442381.3450123, 10.1145/3597499] and how language-model-driven systems may introduce unintended biases [SHEN2023103139]. These directions represent a natural continuation of my earlier work on personalization: the objective remains to understand the user's information need and deliver information that is relevant to that particular context.

### Trustworthy AI: From Prediction to Reliable Intelligence

As my research moved increasingly toward machine learning, a second question became central: **can we trust how a model reaches its decisions?** Predictive accuracy alone is insufficient when a system can obtain the correct answer for the wrong reason, fail under distribution shift, violate known structural constraints, or reproduce unintended biases [GUPTA2023110685, 10884425, SHEN2023103139].

My work on **prior-knowledge dissemination and explainability** illustrates this challenge. In sentiment classification, we investigated whether neural models claimed to incorporate linguistic logic rules actually used those rules when making predictions. Our analysis showed that classification accuracy can conceal incorrect reasoning: a model may predict the correct sentiment while relying on evidence inconsistent with the intended linguistic rule [10.1007/978-3-031-13643-6_9, GUPTA2023110685]. This motivated mask-based approaches that explicitly incorporate prior knowledge into neural representations and constrain which parts of an input influence a prediction [10.1007/978-3-031-28244-7_25, 10651532].

I have extended this principle to **hierarchical classification**, where known relationships between classes provide valuable prior structure. We developed a model-agnostic mask-based output layer that embeds a taxonomy directly into the prediction mechanism, ensuring that predictions across different hierarchical levels remain consistent [10.1145/3511808.3557534]. Subsequent work has explored transformer and taxonomy-aware architectures for hierarchical classification [10.1007/978-981-97-2259-4_29, NOOR2025114444], as well as the use of taxonomic knowledge with multimodal language models [chen-etal-2025-leveraging].

A related strand of my research addresses **robustness under distribution shift**. My earlier work on temporally stable learning investigated how classification models can avoid reliance on features whose predictive value changes over time [Iman_Sanner_Bouadjenek_Xie_2017, doi:10.1137/1.9781611975673.25].

More recently, I have studied **out-of-distribution (OOD) detection**. We proposed Margin-bounded Confidence Scores (MaCS), which explicitly increases the separation between in-distribution and OOD confidence scores while preserving classification performance [10884425]. This research contributes to the broader goal of enabling models to recognize when an input lies outside the conditions under which their predictions can be trusted [Tamang2025, 11098614].

I have also investigated the challenges created by **missing and imperfect data**. Our work critically examined whether advanced machine-learning and deep-learning imputation techniques consistently outperform traditional approaches [10.1007/978-3-031-70381-2_7]. More recently, we developed **MissDDIM**, a deterministic conditional diffusion framework for tabular imputation that achieves competitive imputation accuracy while reducing inference latency and output variability [10.1145/3746252.3760943].

Across explainability, hierarchical learning, OOD detection, bias, and missing data, the underlying objective is the same: to move beyond systems that merely produce accurate predictions toward systems whose behaviour is **reliable, structured, and understandable**.

### Efficient AI: From the Cloud to the Edge

The rapid growth of modern AI introduces a third challenge: **computational efficiency**. Increasing model size has produced remarkable capabilities, but also substantial costs in computation, memory, communication, energy, latency, and infrastructure.

My recent research therefore investigates **machine learning at the edge**, where models must operate closer to the devices and data that they serve. Our work on training machine-learning models at the edge examines on-device, distributed, federated, transfer-learning, and knowledge-distillation approaches, together with the hardware, communication, data, and resource constraints that distinguish edge learning from conventional cloud-based machine learning [khouas2026training].

This research has led me to a broader question that is becoming particularly important with the emergence of LLMs:

> *How much computation does an AI system actually need to solve a particular problem?*

Rather than treating efficiency as an implementation problem that is addressed after a model has been developed, I view computational resources as part of the **learning and decision problem itself**. This perspective motivates my current and future research on adaptive and resource-aware AI [khouas2026training].

## Future Research

My future research will bring **relevance, trustworthiness, and efficiency** together in the context of foundation models and intelligent information systems.

A first direction is **resource-aware LLM inference**. Current systems typically allocate computation according to model architecture rather than the difficulty of an individual request. Yet a simple factual query should not necessarily consume the same computational resources as a difficult reasoning problem. I aim to investigate adaptive inference strategies that dynamically select the model, precision, inference method, and execution environment according to task difficulty and resource constraints. This includes model routing, quantization, early exiting, speculative decoding, and collaboration between cloud and edge resources.

A second direction is **trustworthy and knowledge-aware foundation models**. My previous research has demonstrated the value of explicitly incorporating linguistic rules, taxonomies, contextual information, and other forms of prior knowledge into machine-learning systems. I intend to extend this principle to foundation models by investigating mechanisms that incorporate domain knowledge, evidence, constraints, and uncertainty directly into model reasoning and evaluation.

Finally, I am interested in the growing convergence of **information retrieval, recommendation, and generative AI**. Search retrieves information, recommendation selects information for particular users, and generative models synthesize information into answers. Future intelligent systems will increasingly combine all three. My research on personalized retrieval, recommendation, user interaction, and trustworthy AI provides a foundation for developing retrieval-augmented and conversational systems that decide **what to retrieve, what to trust, how to personalize it, and how much computation to expend**.

## Research Vision

The evolution of my research can be summarized as a progression **from information to intelligence**. My early research asked how systems could identify **the right information for the right user**. My subsequent work investigated how learning algorithms could operate on complex, dynamic, and imperfect data. My more recent research asks whether their decisions are **trustworthy** and whether increasingly powerful AI models can operate **efficiently**.

These questions are becoming inseparable. A system that produces an accurate answer but ignores the user's information need is not useful. A highly relevant system whose decisions cannot be trusted is not reliable. And a trustworthy, high-performing system that requires excessive computational resources cannot be deployed sustainably at scale.

My long-term vision is therefore to develop AI systems that simultaneously understand **what information is relevant**, determine **when and why their decisions can be trusted**, and use **only the computational resources necessary for the task**. Ultimately, I aim to contribute to intelligent systems that identify the right information, reason about it reliably, deliver it to the right user, and do so efficiently.





