# SEID 2364 – Assignment 9
## Mediation Pathways, Capability, and Responsibility

Instructor: Dr. David B. Smith  
Course: SEID 2364 – Societal and Ethical Impacts of Data Science  
Date Assigned: Week 9  
Due: Week 10

---

## Purpose

In prior assignments, you:

- identified harm (Assignment 3)
- evaluated harm using ethical frameworks (Assignment 4)
- described systems structurally (Assignment 5)
- traced mediation pathways across physical and virtual space (Assignment 6)
- evaluated systems under regulation (Assignment 7)
- analyzed bias across deployments (Assignment 8)

This assignment shifts the focus again.

> Not just *where bias or harm exists*, but *how harm emerges through mediation pathways under real conditions of system capability*.

Drawing from strategic analysis (Sun Tzu, Clausewitz), we treat ethics not as intention, but as **capability under constraint**.

A system is therefore evaluated by:

- what it **can do**
- under **actual conditions of access, visibility, and control**

---

## EDOCA: Dimensions of Mediation Assessment

> In BBS terms, a mediation pathway can be understood as **S → V → D**, where the **Vector (V)** is the **transition** that transforms a source state into a destination state.
>
> The goal of analysis is to evaluate the **efficacy of V**: its ability to **maintain the intended signal from S to D** under real conditions.

This assignment introduces **EDOCA** as a formal diagnostic framework for evaluating mediation transitions.

EDOCA is ordered intentionally to reflect how mediation is analyzed:

- **Effort** — what resources are applied
- **Distortion** — what happens to the signal as a result
- **Observability** — who can see the result
- **Control** — who can act on the result
- **Authority** — who can permit or constrain action

This ordering reflects a causal chain: resources produce transformations, transformations produce distortion, distortion produces outcomes that are variably visible, actionable, and governable.

At each critical transition, you must evaluate:

- **Effort / Energy** — the cost required to produce or sustain the transition (time, computation, human labor, infrastructure, attention)
- **Distortion (Fidelity)**
- How effectively does this transition (V) preserve the intended signal from S to D? — how much the signal changes during the transition (noise, ambiguity, translation loss, compression, abstraction, representation mismatch)
- **Observability** — who can see or understand what is happening, and to what degree
- **Control** — who can initiate, modify, redirect, or influence the transition
- **Authority** — who can assign, enable, restrict, or halt capability

> EDOCA is applied at **specific transitions (Vectors, V)**, not to the system as a whole.
>
> Each transition (V) is evaluated based on how well it preserves or transforms the signal from **Source (S)** to **Destination (D)**.

Effort and distortion are deeply related but not identical. In some cases, increased effort (validation, redundancy, higher computation, human review) may reduce distortion and improve fidelity. In other cases, additional transformations or processing may preserve or amplify distortion. You should therefore ask not only how much effort is present, but whether that effort improves or degrades the quality of the mediated signal.

---

## Assignment Overview

You will analyze a real-world AI-related incident by reconstructing the **mediation pathways that produced a harmful outcome**.

Your task is to:

- describe the event clearly (no analysis)
- identify all major **agents** involved
- reconstruct **multiple mediation pathways**
- identify **critical transitions**
- apply **EDOCA at those transitions**
- evaluate **capability vs intent**
- analyze how **responsibility is distributed across the system**

---

## Part 0 – Repository Preparation

Create a new file in your repository:

`assignment-09/pathways.md`

All work for this assignment must appear in this file.

---

## Part 1 — Narrative Description (Descriptive Only)

Provide a narrative answering:

> What happened, to whom, by whom, and what was harmed?

Requirements:

- 1–2 paragraphs
- descriptive only (no analysis)

Do NOT include:

- explanations
- causes
- ethical evaluation

---

## Part 2 — Originating Agents

Identify the primary agents involved.

Include (where applicable):

- End user / operator  
- AI system (LLM / agent)  
- AI developer / manufacturer  
- Platform / infrastructure (APIs, cloud systems)  
- Intermediate tools or environments  

Each agent may initiate **distinct mediation pathways**.

---

## Part 3 — Mediation Pathways (Multi-Agent)

