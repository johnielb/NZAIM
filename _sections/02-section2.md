---
layout: section
title: The Algorithm Charter has yet to develop into the world-class framework that it could be
short_title: 2. Algorithm Charter
section_number: Section 2
description: Analysis of the Algorithm Charter's shortcomings and recommended improvements.
---
# The Algorithm Charter has yet to develop into the world-class framework that it was set to become

I argue that, at the time, Minister James Shaw rightfully described the Algorithm Charter as a world first. Back then, only the Government of Canada (GC) had comparable provisions in this space. The GC’s Directive on Automated Decision Making (DADM) offers less detailed but more practical guidance for managing automated algorithms. It uses the same concrete language as the enterprise processes that operationalise it, giving agencies actionable advice:

- Like the Charter, the DADM requires an explanation of decisions. However, the DADM goes further by outlining what a sufficient explanation looks like

- Like the Charter, the DADM requires human oversight of decisions. However, the DADM recognises that lower-impact algorithms may not need direct human involvement.

- Like the Charter, the DADM requires peer review. However, the DADM goes further by specifying which levels of impact require peer review and which experts are qualified to conduct it, with required expertise increasing as potential impact increases.

On the other hand, New Zealand’s Charter was generally seen as an effort to promote public trust rather than as an impact control framework for the GC. Therefore, New Zealand’s approach encompassed a broader range of normative commitments:

- Active engagement with communities impacted by the algorithm’s use, which the Charter explicitly calls for. This principle is present only in the GC framework when the need arises in an impact assessment.

- Impacted communities may also have Treaty interests, with the Charter calling for embedding an indigenous perspective in the development and use of algorithms. Indigenous-considerate development is not required in the GC framework.

In the age of generative AI, whose capacity to generate “unknown unknowns” challenges established risk methodologies that rely on knowing unknowns and controlling them, AI governance can no longer rely solely on this method. It also needs a normative framework that offers guiding principles to shape the acceptable use of AI systems: one that aims to maximise public benefit and uphold public trust, rather than just minimise the residual risk posed by AI systems to citizens. Given New Zealand’s relatively low trust in AI and declining trust in government, a trust-enhancing approach to AI system delivery is even more critical.

However, normative frameworks cannot replace organisational methodologies—they must support and inform them. The practical challenge of implementing the Charter’s norms was highlighted in the Year 1 Review of the Algorithm Charter by Taylor Fry (2021). Nonetheless, this review confirmed the Charter's overall intent and approach.

> The normative commitment to enhance public trust embodied by the Algorithm Charter are more important than ever in the age of generative AI, declining public trust in government, and low public trust in AI relative to global peers.

## 2.1 Action: Fold Algorithm Charter improvement work into the Public Service AI work programme {#s2-1}

