---
layout: section
title: Guidance must acknowledge different requirements across different use cases AI is applied in
short_title: 5. Use Cases
section_number: Section 5
description: "Contextual taxonomy: front-line, research, and administrative AI use cases."
---
This use case is not hypothetical, as agencies such as the Ministry of Transport use GDO (co-evolutionary algorithms) to simulate changes in traveller behaviour in response to a given transport system intervention. Vendors like PHF Science have developed new GDO models that lower the computational barriers to precisely and representatively simulate five million New Zealanders and their reactions to interventions.

Promoting effective and trustworthy AI use and decision-making with GDO requires system-wide coordination, as multiple agencies contribute data to these models and explore their use in isolation. Issues that a system lead agency can address include:

- Source data improvements: simulation actors are trained by replicating patterns from historical data and often rely on data sources that the interested agency does not collect, such as StatsNZ’s Census data. The impending redevelopment of StatsNZ’s census and survey programme presents a timely opportunity to consider how effective existing data sources are in simulations and GDO, and which new (or extensions to existing) datasets can have the greatest impact for a wide range of user agencies.

- Streamlining procurement: agencies currently commission bespoke GDO solutions tailored to their needs. The vendor market could be evaluated to see if vendor(s) can meet a wide range of agencies' requirements by offering domain-agnostic models that provide flexibility across agencies’ data and operational environments without creating bespoke model architectures for each use case.

- Encouraging use cases: existing communities of practice and networks can more intentionally promote this category of AI, which is currently limited to agencies responsible for explicit system design, such as the transport system. Any agency can reconceptualise their operations – or even policy remit – as an explicit system to be simulated, such as customer journey optimisation or regulatory impact management, with greater detail than traditional coarse appraisal models like Treasury’s CBAx.

> ML models predict to decide, generative models mimic to create, GDO models simulate to solve. GDO is already being used by agencies like MoT. System leadership can promote use and streamline development of GDO models.

# Guidance must acknowledge different requirements across different use cases in which AI is applied

All-of-Government stocktakes in 2018 and 2024 have demonstrated the wide variety of ways that agencies already use or plan to use AI. The 2018 Algorithm Assessment Report clearly distinguished three different types of algorithms, consistent with my definition: operational algorithms, algorithms used for policy development and research, and business rules. This categorisation offers a useful contextual distinction between the aims of each kind of algorithm. Operational algorithms make or recommend complex decisions about individual users of government services. Policy algorithms make or recommend policy decisions that intervene at the aggregate system level. Business rules automate routine administrative processes without applying the same level of individual discretion as more advanced algorithms.

Six years later, the 2024 cross-agency survey of AI use cases adopted a different theming approach rather than the previous systematic taxonomy. While this theming was useful to illustrate the different uses of AI in the public sector, it is not scalable given its focus on specific objectives, such as “boosting productivity and efficiency” and “enhancing customer experience”.

The 2024 survey also did not prompt agencies to consider different types of techniques; it only asked them to report on “AI use cases”. This flaw in survey design has caused agencies to underreport the AI they use. For instance, only one AI use case was recorded by StatsNZ in the survey. However, traditional machine learning modelling has been used for official statistics, such as the International Migration provisional dataset, since 2018, generating highly publicised metrics for policy impact, like net migration. Use cases in ACC identified in [Section 4](../04-section4/), recognised in the 2018 survey, were not disclosed in the 2024 survey. Including them would have highlighted an AI use case that has clearly provided financial benefits to ACC, improved the experience for injured people navigating the system, and followed best practice. A clearer systematic definition of AI could enhance coverage of all kinds of AI use cases across government and highlight low residual risk, high-impact examples already integrated into agencies’ day-to-day operations.

## 5.2 Action: A new taxonomy should differentiate between the different legal obligations associated with different use cases {#s5-2}

A systematic taxonomy can ground AI standards and guidance on the specific considerations of the context in which AI is used. Below, I propose a new taxonomy that builds on the 2018 categorisation to accommodate technologies that have emerged since then.

