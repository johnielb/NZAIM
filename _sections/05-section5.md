---
layout: section
title: Guidance must acknowledge different requirements across different use cases AI is applied in
short_title: 5. Use Cases
section_number: Section 5
description: "Contextual taxonomy: front-line, research, and administrative AI use cases."
---
# Guidance must acknowledge different requirements across different use cases AI is applied in

All-of-Government stocktakes in 2018[^26] and 2024[^27] have illustrated the wide variety of ways that agencies already use or plan to use AI. The 2018 Algorithm Assessment Report helpfully delineated between three different types of algorithms, consistent with my definition of algorithms: operational algorithms, algorithms used for policy development and research, and business rules. This categorisation provides a useful contextual distinction between the aims of each kind of algorithm. Operational algorithms make or recommend complex decisions about individual users of government services. Policy algorithms make or recommend policy decisions that intervene at the aggregate system level. Business rules automate routine administrative processes without applying the same level of individual discretion as more advanced algorithms.

Six years later, the 2024 cross-agency survey of AI use cases applied a different theming of use cases rather than the previous systematic taxonomy. While this theming was useful to illustrate the different uses of AI in the public sector, it is not scalable given its focus on specific objectives, such as “boosting productivity and efficiency” and “enhancing customer experience”.

The 2024 survey also did not prompt agencies to consider different types of techniques, only prompting agencies to report on “AI use cases”. This oversight in survey design has led to agencies under-reporting what AI they use. For example, only one AI use case was identified by StatsNZ in the survey. However, traditional ML modelling has been used for official statistics like the International Migration provisional dataset since 2018, producing highly publicised metrics for policy impact like net migration. Use cases in ACC identified in Section 4 recognised in the 2018 survey were not disclosed in the 2024 survey. Its inclusion would have promoted an AI use case that has demonstrably financially benefitted ACC, improved the experience of injured people navigating the ACC system, and follows best practice[^28]. A better systematic definition of AI can improve coverage of all kinds of AI use cases in government and shine a light on low residual risk – but high impact – exemplars already embedded in agencies’ BAU.

## Action: A new taxonomy should differentiate between the different legal obligations associated with different use cases

A systematic taxonomy can ground AI standards and guidance to the specific considerations of the specific context which an AI used. Below, I propose a new taxonomy that builds on the 2018 categorisation to accommodate technologies that have emerged since then.

- Operational algorithms now belong to the **“front-line”** category of techniques, which now includes both algorithms and GenAI that directly and independently make a decision or recommendation regarding an individual that affects their rights or interests.

- Algorithms for policy development and research should also include operational research employing algorithms and AI, under the **“research”** category. This group includes both operational and policy research techniques that generate data to form the evidence base for system-level decision-making.

- Most business rules and generative AI tools now belong to the **“administration”** category of techniques, which do not directly lead to a conclusive decision but still have a material impact. They may use personal data, subjecting it to the Privacy Act.

> Figure 3: Taxonomy of use cases based on the relevant legal obligations within each category. Operational algorithms and any conclusive algorithm or GenAI are grouped into front-line. Evidence-generating algorithms and AI are grouped into research. Impactful but non-conclusive algorithms and GenAI are grouped into administration.

Like the previous section, I propose new definitions for these three categories rooted in the relevant legal obligations associated with each category, along with examples and the unique challenges each category faces. Applications inherit the challenges based on the intersection they make with the technical taxonomy (e.g. all three contextual categories are susceptible to learning biases when developing supervised learning models).

> Front-line AI directly makes decisions or recommendations around a user of government services, research AI generates evidence to inform system-level decisions, administrative AI support or automate the role of staff.


<div class="box" id="box-5-2-1">
<div class="box__header"><span class="box__number">Box 5.2.1</span><h3 class="box__title">Front-line</h3></div>
<div class="box__body" markdown="1">

Algorithms and AI with its own set of rules that make decisions or recommendations about individuals (including corporations) that affect their rights or interests. Users have specific official information rights to the reasons behind these decisions. Fully automated decision-making and human-in-the-loop algorithms are included as there is no legal distinction between the two in the OIA. However, this category only includes GenAI systems that independently forms its own evaluative conclusions. GenAI systems that collate and summarise evidence to support a human decision maker is administrative.

**Examples:**
- **Front-line algorithms**: MSD automated decision-making (e.g. child support payments), Te Whatu Ora triage rules (e.g. Clinical Priority Assessment Criteria)
- **Supervised front-line models**: ACC Probability of Accept, border agency facial recognition
- **Unsupervised front-line models**: definitive fraud and abuse detection
- **Goal-driven front-line optimisation**: (hypothetical) dynamic clinical treatment policy personalised to patient characteristics and needs and real-time diagnostics, simulations appraising efficacy of a service provider’s intervention
- **Front-line generative AI**: (hypothetical) risk profiling from trawling big data (call transcripts, client documents and assessments). **Should not be used in front-line without intrinsic, faithful explanations of its inferences.**

