# SEID 2364 — Assignment 08
## Bias, Decision-Making, and Harm in AI-Mediated Systems

**Course:** SEID 2364  
**Instructor:** Dr. David B. Smith  
**Date Assigned:** Week 8  
**Due Date:** Week 9

---

## Framing

In Assignment 7, you evaluated an AI system through the lens of EU AI Act regulation. That work was about classification — fitting a system into a fixed regulatory structure and examining what that structure demands.

This assignment asks a different question:

> Where does bias enter an AI system, and how does it shape decisions and produce harm?

This is not a classification exercise. You are not categorizing risk — you are tracing it. The focus is on the internal logic of a system: how design choices, data sources, decision authority, and deployment context create conditions for bias to emerge, persist, or amplify.

The EU AI Act may be relevant as context or as a reference point, but it is not the analytical framework here. The core tools for this assignment come from the required readings.

---

## Assignment Overview

You will select a **new system** from the provided set and develop **three deployment scenarios** of that system. Across those scenarios, you will trace how bias enters and changes, how decisions are shaped, and how harm — direct and indirect — flows through the system's mediation structure.

**Core Constraint:**
The system itself must remain constant. Variation occurs only through:
- deployment context
- user group
- decision authority
- integration within a broader structure

You are not redefining the system — you are **reconfiguring its use** and analyzing what that reconfiguration produces.

---

## System Selection (Required)

You must select **one system only** from the System Selection Set:

[08-SEID2364_usecase_system_set](../resources/08-SEID2364_usecase_system_set.md)

**Important:** If your prior system (from Assignments 4–7) closely resembles one of the options in the set, you must select a **different system** for this assignment. Assignment 8 is intended as a fresh analytical start. Prior familiarity with a system is not a valid reason to reuse it — the goal is to develop new analytical range.

You must use the same core system across all parts of the assignment.

Assume a baseline implementation using contemporary machine learning or LLM-based methods unless otherwise specified.

Custom systems are not permitted for this assignment.

---

## Required Readings

These readings are the analytical foundation of the assignment. Your analysis must engage with them directly — not as background, but as tools for identifying and describing what is happening in your system.

### Core (Required)

- **Implicit Bias** — Stanford Encyclopedia of Philosophy: https://plato.stanford.edu/entries/implicit-bias/
- **Algorithmic Fairness** — Stanford Encyclopedia of Philosophy: https://plato.stanford.edu/entries/algorithmic-fairness/
- **Ethics of Search Engines** — Stanford Encyclopedia of Philosophy: https://plato.stanford.edu/entries/ethics-search/

Before beginning the assignment tasks, write a **brief synthesis (250–400 words)** that:
- defines bias and fairness in your own terms using the readings
- identifies one tension between implicit bias and algorithmic fairness
- explains how search/ranking ethics clarifies at least one risk in your selected system

This synthesis should appear as a standalone section before your deployment analysis, not embedded in a later task.

### Supplementary (Required)

Identify **at least 2 additional sources** relevant to bias, fairness, or AI decision-making in the domain of your selected system. All sources must be added to Zotero and cited in your document.

---

## Tasks

Complete the following as a structured document.

---

### 1. System Definition (Concise)

Describe the core system:
- what it does
- what type of AI function it performs
- inputs and outputs

Do **not** include deployment context here.

---

### 2. Bias and Fairness Synthesis

Submit your synthesis from the Required Readings section here as a standalone section (250–400 words). This should precede your deployment analysis and establish the conceptual vocabulary you will use throughout.

---

### 3. Deployment Scenarios

Construct **three distinct deployments** of the same system. Each must vary across:
- user group
- institutional context
- decision authority (advisory vs. decision-making)
- level of consequence

**Required:**
- At least one deployment must represent a **non-obvious or secondary use** of the system
- For each deployment, explicitly state **what has changed** from the baseline and why it matters analytically

---

### 4. Mediation Pathway and Bias Location (Core Task)

For each deployment, construct a mediation pathway that maps the flow of information, decisions, and outputs through the system. The pathway should trace the journey from initial input to final consequence.