Operationalising Year 1 Review findings has been challenging, with recommendations only partly implemented. [Table 5](#table-5) monitors the progress of the considerations identified in the review, excluding those that simply confirm the current direction. Of my seven groups of considerations, only two have been completed. Two show progress mainly driven by efforts outside of the system lead agencies. Three show no publicly available evidence of progress.

<a id="table-5"></a>

| Done? | Grouping of actionable consideration(s) in Taylor Fry (2021) | Progress as of January 2025 |
| --- | --- | --- |
| ☑️ | Maintain a risk-based approach with supplementary tools for risk assessment and further clarifying guidance that acknowledges the value of algorithms. | Completed in December 2023 with the release of the AIA toolkit, with the Algorithm Threshold Assessment and AIA user guide respectively filling the gaps. |
| ☑️ | Facilitate a community of practice to share use cases captured in the Charter. | BAU – meets quarterly but no public updates since September 2023. |
| ➡️ | Consider working with Māori data experts to develop more detailed guidance, best practice on partnering with Māori, clarify working with existing consultation groups, sharing knowledge with other agencies given limited expert capacity in this area. | Te Kāhui Raraunga has independently developed the Māori AI Governance model. In the same report, **they call for an urgent overhaul to the Algorithm Charter** to align with their model. |
| ➡️ | Detailed technical resources for measuring bias and ensuring human oversight of algorithm outputs. | For traditional machine learning, MSD’s Model Development Lifecycle is sufficiently detailed, and the AIA toolkit mentions this. No equivalent technical resources relevant to generative AI exists, but the GCDO is working on an AI assurance model. |
| ❌ | Investigate novel forms of citizen participation and measuring public trust and confidence in algorithm use. | The [Digital Council report](https://www.toiaria.org/our-projects/towards-trustworthybrand-trusted-automated-decision-brmaking-aotearoa/) investigating this for automated decision-making was shelved and the Digital Council was dissolved. DPMC’s [PCET](https://www.dpmc.govt.nz/publications/policy-community-engagement-tool) may be relevant. |
| ❌ | Consider the creation of an oversight body for the Charter. | No public knowledge of consideration. GCDO has appointed an AI Expert _Advisory_ Panel, but it does not have any oversight powers. |
| ❌ | Develop an annually updated algorithm register. | The GCDO has committed to a central AI register by 2027. |
{:.table-status}

> _Table 5: Actionable considerations identified in the year 1 review of the Algorithm Charter. "Actionable" excludes passive considerations that recommend maintaining current direction. From Taylor Fry, 2021. Algorithm Charter for Aotearoa New Zealand Year 1 Review. [https://www.data.govt.nz/assets/data-ethics/algorithm/Algorithm-Charter-Year-1-Review-FINAL.pdf](https://www.data.govt.nz/assets/data-ethics/algorithm/Algorithm-Charter-Year-1-Review-FINAL.pdf)_
{: .bq--caption}

Over the same period, the GC has adopted a relatively proactive approach to maintenance, completing four reviews of the DADM. Two of these reviews were conducted in the generative AI era following the release of ChatGPT. Like New Zealand, the GC has issued specific guidance on the use of generative AI. However, unlike New Zealand’s guidance, their GenAI guidance clearly separates it from existing algorithmic guidance. The GC’s guidance also offers advice on the most suitable contexts for applying these techniques. [Section 3](../03-section3/) of this report evaluates the progress of the New Zealand Government’s generative AI guidance.

> While Canada has kept its government automated decision-making guidance up-to-date and integrated with new generative AI guidance, New Zealand’s algorithmic guidance has not kept up.

## 2.2 Action: Conduct an evaluation of the AIA toolkit with a view to folding it into the NZAIM {#s2-2}

The AIA toolkit represents the most significant advancement in all-Government AI policy since the Algorithm Charter, turning high-level commitments into tangible actions. Its first tool, the algorithm threshold assessment (ATA), addresses a major criticism by clarifying the scope of systems covered by the Charter. The ATA’s “material impact” test aligns with, but is broader than, the Ombudsman’s interpretation of “personal capacity” in the OIA.

However, no review of the two-year-old AIA toolkit has been announced, despite technological advances, public service AI policy development, and public service AI adoption. Its author, Frith Tweedie, recently joined the GCDO's AI Expert Advisory Panel, indicating better alignment between GCDO and GCDS work programs.

Issues that a review of the AIA toolkit may explore include:

- Evaluating the effectiveness of the toolkit among end users, including the communication and engagement around this tool. Currently, no published AIAs exist for any agency. Agencies that have implemented AI tools have only carried out PIAs.

- Incorporating the Māori AI Governance model throughout the toolkit, not just through _Partnership with Māori_. For example, Question 6.3 (Storage) addresses jurisdictional issues but should also consider iwi Māori interests in onshoring data to bolster control. No Māori data experts were acknowledged for providing feedback on the original AIA.

- How it interacts with technical guidance instruments. For example, the use guide relies on MSD’s Model Development Lifecycle for technical guidance, such as defining a model’s accuracy. However, the MDL has not been updated since October 2021. Thus, it lacks technical guidance on newer techniques such as GenAI. A new NZAIM should serve as the definitive technical instrument, under which an impact assessment process sits alongside other universal processes, such as an AI-specific certification and accreditation process.

- How it interacts with strategic instruments. Given that the privacy impact assessment toolkit organises its risks around the information privacy principles, risks identified by the AIA may be similarly organised under the PSAIF principles.

> The AIA toolkit is the strongest AI guidance instrument the Government currently maintains, but it must be evaluated to understand why no agencies have published a worked example in its two years of existence.

## 2.3 Action: Promote publication of algorithm threshold and impact assessments to data.govt.nz, creating a register that establishes implicit accountability {#s2-3}

The Taylor Fry review found that public reporting of each agency’s use of algorithms, as recommended under the Transparency commitment of the Charter, was “fragmented and incomplete” in 2021. As of December 2025, a site-specific search for “algorithm” on each Charter signatory’s website yielded only one example of a self-reported agency-wide stocktake: the Ministry of Justice. agencies do make certain algorithm and AI assessments available, often in response to OIA requests regarding the Charter. However, consolidated information should already exist for agencies that responded to government-wide stocktakes conducted by system lead agencies for the 2018 algorithm assessment report[^10] and the 2024 cross-agency survey on AI[^11]. Consolidated information on high-impact algorithms (i.e. algorithms that “must” follow the Charter) should already exist within agencies’ enterprise risk registers.

Proactive transparency about AI use acts as a low-effort mechanism of implicit accountability when legal enforcement is absent. An all-of-government register has been recommended since Gavaghan et al. (2019) and the Taylor Fry evaluation. This register can help spread best practices in tackling common challenges by sharing impact controls used in such cases. Such a register also creates a soft compliance dynamic, with agencies that do not report signalling lower governance maturity, thereby encouraging remediation as a form of reputational risk management. Comprehensive reporting on the use of algorithms and AI can also build public trust by clearly indicating where these systems are used and where they are not. Importantly, such a register can be developed without revealing sensitive details. At a minimum, a register should disclose:

- Basic context regarding when, where, and for what purpose the algorithm is used.

- Answers to the questions in the algorithm threshold assessment.

- If ATA’s threshold is met, specify when and who (job title or qualification sufficient) conducted the latest peer review to evaluate potential unintended consequences and how they responded to this information, or justify why a review has not been recently performed (e.g. static legislation and environment minimise risk of concept drift).

In this regime, information may still be justifiably withheld in accordance with the OIA. However, the public can be assured that a separate expert found the algorithm to be, at a minimum, technically and legally compliant. A peer review can offer assurance regarding the lawfulness of decision-making subject to judicial review, in accordance with its establishing legislation and the broader legislative framework previously mentioned. A peer review may also examine alignment with the Charter's non-mandatory commitments. The AIA toolkit already provides a sufficiently comprehensive framework to organise such a peer review.

In Canada, the DADM mandates transparency by requiring the publication of algorithmic impact assessments on the federal Open Government Portal. This website uses CKAN, which also powers New Zealand’s data.govt.nz dataset catalogue, maintained by the GCDO. It is straightforward to add an “Algorithm” or “AIA” tag within data.govt.nz to emulate Canada’s ADM register. Agencies already have procedures and APIs for uploading content to this portal.

> Data.govt.nz can already be used to create a minimum viable self-reported register of algorithm and AI use across government with little additional work, given agencies should already know the necessary information.

## 2.4 Action: Refactor the Algorithm Charter as an extension of DPUP: normative values for AI system delivery to follow {#s2-4}

Both the Charter and the DPUP fulfil closely related functions. Each articulates expectations for the use of data and algorithms that extend beyond existing obligations, with the aim of promoting public trust through their respectful and safe use. However, each fall short in ways that the other compensates for. Taylor Fry (2021) observed that the Charter lacks clarity around the practical implementation of its commitments to partnership and community engagement. The subsequent AIA toolkit now points to DPUP for guidance in these areas. On the other hand, DPUP lacks the formal mandate of other standards, or, in the case of the Charter, publicly recorded voluntary commitment by agencies. DPUP has been employed by agencies implementing AI outside of its original remit in the social sector, such as ACC.[^12]

In recognising their similarity, compliance can be streamlined by refactoring[^13] the normative Charter commitments as a function of DPUP. The Charter commitments of partnership and people overlap with the Manaakitanga principle of DPUP, which goes into greater detail around how to engage communities with a view to upholding their dignity and mana. The Charter’s call to “deliver clear public benefit” is given greater emphasis under the He Tāngata principle in DPUP, which promotes a focus on improving people’s lives. The He Tāngata principle provides a clearer constraint on what AI systems should optimise for, prioritising life outcomes over other definitions of public benefit, such as naïve fiscal optimisation.

A streamlined, enforceable DPUP will emphasise the fundamental, foundational nature of GCDS guidance centred on maintaining public trust in the use of information. Trustworthy use of any information technology does not happen without the trustworthy use of the information that communities entrust to agencies. Conversely, comprehensively trustworthy use of this information begets the trustworthy use of any novel information technology, provided that suitable engagement and evaluation mechanisms are already in place. Trustworthiness can be demonstrated by technical practitioners by ensuring safety, effectiveness, and accountability. However, systems can demonstrate all three without being trustworthy if their use is fundamentally inappropriate. Appropriateness is DPUP’s reason for being: by describing “what doing the right thing looks like”. Technical practitioners alone rarely possess the capability or institutional authority to set such cultural expectations for respectful data practice and to sustain active, meaningful community engagement. Setting cultural expectations requires an explicit whole-of-agency commitment and support, sponsored by a single organisational leader to steward best practice – regardless of whether data is used by algorithms, AI, or humans directly. A unified all-of-government policy provides a coherent structure to support agencies in developing and sustaining such a trustworthy data culture.

A consolidation of GCDS policy also provides an opportunity to consider other pending work:

- How to promote Ngā Tikanga Paihere as general advice for the wider data system, not just projects within the Integrated Data Infrastructure: as a function of DPUP+.

- Consolidating practical advice on Māori engagement and citizen participation, building on existing all-of-government initiatives like the DPMC’s Policy Project[^14], and previous technology-specific research by Toi Āria[^15] and Te Kāhui Raraunga[^16].

- How compliance with GCDS guidance is assessed within implementing agencies, in lieu of legislative, Cabinet or voluntary enforcement. Another potential mechanism is a standardised data maturity assessment, through which agencies are evaluated, directly associating a trustworthy, respectful data culture with high performance. It is unclear how or if the GCDS currently assesses organisational data maturity.

After streamlining normative commitments, what remains of the Algorithm Charter comprises operational obligations that are already mandated by legislation and standards and thus are best clarified in the NZAIM. Transparency around algorithmic decision-making is largely compulsory under the OIA. Failing to ensure and regularly review the fitness of data and algorithms constitutes poor professional practice and exposes agencies to material risk. Privacy and the human right to non-discrimination (through bias mitigation) are safeguarded by existing laws. Accordingly, these residual commitments are largely addressable through technical controls rather than requiring standalone normative commitments.

> The GCDS maintains a range of normative best practice on specific systems (algorithms, IDI) which are largely applicable to any data use. All guidance promoting a trustworthy, respectful data culture can be consolidated into DPUP.


## References

[^10]: StatsNZ, 2018. Algorithm assessment report. [https://data.govt.nz/toolkit/data-ethics/government-algorithm-transparency-and-accountability/algorithm-assessment-report](https://data.govt.nz/toolkit/data-ethics/government-algorithm-transparency-and-accountability/algorithm-assessment-report)
[^11]: Department of Internal Affairs, October 2024. Proactive release of material relating to Artificial Intelligence in the month of July. [https://www.dia.govt.nz/diawebsite.nsf/Files/Proactive-Releases-2024-25/$file/Proactive-release-of-material-relating-to-Artificial-Intelligence-in-the-month-of-July.pdf](https://www.dia.govt.nz/diawebsite.nsf/Files/Proactive-Releases-2024-25/$file/Proactive-release-of-material-relating-to-Artificial-Intelligence-in-the-month-of-July.pdf)
[^12]: ACC, March 2025. ACC Privacy Impact Assessment (PIA) - Agent Copilot. [https://www.acc.co.nz/assets/corporate-documents/Privacy-Impact-Assessment-Agent-Copilot.pdf](https://www.acc.co.nz/assets/corporate-documents/Privacy-Impact-Assessment-Agent-Copilot.pdf)
[^13]: Reorganising text (typically software code) to improve readability and reusability without affecting its function.
[^14]: Department of Prime Minister and Cabinet, October 2023. Policy Community Engagement Tool. [https://www.dpmc.govt.nz/publications/policy-community-engagement-tool](https://www.dpmc.govt.nz/publications/policy-community-engagement-tool)
[^15]: Digital Council for Aotearoa New Zealand, 2020. Towards trustworthy and trusted automated decision-making in Aotearoa. [https://www.toiaria.org/our-projects/towards-trustworthybrand-trusted-automated-decision-brmaking-aotearoa/](https://www.toiaria.org/our-projects/towards-trustworthybrand-trusted-automated-decision-brmaking-aotearoa/)
[^16]: As outlined in [Table 4](../01-section1/#table-4).