Construct mediation pathways organized by **originating agent**.

Requirements:

- At least **2 agents** must be analyzed
- Each agent must have **at least one pathway** (max 2–3 per agent)
- Each pathway must include **minimum 3 stages**
- Focus on **critical pathways only**

Format:

```
Agent → Stage 1 → Stage 2 → Stage 3 → Outcome
```

For each stage, identify:

- Space type: Personal / Local / Remote / Unreachable
- Transition type (where relevant):
  - physical ↔ virtual
  - symbolic ↔ computational
  - local ↔ remote

---

## Part 4 — EDOCA Assessment of Critical Transitions

> Each selected transition corresponds to a **Vector (V)** in an S → V → D structure. Your task is to evaluate how effectively that transition maintains or transforms the signal between states.

Select at least **two transitions** across your pathways.

For each:

### 1. Identify the Transition (Vector V)
- What state change occurs (S → D)?
- What transformation (V) produces that change?
- Between which spaces or representations does this occur?

### 2. Apply EDOCA

**Effort / Energy**  
- What resources are required?  
- Who provides them?

**Observability**  
- Who can observe this transition?  
- What is hidden, partial, delayed, or opaque?

**Control**  
- Who initiates or modifies the transition?  
- Who is read-only?

**Authority**  
- Who can enable, restrict, or halt this transition?  
- Is authority aligned with control?

**Distortion / Fidelity**  
- How does the signal change during this transition?  
- What forms of distortion are introduced, reduced, preserved, or amplified?  
- Does the transition improve fidelity, degrade fidelity, or leave the signal mostly unchanged?

### 3. Synthesis

> How does this EDOCA configuration contribute to potential harm?

---

## Part 5 — Signal and State Integrity

Because distortion is now included directly in EDOCA, this section should focus on the consequences of distortion and on the difference between signal failure and state failure.

For selected transitions, identify:

- **Signal degradation / distortion** — already described through the Distortion / Fidelity dimension of EDOCA
- **State divergence** — where the internal system model does not match the actual system state
  - example: the system believes an action succeeded when it did not

Distinguish between:

- **Symbolic failure** — errors introduced during representation, translation, or interpretation
- **State failure** — errors introduced when system state becomes inconsistent with reality
- **Bias** — patterned distortion that systematically affects certain people, groups, outputs, or decisions

Additionally, indicate:

> Where does distortion first appear, and where is it amplified across subsequent transitions?

> At what point does distortion become error, bias, or harm?

---

## Part 6 — Capability vs Intent

- What was the system intended to do?
- What was it capable of doing under actual conditions?

Then answer:

> Is this truly an “unintended consequence”? Why or why not?

---

## Part 7 — Responsibility Distribution

Using your pathways:

- Where does responsibility appear to reside?
- Where does it become distributed or unclear?

Focus on mismatches between:

- Authority
- Control
- Capability

---

## Part 8 — Reflection

Respond briefly:

> How did reconstructing mediation pathways change your understanding of how harm is produced in complex systems?

---

## Example (Outline Only)

### Originating Agent — Developer

Developer → Prompt (Local symbolic) → AI Agent (Remote computational) → API (Remote infrastructure) → System State Change

### Originating Agent — AI System

Internal State → Plan Generation → Execution Commands → System State

### Originating Agent — Infrastructure

API Design → Permission Scope → Execution → Data Outcome

---

## Deliverables

Submit to GitHub:

```
/students/yourname/assignment-09/pathways.md
```

---

## Evaluation Criteria

- Pathway clarity and structure  
- Correct identification of agents  
- EDOCA application precision  
- Signal/state distinction accuracy  
- Capability vs intent reasoning  
- Responsibility analysis depth  
- Clarity and organization  

---

## TL;DR

- Describe what happened (no analysis)
- Identify agents
- Build mediation pathways
- Select critical transitions
- Apply EDOCA
- Analyze signal vs state
- Evaluate capability vs intent
- Identify responsibility
- Commit and push

---

## Reminder

> Systems are not evaluated by what they are designed to do, but by what they are capable of doing under real conditions.