**Challenges**:
- **Accountability** – government decisions can be reviewed by **dedicated independent reviewers** (e.g. Benefit Review Committee for MSD benefit decisions). If such a channel is unavailable, the **Ombudsman** may also investigate decisions and actions, who may report back to the agency if they find a decision to be contrary to law, unreasonable, unjust, oppressive, improperly discriminatory, a mistake or wrong. Decisions and actions made under a specific legal power are also judicially reviewable, where the **High Court** assesses if actions were undertaken within the constraints of the law (e.g. algorithm’s consistency with legislation). In any case, an oversight body will require a sufficient degree of explanation as to how a decision was reached.
- **Transparency** – any front-line decision made by an AI regarding an individual must be logically explainable linking the requestor’s data (“material issues of fact”) with every step of reasoning to the conclusion (“the reasons for the decision”). This requirement rules out many non-intrinsic explainable AI methods that rely on apparent or likely reasons, or post-hoc rationalisations of opaque reasoning. Prompt engineering techniques like chain-of-thought reasoning simply imitate statistically likely reasoning and does not provide a trace of the actual computations that led to the decision.  Furthermore, without intrinsic explanation, developers cannot eliminate the risk of the use or unintentional inference of protected attributes that should never be considered in a decision. No mainstream GenAI tool rendering its own conclusions independently can provide such faithful explanations that may be required under OIA s23.

</div>
</div>


<div class="box" id="box-5-2-2">
<div class="box__header"><span class="box__number">Box 5.2.2</span><h3 class="box__title">Research</h3></div>
<div class="box__body" markdown="1">

Algorithms and AI that generate data that support decision-making at the system level or are involved in intervention development itself. These models do not need to be tied to a specific intervention; this category includes models generating routine data that measures the general impact of policy. This category also excludes the use of AI tools outside of evidence generation. For example, using generative AI for the general collation of research automates part of the routine operations of staff, and is thus administrative in nature.

Here, data from individuals are used in aggregate. The Privacy Act allows the use of already collected personal information for statistical or research purposes if individuals cannot be reasonably identified from the outputs of the research. This exception also enables research techniques like the Integrated Data Infrastructure and synthetic data to be used outside the purpose of collection, if confidentiality can be guaranteed.

Outputs of these systems form part of the evidence base for system-level decisions. Thus, governance around such systems is primarily to assure robust and impartial advice is given to those who make these decisions (e.g. Ministers, Crown agent boards, management). Nevertheless, other ongoing capability maintenance and other risk controls like QA will still be necessary to ensure human-factor risks remain low.

**Examples**:
- **Research algorithms:** rules-based qualitative coding, CBAx cost-benefit analysis,
- **Supervised models**: StatsNZ net migration nowcasting, building consent data automated coding; Reserve Bank GDP nowcasting proof-of-concept
- **Unsupervised research models**: clustering cohorts of interest to target interventions
- **Goal-driven optimisation research models**: MoT’s Monty simulation (co-evolutionary computation), PHF Science’s ALMA digital twin (large population model), MoE school bus route optimiser (possibly traditional combinatorial optimisation)
- **Research large language models**: thematic analysis of qualitative data like customer feedback and statutory consultation, orchestrating LLMs that perform analysis and predictions.

**Challenges**:
- **Transparency of models:** Requests for this information are handled by the more general section 12, where information can be withheld by any exemption. Objective data and evidence generally are not withheld to the same extent as advice and opinion.
- **Trustworthy policymaking**: The subject matter surrounding research AI may be conceptually inaccessible to the public, if not inaccessible due to conclusive or good withholding grounds. Citizens, and accountable decision-makers who also may not have the same degree of expertise, place a unique trust in these specialists to provide “comprehensive, objective and balanced” policy advice (as characterised by DPMC). Given the reduced accessibility, increased breadth of impact, and the presence of context-agnostic technical challenges from Section 4, fostering public trust in research AI should still be sought through robust quality assurance processes and disclosure.

</div>
</div>


<div class="box" id="box-5-2-3">
<div class="box__header"><span class="box__number">Box 5.2.3</span><h3 class="box__title">Administration</h3></div>
<div class="box__body" markdown="1">