- Operational algorithms now belong to the **“frontline”** category of techniques, which includes both algorithms and GenAI that directly and independently make decisions or recommendations regarding an individual that affect their rights or interests.

- Algorithms for policy development and research should also incorporate operational research using algorithms and AI, classified under the **“research”** category. This group encompasses both operational and policy research techniques that produce data to establish the evidence base for system-level decision-making.

- Most business rules and generative AI tools now fall into the **“administration”** category of techniques, which do not directly lead to a definitive decision but still have a significant impact. They may utilise personal data, subjecting it to the Privacy Act.

{% include figure.html id="FIGURE_5" src="" caption="" type="decorative" %}

> _Figure 3: Taxonomy of use cases based on the relevant legal obligations within each category. Operational algorithms and any conclusive algorithm or GenAI are grouped into frontline. Evidence-generating algorithms and AI are grouped into research. Impactful but non-conclusive algorithms and GenAI are grouped into administration._

As in the previous section, I propose new definitions for these three categories, rooted in the relevant legal obligations associated with each, along with examples and the unique challenges each faces. Applications inherit challenges from the intersection they form with the technical taxonomy (e.g. all three contextual categories are susceptible to learning biases when developing supervised learning models).

> Frontline AI directly makes decisions or recommendations around a user of government services, research AI generates evidence to inform system-level decisions, administrative AI support or automate the role of staff.


<div class="box" id="box-5-2-1">
<div class="box__header"><span class="box__number">Box 5.2.1</span><h3 class="box__title" id="box-5-2-1-h">Frontline</h3></div>
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
Research

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
- **Trustworthy policymaking**: The subject matter surrounding research AI may be conceptually inaccessible to the public, if not inaccessible due to conclusive or good withholding grounds. Citizens, and accountable decision-makers who also may not have the same degree of expertise, place a unique trust in these specialists to provide “comprehensive, objective and balanced” policy advice (as characterised by DPMC). Given the reduced accessibility, increased breadth of impact, and the presence of context-agnostic technical challenges from [Section 4](../04-section4/), fostering public trust in research AI should still be sought through robust quality assurance processes and disclosure.

</div>
</div>


<div class="box" id="box-5-2-2">
<div class="box__header"><span class="box__number">Box 5.2.2</span><h3 class="box__title" id="box-5-2-2-h">Administration</h3></div>
<div class="box__body" markdown="1">

Algorithms and AI that automate (or otherwise significantly support) core functions of government staff in routine operations that does not otherwise have a direct effect on individual’s rights or interests. The execution of administrative systems is still critical to operational integrity and requires performance monitoring to minimise risk. A function is only considered ‘core’ if its performance is fundamental to the output of a human-equivalent role. For example, a legal advisor may require performance improvement if they are consistently unable to correctly identify, interpret and summarise facts and case law, but will not for incidental issues like spelling mistakes, poor meeting transcripts, or unengaging presentation visuals. Reapplying this analogy brings document summarisation in scope, but spell check, meeting transcription and media generation out. This definition is fundamentally risk-based and self-assessed; it is up to agencies and their risk appetite to determine whether a system is worth monitoring.

**Examples**:
- **Administrative algorithms**: business rules e.g. customer relationship management, internal enterprise rules e.g. payroll calculation, document classification as per Protective Security Rules
- **Supervised administrative models**: DOC object identification in aerial camera imagery, MPI face redaction and event flagging in fishing vessel footage, StatsNZ automated coding in building consents data
- **Unsupervised administrative models**: fraud and abuse event flagging, where no definitive decision is made
- **Administrative generative AI**: customer service chatbots, assistive web search, customer call transcription, customer call real-time knowledge discovery, document creation e.g. policy documents, business processes.

> **Challenges**: as for the specific type of algorithm used, e.g. varying degrees of automation bias by technique; user acceptance testing is still advisable. Use of these kinds of AI may still be contentious with the public, e.g. staff rigidly following AI recommendations without an element of human discretion, so process controls remain relevant.

</div>
</div>
