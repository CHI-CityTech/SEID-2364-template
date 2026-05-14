# SEID 2364 – Assignment 11
## Comparative Ethical Framework Analysis
### ACM, IEEE, EU Governance, and Bad Actors in Socio-Technical Systems

**Course:** SEID 2364 – Societal and Ethical Impacts of Data Science  
**Instructor:** Dr. David B. Smith  
**Date Assigned:** [Insert Date]  
**Due Date:** [Insert Date]

---

## Framing

In earlier assignments, you evaluated ethical problems using several different approaches. You identified harm, applied ethical theories, analyzed systems structurally, used the EU AI Act as a regulatory framework, examined how risk changes across deployment contexts, and reconstructed mediation pathways using EDOCA.

This assignment shifts the focus again.

You are no longer only applying a framework to a system. You are comparing how different professional and governance frameworks evaluate the same socio-technical system differently.

This assignment formalizes the comparative work introduced in the Week 11 live session. In class, you begin with the short COVID case card in order to surface your own ethical criteria around authority, harm, and responsibility. The lecture then introduces professional and governance frameworks as different ways of operationalizing ethical responsibility. The assignment asks you to extend that classroom work into a structured comparative analysis.

The central question is:

> How do professional and governance frameworks operationalize ethical responsibility differently, and how do those differences shape the evaluation of a data-driven system?

You will compare:

- ACM Code of Ethics and Professional Conduct
- IEEE Code of Ethics
- an EU-oriented governance framework
- BBS / EDOCA as a mediation and power-structure analysis

You will use **COVID-19 misinformation moderation** as the required shared case. The goal is not to decide whether COVID moderation was simply “right” or “wrong.” The goal is to analyze how different frameworks make different harms, responsibilities, actors, and power structures visible.

---

## Required Case

### COVID-19 Misinformation Moderation

During the COVID-19 pandemic, false and misleading claims about the virus, masks, vaccines, treatments, public-health restrictions, and the credibility of institutions circulated widely online. Platforms responded by labeling, downranking, removing, or restricting some COVID-related claims. These actions often involved public-health guidance, platform policy, fact-checking organizations, automated moderation systems, human review, regulators, and users.

This case is ethically ambiguous because moderation may have reduced harmful misinformation and protected public health, while also raising concerns about free expression, scientific uncertainty, platform power, state influence, transparency, appeals, and public trust.

You should use the expanded student-facing COVID case study brief in `case-studies/case_study-covid_misinformation.md` as your primary case background. The short Week 11 case card is only an entry point for the live class discussion.

---

## Required Frameworks

### 1. ACM Code of Ethics and Professional Conduct
https://www.acm.org/code-of-ethics

You may also consult ACM Publications Policies if relevant to authorship, disclosure, misinformation, research integrity, or professional conduct:

https://www.acm.org/publications/policies

### 2. IEEE Code of Ethics
https://www.ieee.org/about/corporate/governance/p7-8.html

### 3. EU-Oriented Governance Framework
Use at least one EU-oriented source. Recommended options include:

- European Commission Ethics Guidelines for Trustworthy AI  
  https://digital-strategy.ec.europa.eu/en/library/ethics-guidelines-trustworthy-ai

- European Commission COVID-19 Disinformation Monitoring Programme  
  https://digital-strategy.ec.europa.eu/en/policies/covid-19-disinformation-monitoring

- EU AI Act materials, if your analysis focuses on automated moderation, recommender systems, risk classification, or AI-mediated decision-making.

### 4. BBS / EDOCA
Use BBS and EDOCA to analyze mediation, observability, control, authority, distortion, and responsibility distribution.

---

## Assignment Goal

Your goal is to investigate how these frameworks differ, not to memorize or summarize them.

You should ask:

- What does each framework make visible?
- What does each framework under-describe?
- Whose responsibility is emphasized?
- Which harms are foregrounded?
- Which ethical theories appear most strongly weighted?
- How does each framework help identify or prevent bad-actor behavior?
- Where do the frameworks agree?
- Where do they diverge?

---

## Key Concepts

### Ethical Weighting

No professional or governance framework is purely deontological, consequentialist, or virtue-based. Most frameworks mix multiple ethical tendencies. Your task is to identify how each framework appears to weight different ethical traditions.

For example:

- deontological tendencies may appear as duties, obligations, rules, rights, or prohibitions;
- consequentialist tendencies may appear as harm reduction, public welfare, safety, risk mitigation, or societal impact;
- virtue-oriented tendencies may appear as honesty, competence, integrity, responsibility, professionalism, or care.

Do not simply label ACM as one theory and IEEE as another. Instead, identify how each framework combines ethical approaches.

### Bad Actor

In this assignment, a bad actor does not necessarily mean a bad person. A bad actor is an agent whose behavior degrades the integrity, safety, trust, fairness, or accountability of a system.

Bad actors may be:

- malicious;
- strategic;
- reckless;
- negligent;
- misinformed;
- institutional;
- procedural.