Algorithms and AI that automate (or otherwise significantly support) core functions of government staff in routine operations that does not otherwise have a direct effect on individual’s rights or interests. The execution of administrative systems is still critical to operational integrity and requires performance monitoring to minimise risk. A function is only considered ‘core’ if its performance is fundamental to the output of a human-equivalent role. For example, a legal advisor may require performance improvement if they are consistently unable to correctly identify, interpret and summarise facts and case law, but will not for incidental issues like spelling mistakes, poor meeting transcripts, or unengaging presentation visuals. Reapplying this analogy brings document summarisation in scope, but spell check, meeting transcription and media generation out. This definition is fundamentally risk-based and self-assessed; it is up to agencies and their risk appetite to determine whether a system is worth monitoring.

**Examples**:
- **Administrative algorithms**: business rules e.g. customer relationship management, internal enterprise rules e.g. payroll calculation, document classification as per Protective Security Rules
- **Supervised administrative models**: DOC object identification in aerial camera imagery, MPI face redaction and event flagging in fishing vessel footage, StatsNZ automated coding in building consents data
- **Unsupervised administrative models**: fraud and abuse event flagging, where no definitive decision is made
- **Administrative generative AI**: customer service chatbots, assistive web search, customer call transcription, customer call real-time knowledge discovery, document creation e.g. policy documents, business processes.

**Challenges**: as for the specific type of algorithm used, e.g. varying degrees of automation bias by technique; user acceptance testing is still advisable. Use of these kinds of AI may still be contentious with the public, e.g. staff rigidly following AI recommendations without an element of human discretion, so process controls remain relevant.

</div>
</div>

## Action: Overlay the technical and contextual categorisation to refine algorithm and AI guidance

Other jurisdictions like the EU and Canada, as well as the current Algorithm Charter, take a risk-based approach to classifying algorithms and AI. New Zealand’s approach has been criticised as being too flexible to be useful, relying on agencies to self-rate the material impact of algorithms while providing little guidance in terms of precedent. More useful taxonomies have been developed by organisations like the OECD. Their Framework for the Classification of AI Systems[^29] provides 31 different criteria for classifying AI systems grouped into 5 dimensions. While this may be appropriate in the international, sector-cutting environment the OECD operates in, much of the criteria can be answered similarly – some not even relevant – for any application in government.

{% include diagrams/figure3-4-matrix.html %}

> _Figure 4: Diagram overlaying the technical categories outlined in Section 4 (symbolic AI, supervised learning, unsupervised learning, goal-driven optimisation and generative AI) with the contextual categories outlined in Section 5 (front-line, research, and administration)_

A two-way technical-contextual taxonomy, as illustrated by Figure 3, provides enough practical specificity relevant for monitoring and governance in the New Zealand context. One axis dives into just enough technical detail such that similar monitoring and evaluation approaches exist within a category. The other axis is rooted in the legislative context that the system will operate in. When new technologies emerge, guidance across the contextual axis should already exist to help agencies navigate their existing legal obligations, creating an environment where agencies can safely innovate. Appendix 2 illustrates how this taxonomy can be used to categorise existing and potential AI use cases, providing a visual way to conceptualise how AI is and can be used in Government.


## References

[^26]: StatsNZ, Algorithm Assessment Report, (2018). [https://data.govt.nz/toolkit/data-ethics/government-algorithm-transparency-and-accountability/algorithm-assessment-report](https://data.govt.nz/toolkit/data-ethics/government-algorithm-transparency-and-accountability/algorithm-assessment-report)
[^27]: Department of Internal Affairs, AI use in Public Services and key opportunities for the system, Proactive release of material relating to Artificial Intelligence in the month of July (2024). [https://www.dia.govt.nz/diawebsite.nsf/Files/Proactive-Releases-2024-25/$file/Proactive-release-of-material-relating-to-Artificial-Intelligence-in-the-month-of-July.pdf](https://www.dia.govt.nz/diawebsite.nsf/Files/Proactive-Releases-2024-25/$file/Proactive-release-of-material-relating-to-Artificial-Intelligence-in-the-month-of-July.pdf)
[^28]: John Zerilli, Alistair Knott, James Maclaurin & Colin Gavaghan, December 2019. Algorithmic Decision-Making and the Control Problem. [https://link.springer.com/article/10.1007/s11023-019-09513-7](https://link.springer.com/article/10.1007/s11023-019-09513-7)
[^29]: Organisation for Economic Cooperation and Development, OECD Framework for the Classification of AI systems, 2022. [https://www.oecd.org/en/publications/oecd-framework-for-the-classification-of-ai-systems_cb6d9eca-en.html](https://www.oecd.org/en/publications/oecd-framework-for-the-classification-of-ai-systems_cb6d9eca-en.html)
