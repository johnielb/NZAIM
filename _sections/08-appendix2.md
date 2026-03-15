---
layout: section
title: "Appendix 2: Map of NZ government algorithms and AI under the technical-contextual taxonomy"
short_title: Appendix 2
section_number: Appendix 2
description: Mapping of known New Zealand government AI systems to the proposed taxonomy.
---
# Appendix 1: Summary of challenges identified in each technical ([Section 4](../04-section4/)) category

****Legend****

<a id="table-6"></a>

| ***Build: Challenges addressed during the design and training (if data-driven) of the system*** |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| **Challenges** | **Hand-crafted** | **GDO** | **Supervised** | **Unsupervised** | **Generative** |
| **Output-outcome misalignment (proxy mismatch)** |  |  |  |  |  |
| **Biased, inequitable or homogeneous outputs** | Designer responsible |  |  |  |  |
| **Opacity makes it difficult to understand or review** |  | Technique dependent |  |  |  |
| **Input data accuracy assumed** |  | Often not known |  |  |  |
| **Confounding variables biases outputs** |  |  |  |  |  |
| **Value chain hard to interrogate** |  | If pre-trained |  |  |  |
| **Problem definition difficult** |  | No ‘truth’ | Highly generalisable |  |  |
| **Target(s) accuracy assumed** |  | No target | Often not known |  |  |
| **Output accuracy isn’t validated by design** |  |  |  |  |  |
| ***Process: Challenges outside the system’s build and use relating to how users and the environment interact with the system.*** |  |  |  |  |  |
| **Users vulnerable to automation bias** |  | More active controls needed |  |  |  |
| **User hijacking** | ‘Game’-able | ‘Game’-able if live | Often arbitrary |  |  |
| ***Use: Challenges that may arise during the operation of the system*** |  |  |  |  |  |
| **Concept or data drift** |  |  |  |  |  |
| **Compute cost** |  | If DL |  |  |  |
| **Hallucination** |  |  |  |  |  |
| **Unauthorised data reuse** |  |  |  |  |  |

# Appendix 2: Map of NZ government algorithms and AI under the technical-contextual taxonomy

{% include diagrams/appendix2-taxonomy-map.html %}

_* Pre-training generative AI systems is not the object of generative AI evaluation, which relies on expert and end-user acceptance in the specific context it is applied in, rather the general performance benchmarking undertaken in pre-training. Technically, pre-training (and prior fine-tuning) uses a combination of self-supervised, supervised and reinforcement learning. While fine-tuning may take place when the context has been established, this is only a means to improving the performance upon evaluation, not the end evaluation of the system per se._
