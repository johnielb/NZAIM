---
layout: section
title: Rules and best practice in NZ for algorithm and AI system delivery are currently fragmented
short_title: 1. Fragmented Guidance
section_number: Section 1
description: Overview of the fragmented legal and guidance landscape for AI in New Zealand government.
---
# Rules and best practice in NZ for algorithm and AI system delivery are currently fragmented across different laws and guidance

Deployers of AI systems in government face a complex maze of laws, principles, standards, and guidance to deploy AI safely and effectively. This approach can be advantageous, as broad rules address long-lasting risks or support enduring objectives – rules relevant regardless of context or technology. Specific rules are created by specialised entities with the expertise to manage certain risks or achieve certain objectives. [Figure 1](#figure-1) depicts this guidance ecosystem as a layered pyramid, with higher-level instruments becoming more technically specific, while guidance in instruments below it remains applicable. Following guidance at all levels is essential to maximising the benefits.

This fragmentation becomes problematic when each specialist entity develops its own framework, toolkit, or checklist for AI, often with overlapping elements. This issue worsens for implementing agencies, which must interpret the various rules and tools and incorporate these frameworks into their policies. While this integration can help tailor governance to each agency’s operational environment, a lack of a common scope and framework leads to inconsistent recordkeeping across agencies. This inconsistency makes it harder for the public –including academia and the media – or even a government system leader, to understand AI use across the government.

<div id="figure-1">{% include diagrams/figure1-current-pyramid.html %}</div>

Figure 1: Current hierarchy of laws, standards, principles, and guidance that inform the use of information, information technology, algorithms, and AI systems, coloured by the type of instrument, and outlined if the instrument is maintained by a system leader. Following guidance in all layers is essential to fully realise its benefits.

## 1.1 **Generic legislation** mandates broad obligations on the use of AI, like transparency, privacy and information provenance {#s1-1}

As previously discussed, generic legislation establishes lasting rules that persist regardless of context or technology. Three such acts serve as technology-neutral mechanisms that address specific risks through principles or rights-based regulation. The Official Information Act 1982 mitigates government opacity and promotes good decision-making and behaviour through freedom of information mechanisms ([Box 1.1.1](#box-1-1-1)). The Privacy Act 2020 mitigates unauthorised and harmful collection, use, and disclosure of personal information, which infringes on individuals' rights to privacy ([Box 1.1.2](#box-1-1-2)). The Public Records Act 2005 mitigates the erosion of accountability caused by poor and incomplete record-keeping ([Box 1.1.3](#box-1-1-3)). Together, this ecosystem provides a stable regulatory baseline for democratic accountability. This baseline endures regardless of the technology in use and therefore applies to AI systems.


<div class="box" id="box-1-1-1">
<div class="box__header"><span class="box__number">Box 1.1.1</span><h3 class="box__title" id="box-1-1-1-h">Official Information Act 1982 (OIA)</h3></div>
<div class="box__body" markdown="1">

Promotes government transparency and accountability, requiring all public service agencies to provide anyone in New Zealand with information the government holds. Sections 22 and 23 promote good government decision-making by providing anyone in New Zealand (including businesses) the right to know, respectively:
- **How** a decision (including recommendations) was made: the **right** to access rules affecting decisions that can affect **anyone’s** rights or interests. Any document (including electronic information) that contains such rules can be requested. [a]
- **Why** a decision (including recommendations) was made: the **right** to access the reasons for decisions that affect the **requestor’s** rights or interests. [b]

The Act specifies valid reasons for withholding this information. s6 outlines conclusive withholding grounds, while s9 outlines other withholding grounds that must outweigh the public interest in making information available. As these are **rights**, fewer s9 withholding grounds apply to rules/reasons requests. s18, which outlines grounds for refusing requests, do not apply to rules/reasons requests.

Requestors affected by general decisions, such as policy decisions, cannot use s23 to determine the reasons for such a general decision where it does not uniquely affect their own rights or interests. This information may be requested under a normal section 12 request, subject to other potential withholding grounds, such as free and frank opinions. [b]

A response to a s23 request must include:
- the findings on material issues of fact (the data, evidence and inferences used to support a decision)
- where those findings originated (not necessarily the documents themselves, but it is more administratively efficient to include them if they are requestable)
- a logical explanation of the reasoning that links such facts to the conclusion, not just the conclusion itself – an approximate or post-hoc explanation is insufficient

These provisions are closely coupled with that of the **Ombudsman Act 1975** enabling the Ombudsman to investigate most government actions or decisions as contrary to law; unreasonable, unjust, oppressive, or improperly discriminatory; a mistake; or wrong.

For AI use in government, OIA ss 22 and 23 serve as the most significant constraint. Agencies that deploy AI that cannot faithfully explain personally impactful decisions deprive people of their right to information contravening the OIA. Unexplainable AI may still be used outside of making conclusive personally impactful decisions. [Section 5](../05-section5/) elaborates on the different degrees of compliance required for different uses of AI systems.

**Further reading**: [a] [Requests for internal decision making rules: A guide to section 22 of the OIA and section 21 of the LGOIMA - Ombudsman New Zealand - May 2019](https://www.ombudsman.parliament.nz/resources/requests-internal-decision-making-rules-guide-section-22-oia-and-section-21-lgoima) and [b] [Requests for reasons for a decision or recommendation: A guide to section 23 of the OIA and section 22 of the LGOIMA - Ombudsman New Zealand - May 2019](https://www.ombudsman.parliament.nz/resources/requests-reasons-decision-or-recommendation-guide-section-23-oia-and-section-22-lgoima) and [c] [AI systems and OIA section 22 and 23 - Ombudsman query - Johniel Bocacao - February 2026](https://fyi.org.nz/request/33209-ai-systems-and-oia-section-22-and-23?post_redirect=1)

</div>
</div>


<div class="box" id="box-1-1-2">
<div class="box__header"><span class="box__number">Box 1.1.2</span><h3 class="box__title" id="box-1-1-2-h">Privacy Act 2020</h3></div>
<div class="box__body" markdown="1">

Promotes the human right to privacy by requiring any holder of a person’s information (not just a government agency) to follow these information privacy principles (IPPs), notwithstanding exceptions elsewhere in the Act.
- Collection of personal information has a lawful and necessary purpose (1), is collected from the individual where possible (2) who understands why it is collected (3), and is done in a lawful and reasonably unintrusive manner (4)
- Personal information is stored and secured against loss, and unauthorised access (5)
- Individuals have the **right** to access (6) and correct (7) information about them.
- Information is checked as accurate before use or disclosure (8)
- Information is not kept longer than necessary (9) nor used (10) or disclosed (11) for anything beyond the original purpose of collection.
- Information can only be disclosed to foreign entities who comply the Act or provide similar safeguards (12)
- Unique identifiers are only generated when necessary for an entity’s functions, and cannot be reused by another entity (13)

This Act establishes the Privacy Commissioner, who may issue guidance (e.g. [a]), tools like the Privacy Impact Assessment, and legally binding codes of practice, outlining different standards (may be more or less stringent) for specific types of information, such as the Health Information Privacy Code applicable to all health agencies.

Wherever AI systems in government use personal information, the Privacy Act’s principles prompt deployers to consider several questions:
- Does the information used come directly from the person it is about (2)? Is AI being used to generate predictions or assumptions, or draw on public sources, rather than collected from the person directly?
- Does the individual know their information may be used by (or used to train) AI tools (3)?
- Is personal information protected against unauthorised access, particularly where publicly available AI tools risk data leakage and other unintentional data memorisation (5)?
- Can individuals access and correct data being used to train an agency’s predictive models (6-7)?
- Can individuals correct (7) or challenge the accuracy of a prediction or other AI-derived output (8)? Such AI-derived outputs itself are still considered personal information under the Privacy Act.
- Is the use of personal information in AI directly related to the original purpose of its collection (10)? Could it be reused by the AI provider, particularly publicly available AI tools?

**Further reading**: [a] [Artificial intelligence and the Information Privacy Principles - Privacy Commissioner - Sept 2023](https://www.privacy.org.nz/assets/New-order/Resources-/Publications/Guidance-resources/AI-Guidance-Resources-/AI-and-the-Information-Privacy-Principles.pdf)

</div>
</div>


<div class="box" id="box-1-1-3">
<div class="box__header"><span class="box__number">Box 1.1.3</span><h3 class="box__title" id="box-1-1-3-h">Public Records Act 2005 (PRA)</h3></div>
<div class="box__body" markdown="1">

Promotes comprehensive recordkeeping within government by regulating how all information about an agency’s “affairs” is managed within them.

All information generated by a “government office”, including AI-generated information, is considered a public record. Section 17 mandates that agencies “create and maintain full and accurate records of its affairs”. Section 27 enables Archives New Zealand to set mandatory recordkeeping standards. The current standard has three principles, the third of which (“Information and records are well managed”) elaborates on the obligations on agencies:
- Recordkeeping occurs as part of normal business practice
- Records must be reliable and trustworthy
- Records must be protected from unauthorised access, alteration or loss

Wherever AI is used in government, the use and impact of AI on an agency’s affairs and information needs to be documented as part of routine recordkeeping. Archives New Zealand provides a checklist tool to promote compliance by recording what the AI system is and will be used for.

**Further reading**: [Artificial intelligence and public and local authority records - Archives New Zealand](https://www.archives.govt.nz/manage-information/how-to-manage-your-information/implementation/artificial-intelligence-and-public-records)

</div>
</div>

## 1.2 Automating statutory decisions and actions must be legislated {#s1-2}

Establishing legislation, the laws that set up an entity and determine its mandate, may include provisions that enable Automated Electronic Systems (AES) to perform actions specified in legislation that only specified authorised people (typically the chief executive) can do, as if such an authorised person performed the action themselves. While the term is not defined in law, it can reasonably be understood to include any algorithm or AI (as defined in [Section 4](../04-section4/)) that makes decisions without human intervention. AES provisions typically follow this pattern:

- Arranging the use of an AES

  - Outlining which statutory roles and actions the system can substitute

  - System must be able to perform the actions “with reasonable reliability”

  - A human alternative must always be available to perform the action instead

  - Allowing systems with components outside New Zealand to be used

  - Mandating consultation with the Privacy Commissioner

- Describing the effect of the use of the system

  - Treating its action as done properly, as if it were done by the specified person

  - If its actions are clearly wrong, they may be done by people

- Describing offences against an AES if applicable

  - Failure to comply with requirements or directions from an AES

  - Obstructing, hindering, damaging or impairing an AES

  - Deceiving or withholding information from an AES

  - Covering legislation-specific offences, e.g. manipulating offending goods seized by an AES without its permission.

This pattern is not in legislation where powers are conferred on entities rather than specified individuals. For example, the Accident Compensation Corporation (ACC) – a Crown agent with well-publicised automated decision-making – is not empowered to use AES. Most of its administrative decisions are conferred on “the Corporation”, not on a chief executive or a qualified person. ACC may need specific AES provisions if it wishes to automate complicated decisions that must be made by qualified assessors, such as rehabilitation support needs.

> Explicit legislation is required to say the system’s action counts as a specified person’s action, if the legislation requires a specified person to perform an action to be automated.

## 1.3 Agencies may be given the power to enact secondary legislation on their own {#s1-3}

Two examples of secondary legislation have already been mentioned:

- Privacy Act codes of practice, issued by the Privacy Commissioner

- Information and records management standard, issued by Archives New Zealand

Secondary legislation holds the same authority as any other Act of Parliament. However, it is usually drafted by the agency responsible for administering the Act. The Cabinet Manual describes secondary legislation as addressing matters of detail, technical issues, or those likely to require frequent changes. Therefore, this regulatory route is preferred for giving effect to generic principles (like those in the Acts mentioned) by clarifying obligations at a technical level. For the Privacy Act 2020, secondary legislation can also modify the Act’s obligations in specific situations. For instance, the Health Information Privacy Code clarifies when health privacy protections are stronger (e.g. parents have less access once a child is 16 or older) or weaker (e.g. legal representatives of deceased or incapacitated individuals may access information).

> AI systems must also follow any secondary legislation that applies to the context it is being used, or data it is using.

## 1.4 Government-wide **standards and guidance** provide all-of-Government best practice in particular areas {#s1-4}

The Public Service Act 2020 enables the designation of a specific agency as a system leader to “lead and co-ordinate best practice in a particular subject matter area” across all government sectors. This leadership is realised through setting standards or guidance in such areas. Standards are applicable to public service agencies, while guidance applies to any Crown organisation. These standards and guidance were issued before the 2020 act, with varying levels of enforceability. Some are mandated by Cabinet directives or ministerial instructions; others are voluntary best practice. The following section describes relevant system leaders whose guidance influences the use of AI systems as of December 2025.


<div class="box" id="box-1-4-1">
<div class="box__header"><span class="box__number">Box 1.4.1</span><h3 class="box__title" id="box-1-4-1-h">Government Chief Digital Officer (GCDO)</h3></div>
<div class="box__body" markdown="1">

Coordinates the development, procurement, assurance and use of digital systems across government. Operated out of the Department of Internal Affairs until April 2026.
- Maintains guidance and tools that facilitate best practice design and implementation of digital systems, including AI tools which are typically cloud-hosted Web interfaces.
  - [Information sharing standard](https://www.digital.govt.nz/standards-and-guidance/information-sharing-standard): facilitating protection of personal information held by government when systematically sharing or collecting information from a third party outside government. Mandated under s57 Public Service Act 2020.
  - [Digital Service Design Standard](https://www.digital.govt.nz/standards-and-guidance/digital-service-design-standard): supporting the government to design and provide public services that are easily accessible, integrated, inclusive and trusted by all New Zealanders. Applies to public-facing or inter-agency digital services undertaken by external third parties.
  - [Government Web Standards](https://www.digital.govt.nz/standards-and-guidance/nz-government-web-standards): usability and accessibility standards for both internal and public facing web interfaces. Mandated by Cabinet direction.
  - [Risks assessment for public cloud services](https://www.digital.govt.nz/standards-and-guidance/technology-and-architecture/cloud-services/assess-the-risks): helps identify risks and security controls to consider when using a public cloud service. Optional tool for assisting in mandatory risk assessments.
- Maintains guidance and frameworks for the safe and responsible use of AI
  - [Public Service AI Framework](https://www.digital.govt.nz/standards-and-guidance/technology-and-architecture/artificial-intelligence/public-service-artificial-intelligence-framework) (PSAIF) provides a strategic vision and principles for adopting AI responsibly across the public service.
  - [Responsible AI Guidance (RAIG) for the Public Service: GenAI](https://www.digital.govt.nz/standards-and-guidance/technology-and-architecture/artificial-intelligence/responsible-ai-guidance-for-the-public-service-genai) (RAIG-PSG) guides agencies in the development and use of GenAI systems, linked to the OECD AI Principles. RAIG is intended to be a series, for example the Ministry of Business, Innovation and Employment (MBIE) has developed [RAIG for businesses](https://www.mbie.govt.nz/business-and-employment/business/support-for-business/responsible-ai-guidance-for-businesses).
- Mandates coordinated procurement of common digital products and services
  - [ICT Common Capability contracts](https://www.digital.govt.nz/products-and-services/buying-products-and-services) enable procurement of a commonly used technology once on behalf of multiple or all government agencies.
  - [Assurance Services Panel](https://www.digital.govt.nz/standards-and-guidance/governance/system-assurance/gcdo-assurance-services-panel) convenes trusted providers of quality assurance services that agencies are required to use for any digital investment they make.
- Coordinates digital transformation across the public service through the [Service Modernisation Roadmap](https://dns.govt.nz/digital-government/key-areas-of-work/service-modernisation). AI-related initiatives include:
  - All-of-Government AI reference architecture to guide the design and implementation of government’s AI solutions, promote best practices and accelerate development across the public service.
  - Two-year roadmap to FY27/28 for accelerating use of government AI solutions

The GCDO is the key leader responsible for standards and guidance in AI systems and tools whose development is contracted out, as with most digital systems in government.

</div>
</div>


<div class="box" id="box-1-4-2">
<div class="box__header"><span class="box__number">Box 1.4.2</span><h3 class="box__title" id="box-1-4-2-h">Government Chief Information Security Officer (GCISO)</h3></div>
<div class="box__body" markdown="1">

Issues mandatory security requirements to government agencies. These functions are hosted by the National Cyber Security Centre (NCSC) which provides guidance and intelligence for cybersecurity threats to public and private organisations. Both are operated out of the Government Communications Security Bureau.
- The GCISO maintains the [Protective Security Requirements (PSR),](https://www.protectivesecurity.govt.nz/) expectations for managing all aspects of an agency’s security: physical, personnel and information security, and security governance. Mandated by Cabinet Directive CAB MIN (14) 39/38.
  - [New Zealand Information Security Manual](https://nzism.gcsb.govt.nz/) catalogues essential controls and additional recommended controls.
- The NCSC works with its allied counterparts to issue non-binding joint guidance on secure AI use for any NZ organisation to consider:
  - [Guidelines for secure AI system development](https://www.ncsc.govt.nz/protect-your-organisation/guidelines-for-secure-ai-system-development/), December 2023. Provides four high level guiding principles to frame secure AI system development: secure design, secure development, secure deployment, and secure operation & maintenance.
  - [Engaging with artificial intelligence](https://www.ncsc.govt.nz/protect-your-organisation/engaging-with-artificial-intelligence/), January 2024. Outlines common challenges around AI and potential mitigations for model data poisoning, input manipulation, hallucination, privacy concerns, model stealing.
  - [Deploying artificial intelligence (AI) systems securely](https://www.ncsc.govt.nz/protect-your-organisation/deploying-ai-systems-securely/), April 2024. Expands on the secure deployment and secure operation & maintenance of the December 2023 guidance, and builds on mitigations identified in the January 2024 guidance.
  - [Artificial intelligence (AI) data security](https://www.ncsc.govt.nz/protect-your-organisation/ai-data-security/), May 2025.  Provides guidance for securing data used during AI development and deployment.
  - [Principles for the Secure Integration of Artificial Intelligence in Operational Technology](https://www.ncsc.govt.nz/assets/guidance/Documents/Principles-for-the-Secure-Integration-of-Artificial-Intelligence-in-Operational-Technology.pdf), December 2025. Prescribes technical considerations around the use of AI in safety-critical equipment and facilities, such as electricity infrastructure management, hospital operation, traffic management, police and correctional facility security.

The GCISO’s security mandates necessarily applies to any government AI model or system, including those developed in-house. The wider NCSC provides internationally endorsed best practice around securing AI systems.

</div>
</div>


<div class="box" id="box-1-4-3">
<div class="box__header"><span class="box__number">Box 1.4.3</span><h3 class="box__title" id="box-1-4-3-h">Government Chief Data Steward (GCDS)</h3></div>
<div class="box__body" markdown="1">

Promotes accessibility, reliability and ethical use of data in government. Operated out of Statistics New Zealand.
- Maintains policies that promote trusted use of data and algorithms (including AI) in government, all of which are voluntary.
  - [Data Protection Use and Policy](https://www.digital.govt.nz/standards-and-guidance/privacy-security-and-risk/privacy/data-protection-and-use-policy-dpup) (DPUP) outlines values, behaviours and practice beyond legal obligations to promote respectful, culturally considerate and transparent collection and use of personal data.
  - [Algorithm Charter](https://data.govt.nz/toolkit/data-ethics/government-algorithm-transparency-and-accountability/algorithm-charter) (“the Charter”) is signed by individual agencies to signal how they design and implement algorithms in a transparent, people-focused, legally compliant, and human-overseen manner.
  - [Algorithm impact assessment (AIA) toolkit](https://data.govt.nz/toolkit/data-ethics/government-algorithm-transparency-and-accountability/algorithm-impact-assessment-toolkit) helps agencies operationalise their Charter commitments, providing a specific threshold for systems in scope of the Charter, and specific guidance at each stage of development.
- Outside of the GCDS, StatsNZ is responsible for the maintenance of systems that securely integrate and match data from different agencies. Given the sensitivity around massively integrated data, policies surrounding their use are strictly enforced.
  - [Five Safes](https://www.stats.govt.nz/integrated-data/how-we-keep-integrated-data-safe/) framework conditions access to integrated data given: safe people, safe projects, safe settings, safe data, and safe output.
  - [Ngā Tikanga Paihere](https://data.govt.nz/toolkit/data-ethics/nga-tikanga-paihere) outlining ten tikanga Māori concepts that promote culturally appropriate, good faith engagement with Māori and use of Māori data.

The GCDS provides voluntary guidance for the trustworthy, ethical and culturally appropriate use of government data inputted in AI systems and tools, and in the development of their own AI models.

</div>
</div>

## 1.5 Government agencies use international standard risk methodologies, and new standards are emerging to facilitate AI system risk management {#s1-5}

The PSR requires agencies follow ISO 31000 to manage risk, a widely practiced international standard. ISO 31000 does not impose a checklist exercise, but rather actively engages an organisation in identifying the specific risks within an agency, analysing its impact, evaluating the acceptability of risk, then deciding how to approach it (accept, transfer, mitigate, avoid).

The PSR also references the ISO 27000 family of standards, which provides specific guidance for managing risk in information systems and is usually already implemented by government agencies. A new family of ISO standards is emerging for the governance and risk management of AI systems that mirrors the structure of the ISO 27000 family. There are gaps, as shown in [Table 1](#table-1), but all listed AI system standards are officially published with full consensus from ISO.

Notably, early-adopter government agencies like ACC have opted to use the American federal government’s standard for AI risk management, given their use of American cybersecurity and privacy standards.

<a id="table-1"></a>

| Function of standard | ISO 2700x Information system standards | ISO AI system standards |
| --- | --- | --- |
| Definitions for shared vocabulary | ISO 27000 | ISO 22989 |
| Management system requirements (risk governance spine) | ISO 27001 | ISO 42001 |
| Catalogue of risk control guidance | ISO 27002 | _No definitive equivalent, some in ISO 24027-29_ |
| Measurement and metrics | ISO 27004 | _No equivalent_ |
| Tailoring ISO 31000 (risk management methodology) to a specific domain | ISO 27005 | ISO 23894 |
| Impact and control assessment | ISO 27008 | ISO 42005 |

> _Table 1: Functional alignment between ISO information system and AI system standards_

> Mandatory security requirements are largely based on international standards. Agencies can adopt emerging recognised international standards for AI risk management with the confidence that future mandatory requirements are likely to closely align with them.

## 1.6 Frameworks help affirm Māori **sovereignty over their data, and algorithms** developed from their data {#s1-6}

Iwi Māori retain tino rangatiratanga over all their taonga, as guaranteed in Article 2 of Te Tiriti o Waitangi. This rangatiratanga extends to any data about or from Māori people and culture, as outlined in Wai 2522[^2]. Te Mana Raraunga, a network of Māori experts in data, have devised principles (which are currently not mandated across government) to promote practices that affirm Māori data sovereignty, as outlined in [Table 2](#table-2).

<a id="table-2"></a>

| **Rangatiratanga**: Right to control and access Māori data and data ecosystems, storing data here enhances control | **Whakapapa**: Metadata should be accessible to provide context, origin, provenance. Methodologies should prioritise Māori aspirations | **Whanaungatanga:** Individual rights to data and privacy are balanced with those of the collective |
| --- | --- | --- |
| **Kotahitanga:** Empower Māori to derive individual and collective benefit | **Manaakitanga:** Respect the dignity and consent of Māori, avoid deficit-based data practices | **Kaitiakitanga**: Enable Māori to protect their data at all parts of the lifecycle (e.g. storage, transfer, disclosure) according to tikanga |
{:.table-plain}

> _Table 2: Principles of Māori Data Sovereignty. From Te Mana Raraunga, October 2018. [https://www.temanararaunga.maori.nz/principles-of-maori-data-sovereignty](https://www.temanararaunga.maori.nz/principles-of-maori-data-sovereignty)_

This framework was extended by Brown et al. (2024) to promote sovereignty of algorithmic systems (not just the algorithm itself, but the inputs, output interpretation, design and ongoing management) informed by data about or from Māori. In addition to the obligations above on data used by algorithms, their framework also offers further algorithm-specific guidance around each of the principles, as outlined in [Table 3](#table-3).

<a id="table-3"></a>

| **Rangatiratanga**: Right to control development and use of algorithmic systems | **Whakapapa**: Māori understand of all aspects of the algorithm system | **Whanaungatanga:** Right to challenge its output or outcome, system owners are accountable to Māori |
| --- | --- | --- |
| **Kotahitanga:** As above, for algorithmic systems | **Manaakitanga:** Consider individual and collective privacy throughout the entire operation of the system | **Kaitiakitanga**: As above, for algorithmic systems |
{:.table-plain}

> _Table 3: Principles of Māori Algorithmic Sovereignty. From _Paul T. Brown, Daniel Wilson, Kiri West, Kirita-Rose Escott, Kiya Basabas, Ben Ritchie, Danielle Lucas, Ivy Taia, Natalie Kusabs, Te Taka Keegan, April 2024. Māori Algorithmic Sovereignty: Idea, Principles, and Use._ [https://datascience.codata.org/articles/10.5334/dsj-2024-015](https://datascience.codata.org/articles/10.5334/dsj-2024-015)_

Te Kāhui Raraunga, under the direction of the Data Iwi Leaders Group, have devised Māori Data and AI Governance frameworks for use within the public service. The Māori Data Governance model implements the six principles from Te Mana Raraunga. Five values frame the directives under the eight pou which categorise actions that give effect to the values, as shown in [Table 4](#table-4).

<a id="table-4"></a>

| **Vision:** Tuia te korowai o Hine-Raraunga / Data for self-determination |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Values** |  |  |  |  |
| Nurture data as taonga | Use data for good | Put iwi Māori data in iwi Māori hands | Be accountable | Decolonise data systems |
| **Pou (Pillars)** |  |  |  |  |
| 1. Capacities and workforce development | 2. Data / **IT** infrastructure | 3. Data collection / **AI data generation** | 4. Data protection |  |
| 5. Data access, sharing and repatriation | 6. Data use and reuse / **for AI implementation** | 7. Data / **AI** quality and system integrity |  |  |
| 8. Data classification |  |  |  |  |
{:.table-plain}

> _Table 4: Māori Data Governance Model (with Māori AI Governance Model overlaid in bold). From Tahu Kukutai, Kyla Campbell-Kamariera, Aroha Mead, Kirikowhai Mikaere, Caleb Moses, Jesse Whitehead and Donna Cormack, 2023. Māori data governance model, Te Kāhui Raraunga, [https://www.kahuiraraunga.io/maoridatagovernance](https://www.kahuiraraunga.io/maoridatagovernance) and Te Kāhui Raraunga, 2025. Māori Artificial Intelligence Governance Framework. Contextualised advice for AI use, extending the Māori data governance model, [https://www.kahuiraraunga.io/maoriaigovernance](https://www.kahuiraraunga.io/maoriaigovernance)_

> Much like the NZISM outlines how to comply with the PSR’s principles, the Māori Data and AI Governance Models outline requirements that affirm the principles of Māori data sovereignty that arise from Te Tiriti o Waitangi.

## 1.7 Agencies set their own **departmental policies and procedures** to clearly establish accountability for following laws, standards and guidance {#s1-7}

These laws, standards and guidance ultimately achieve operational effect when embedded in an agency’s policies and procedures. These policies are enforced through the authority of their chief executive, with breaches addressed primarily through internal managerial consequences. Departmental policies outline legal obligations and give a mandate to government-wide standards and guidance by defining expectations for staff – tailored to its operating environment. Thus, departmental policies are the most effective mechanism for giving practical effect to, and enabling accountability for, laws, standards and guidance within agencies.

Most agencies with published AI policies focus primarily on the use of GenAI tools: mandating use of only approved AI tools, prohibiting the use of sensitive or classified information, promoting awareness of the risk of inaccuracy, bias and confidentiality breaches, requiring training before using approved AI tools, and outlining roles and responsibilities.

Agencies that have published departmental policies for AI use include:

- Ministry of Social Development: predates generative AI but exemplifies mature policies and – more importantly – procedures for algorithm and AI development. Their ADM Standard (MSD, 2022)[^3] outlines baseline requirements for any algorithm that makes decisions, supplemented with technical guidance for more complex systems in their Model Development Lifecycle (MSD, 2021)[^4].

- Courts of New Zealand (2023)[^5]: specific guidance for specific roles with the same principles throughout, with plain English explanations of the limitations of GenAI and why the risks exist. Notably, GenAI use does not need to be disclosed unless asked by courts.

- Land Information New Zealand (2023)[^6]: anonymise names when discussing personal scenarios with AI, disclosing AI use for externally released work, work with Treaty partners if Māori data is involved or Māori interests may be affected in the use of AI.

- Accident Compensation Corporation (2023)[^7]: mandating human oversight throughout use, actively protecting taonga Māori in accordance with Treaty commitments, prescribing unacceptable use of GenAI (e.g. for client care, for resourcing decisions, with personal, health or confidential information).

- New Zealand Police (2025)[^8]: mandating labelling to disclose where GenAI is being used, external vendor disclosure of GenAI use, requiring Tier 2 approval for urgent unapproved uses, prohibiting fully automated (no human in the loop) GenAI, prohibiting use of AI in court, requiring audit logs for complete recordkeeping.

> Departmental policies are ultimately how standards and guidance are given effect: as expectations on staff relying on internal accountability. They are also an opportunity to tailor policy around what agencies do and how they operate.

## 1.8 Action: Establish a New Zealand Artificial Intelligence Manual (NZAIM) to unify technical guidance in implementing trustworthy government AI systems {#s1-8}

The right rules, principles and objectives for promoting trustworthy AI system delivery are already in place. The OIA’s transparency requirements effectively bind agencies to thoroughly consider best practice – offered but not mandated by other guidance instruments – in designing transparent AI systems trusted in independently making decisions. Other best practice around fairness and non-discrimination are promoted through recognising the ex post risk of an investigation finding AI decisions to be unlawful, mistaken or discriminatory.

However, the current guidance ecosystem is missing a keystone instrument that provides a single authoritative source of technical guidance around controlling the risks and promoting the norms identified by other relevant instruments.[^9] To reduce existing fragmentation, this unified guidance should organise all the **objectives** of each guidance instrument, and mandate or recommend technical **controls** and its **rationale**. This approach is already employed by the NZISM, which provides agencies flexibility around specific controls it recommends but does not mandate, requiring agencies to document and accept the residual risk of non-use. These controls are supported by a structured certification and accreditation process standardising system assurance. This approach has streamlined cybersecurity practice in government and transparently models best practice for non-government entities. An NZAIM can not only promote these outcomes for government AI, but also to private AI by providing a consumer signal accrediting, rather than outright regulation compelling, best practice. The GCDO has committed to an AI assurance model and toolkit by 2027, and a separate deliverable on safety certifications. Like the NZISM, an NZAIM would encompass both.

> The NZAIM would catalogue gold standard technical controls for AI risk management in government, helping technical practitioners give effect to all the different guidance instruments, and model best practice for the private sector.


## References

[^2]: Waitangi Tribunal, March 2023. The Report on the Comprehensive and Progressive Agreement for Trans-Pacific Partnership. [https://www.waitangitribunal.govt.nz/en/news/tribunal-releases-report-on-cptpp](https://www.waitangitribunal.govt.nz/en/news/tribunal-releases-report-on-cptpp)
[^3]: Ministry of Social Development, 2022. About MSD’s Automated Decision-Making Standard. [https://www.msd.govt.nz/about-msd-and-our-work/work-programmes/initiatives/phrae/adm-standard.html](https://www.msd.govt.nz/about-msd-and-our-work/work-programmes/initiatives/phrae/adm-standard.html)
[^4]: Ministry of Social Development and Nicholson Consulting, October 2021. Model Development Lifecycle. [https://www.msd.govt.nz/about-msd-and-our-work/work-programmes/initiatives/phrae/model-development-lifecycle.html](https://www.msd.govt.nz/about-msd-and-our-work/work-programmes/initiatives/phrae/model-development-lifecycle.html)
[^5]: Courts of New Zealand, December 2023. Guidelines for use of generative artificial intelligence in Courts and Tribunals. [https://www.courtsofnz.govt.nz/going-to-court/practice-directions/practice-guidelines/all-benches/guidelines-for-use-of-generative-artificial-intelligence-in-courts-and-tribunals](https://www.courtsofnz.govt.nz/going-to-court/practice-directions/practice-guidelines/all-benches/guidelines-for-use-of-generative-artificial-intelligence-in-courts-and-tribunals)
[^6]: Land Information New Zealand, December 2023. Artificial Intelligence (AI) Use Policy. [https://www.linz.govt.nz/sites/default/files/2024-05/DOIA%2024-261%20Artificial%20Intelligence%20Use%20Policy%20signed.pdf](https://www.linz.govt.nz/sites/default/files/2024-05/DOIA%2024-261%20Artificial%20Intelligence%20Use%20Policy%20signed.pdf)
[^7]: ACC, August 2023. Generative AI Models and Services Policy. [https://www.acc.co.nz/assets/oia-responses/Documents-relating-to-the-algorithm-charter-of-aotearoa-oia-response-gov-031495.pdf](https://www.acc.co.nz/assets/oia-responses/Documents-relating-to-the-algorithm-charter-of-aotearoa-oia-response-gov-031495.pdf)
[^8]: New Zealand Police, September 2025. Acceptable use of Generative AI. [https://www.police.govt.nz/about-us/programmes-and-initiatives/police-use-emergent-technologies/generative-ai](https://www.police.govt.nz/about-us/programmes-and-initiatives/police-use-emergent-technologies/generative-ai)
[^9]: It may be argued that the AIA toolkit fulfils such a role. It is primarily a risk assessment framework and only prescribes high-level controls, not to the same technical depth as the NZISM.