You should distinguish between:

- misinformation: false or misleading information shared without necessarily intending harm;
- disinformation: false or misleading information shared deliberately to deceive or manipulate;
- malinformation: true or partly true information used harmfully or out of context.

### Observability, Control, and Authority

For each framework, ask whether it helps identify:

- who can observe the system;
- who can control the system;
- who has authority over system action;
- who is affected but cannot intervene;
- where authority, control, and observability are separated.

### Example of Framework Divergence

One useful question for this assignment is whether different professional frameworks might judge the same conduct differently in emphasis, even when they overlap in concern.

For example, imagine a moderation engineer knows that a COVID misinformation classifier has a high false-positive rate for posts discussing adverse vaccine side effects in non-standard English. The engineer is pressured to deploy the model anyway because the platform wants to reduce harmful misinformation quickly during a public-health emergency.

- An **ACM-oriented analysis** might foreground fairness, avoidance of harm, transparency, and the obligation not to build or deploy a system that systematically misclassifies already vulnerable users.
- An **IEEE-oriented analysis** might foreground safety, risk disclosure, technical responsibility, and the obligation to communicate known system limitations and avoid reckless deployment of an unreliable technical system.

These may lead to overlapping criticism, but not identical criticism. ACM may make the inequity and professional duty to affected users more visible. IEEE may make engineering risk, disclosure, and technical safety obligations more visible. Your task is to identify such differences precisely rather than treating the frameworks as interchangeable.

---

## Tasks

Complete the following as a structured document.

---

## Part 1 – Case Definition

Briefly describe the COVID misinformation moderation system you are analyzing.

Include:

- what action is being taken: labeling, downranking, removal, suspension, redirecting users, demonetization, or another action;
- who is taking the action;
- who is affected;
- what decision or transformation occurs;
- what makes the case ethically ambiguous.

Do not begin with your final judgment. Describe the system first.

---

## Part 2 – Stakeholder Map

Identify the major stakeholders.

Include where relevant:

- users posting content;
- users consuming content;
- public-health authorities;
- platform companies;
- engineers and moderators;
- fact-checkers or expert reviewers;
- regulators or courts;
- researchers and journalists;
- advertisers or platform business interests;
- the broader public.

For each stakeholder, identify:

- possible benefit;
- possible harm;
- what they can observe;
- what they can control;
- what authority they have or lack.

You may use a table.

---

## Part 3 – Bad Actor Analysis

Analyze the different kinds of actors that may appear in the case.

You do not need to find every category, but you should discuss at least three.

Possible categories:

- misinformed actor;
- negligent actor;
- reckless actor;
- strategic actor;
- malicious actor;
- institutional actor;
- procedural actor.

For each category you discuss:

1. Define the actor’s role in the case.
2. Explain whether the actor’s harm is intentional, negligent, structural, or uncertain.
3. Explain whether the system can observe the difference between this actor and other actors.
4. Explain why that distinction matters ethically.

Guiding question:

> If two users share the same false claim, but one sincerely believes it and the other is deliberately manipulating people, should the system treat them the same way? What if the system cannot tell the difference?

---

## Part 4 – ACM Framework Analysis

Analyze the case through the ACM Code of Ethics.

Do not summarize the entire code. Select the principles most relevant to your case.

Discuss:

- Which ACM principles are most relevant?
- What does ACM make visible in the case?
- What kinds of harm does ACM foreground?
- What responsibilities does ACM place on computing professionals?
- How might ACM help prevent a professional or institution from becoming a bad actor?
- What does ACM under-describe or leave unresolved?

Be specific. Refer to particular ACM principles where possible.

---

## Part 5 – IEEE Framework Analysis

Analyze the case through the IEEE Code of Ethics.

Do not summarize the entire code. Select the principles most relevant to your case.

Discuss:

- Which IEEE principles are most relevant?
- What does IEEE make visible in the case?
- What kinds of harm does IEEE foreground?
- What responsibilities does IEEE place on engineers or technical professionals?
- How might IEEE help prevent reckless, negligent, or unsafe technical practice?
- What does IEEE under-describe or leave unresolved?

Be specific. Refer to particular IEEE commitments where possible.

---

## Part 6 – EU-Oriented Governance Analysis

Analyze the case through an EU-oriented governance framework.

You may use the Ethics Guidelines for Trustworthy AI, the COVID-19 Disinformation Monitoring Programme, the EU AI Act, or another approved EU governance source.

Discuss:

- What does the EU-oriented framework make visible?
- Does it focus on rights, transparency, accountability, proportionality, oversight, systemic risk, or public welfare?
- Who is treated as responsible: the professional, the platform, the deployer, the institution, the regulator, or society?
- How does this differ from ACM and IEEE?
- What does the EU-oriented framework under-describe or leave unresolved?