**Required pathway elements:**
- Sources (where data and inputs originate)
- Vectors (how information moves and is transformed)
- Destinations (who receives outputs and acts on them)
- Boundary objects (points where information crosses between actors, systems, or contexts)
- Decision points (where outputs become decisions or recommendations)

**Bias location is the primary analytical task.** For each element in the pathway, identify:
- Whether bias can be introduced at that point
- What form that bias takes (e.g., sampling bias, labeling bias, feedback loops, proxy variables, interface framing, authority assumptions)
- Whether the bias is introduced fresh, inherited from an earlier stage, or emergent from the combination of multiple pathway elements

The goal is to be **exhaustive in identifying candidate locations** — do not limit yourself to the most obvious entry points. Every transformation, handoff, and design choice in the pathway is a potential bias site.

**Required artifact:** For each deployment, produce either:
- a structured pathway diagram (annotated with bias locations), or
- a structured table listing each pathway stage, the transformation occurring, and the bias risk at that stage

**Comparative requirement:** After mapping all three deployments, identify:
- which bias locations are consistent across all deployments
- which are specific to particular deployment configurations
- where changing the deployment context creates new bias risks that did not exist before

---

### 5. Decision Pathway Analysis

For each deployment, trace how the system's output becomes a consequential decision:
- What does the system produce?
- Who receives that output, and with what authority to act on it?
- What happens if the output is wrong, biased, or incomplete?

Identify:
- where human judgment enters or exits the decision pathway
- where accountability is clear, diffused, or absent
- how the mediation structure shapes who is visible and who is not to the decision-maker

---

### 6. Harm Analysis

Across all three deployments:

**Direct harm**
- What harms are directly traceable to the system's output?

**Indirect harm**
- What harms emerge downstream, through the decisions or structures the system feeds into?
- Identify at least one indirect harm pathway

**Distribution**
- Who is harmed, and who is not?
- Are harms evenly distributed or concentrated in particular populations?

Connect this section explicitly to the harm vocabulary from prior course work.

---

### 7. Critical Reflection

Respond to the following question in **400–600 words**:

> Given what you have found, where does responsibility for bias-related harm sit — in the system, in the people who deploy it, or in the structures that surround it?

Ground your response in your deployment analysis and the required readings. You may reference the EU AI Act if relevant, but regulatory classification is not the point — the question is about responsibility and structure.

---

## Deliverables

Submit via GitHub:
- main document (.md or .pdf)
- any diagrams
- Zotero entries

Recommended filename: `08-bias-decision-harm.md`

---

## Assessment Criteria

### Bias and Fairness Synthesis
- Excellent: defines terms precisely, identifies a genuine tension, connects directly to the selected system
- Competent: definitions present, connection to system partial
- Needs Revision: generic or disconnected from the readings

### Deployment Scenarios
- Excellent: distinct, well-motivated, variation is analytically meaningful
- Competent: scenarios differ but variation is surface-level
- Needs Revision: scenarios are too similar or changes are not explained

### Mediation Pathway and Bias Location
- Excellent: pathway fully mapped for each deployment; bias locations identified at multiple stages with specific descriptions; comparative analysis identifies what is consistent vs. deployment-specific
- Competent: pathway present and some bias locations identified; comparative element partial
- Needs Revision: pathway incomplete or bias locations limited to one or two obvious points

### Decision Pathway
- Excellent: clear account of how outputs become decisions; accountability and visibility mapped
- Competent: pathway present but accountability unclear
- Needs Revision: missing or superficial

### Harm Analysis
- Excellent: direct and indirect harms identified; distribution analyzed; connected to course vocabulary
- Competent: harms named but not traced or distributed
- Needs Revision: vague or incomplete

### Critical Reflection
- Excellent: takes a clear position, grounded in analysis and readings
- Competent: position present but weakly supported
- Needs Revision: restates the question without engaging it

### Research Integration
- Excellent: sources actively inform analysis throughout
- Competent: sources cited but not integrated
- Needs Revision: minimal or absent

---

## Notes

This assignment is not asking you to resolve questions about bias and harm. It is asking you to locate them — to identify precisely where in a system's structure and deployment context they arise, and to reason about what follows from that.

You are expected to:
- use the readings as analytical tools, not background
- make your reasoning visible
- be specific rather than comprehensive

---

End of Assignment