Important note: The EU AI Act may not be the most direct framework for the COVID moderation case unless your analysis focuses specifically on AI classifiers, recommender systems, or automated decision-making. You may use EU platform-governance or disinformation-monitoring materials instead.

---

## Part 7 – Ethical Theory Weighting Comparison

Compare ACM, IEEE, and your EU-oriented framework in terms of ethical theory.

For each framework, identify evidence of:

- deontological reasoning;
- consequentialist reasoning;
- virtue-oriented reasoning.

Then answer:

- Which ethical tendency appears strongest in each framework?
- Which tendency appears secondary?
- Are any important tendencies missing or weak?
- How does this weighting affect the way the framework evaluates the COVID moderation case?

You may use a table.

Recommended table format:

| Framework | Deontological Elements | Consequentialist Elements | Virtue Ethics Elements | Dominant Weighting | What This Makes Visible |
|---|---|---|---|---|---|
| ACM | | | | | |
| IEEE | | | | | |
| EU-Oriented Governance | | | | | |

---

## Part 8 – BBS / EDOCA Power-Structure Analysis

Using BBS / EDOCA, analyze the distribution of observability, control, and authority.

At minimum, address:

- Who can observe moderation decisions?
- Who can observe why a decision was made?
- Who controls ranking, labeling, removal, or appeal?
- Who has authority to define dangerous misinformation?
- Who is affected but cannot intervene?
- Where are authority and control separated?
- Where are control and observability separated?
- Where is responsibility distributed or unclear?

You may include effort and distortion if useful.

Guiding principle:

> Frameworks identify values. EDOCA identifies power.

---

## Part 9 – Comparative Synthesis

Write a synthesis comparing the frameworks.

You must answer:

1. Where do ACM, IEEE, and EU-oriented governance agree?
2. Where do they diverge?
3. Which stakeholders become visible under each framework?
4. Which harms become visible under each framework?
5. Which actors or harms remain under-described?
6. Which framework is strongest for identifying professional responsibility?
7. Which framework is strongest for identifying system-level governance responsibility?
8. Which framework is weakest for this case, and why?

Do not end by saying simply that “all frameworks are useful.” Explain how they are useful differently.

---

## Part 10 – Reflection

Respond briefly:

> How did comparing professional and governance frameworks change your understanding of ethical responsibility in data science?

You may also address:

- how professionals can avoid becoming bad actors;
- how institutions can create bad-actor conditions;
- how ethical frameworks handle uncertainty;
- how mediation pathways change responsibility.

---

## Deliverable

Submit a structured document in Markdown or PDF.

Recommended filename:

`assignment-11-comparative-framework-analysis.md`

Recommended structure:

1. Case Definition
2. Stakeholder Map
3. Bad Actor Analysis
4. ACM Analysis
5. IEEE Analysis
6. EU-Oriented Governance Analysis
7. Ethical Theory Weighting Comparison
8. BBS / EDOCA Power-Structure Analysis
9. Comparative Synthesis
10. Reflection
11. Sources

---

## Source Requirements

You must cite:

- ACM Code of Ethics and Professional Conduct;
- IEEE Code of Ethics;
- at least one EU-oriented governance source;
- the COVID misinformation case study brief or sources referenced in it;
- any additional sources you use.

Add your sources to Zotero where applicable.

---

## Evaluation Criteria

### Framework Understanding
Excellent work identifies relevant portions of ACM, IEEE, and EU-oriented governance frameworks and explains how they operate differently. Weak work merely summarizes the documents.

### Ethical Theory Comparison
Excellent work identifies how each framework combines deontological, consequentialist, and virtue-oriented reasoning. Weak work assigns each framework to only one ethical theory without evidence.

### Bad Actor Analysis
Excellent work distinguishes malicious, strategic, negligent, reckless, misinformed, institutional, and procedural forms of harmful agency. Weak work treats all harmful actors as the same.

### Stakeholder and Power Analysis
Excellent work identifies who benefits, who is harmed, who can observe, who can control, and who has authority. Weak work lists stakeholders without analyzing their power positions.

### BBS / EDOCA Integration
Excellent work uses observability, control, authority, distortion, and responsibility distribution to deepen the framework comparison. Weak work adds BBS terminology without applying it.

### Comparative Synthesis
Excellent work explains where the frameworks agree, diverge, and leave gaps. Weak work concludes that all frameworks are similar or equally useful without analysis.

### Clarity and Organization
Excellent work is clearly structured, specific, and grounded in sources. Weak work is vague, overly general, or unsupported.

---

## TL;DR

You are comparing ethical frameworks, not simply judging COVID moderation.

Use the COVID misinformation case as a shared test case.

Compare:

- ACM;
- IEEE;
- EU-oriented governance;
- BBS / EDOCA.

Analyze:

- ethical theory weighting;
- stakeholders;
- bad actors;
- observability;
- control;
- authority;
- agreement;
- divergence;
- unresolved ambiguity.

Your conclusion should explain how different frameworks make different ethical problems visible.

