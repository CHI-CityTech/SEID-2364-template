# Signal Record Instructions

> Template file: [Signal Record Template](10-03-signal_card_template.md)

These instructions explain how to create and maintain your signal record in the Unit 10 wiki activity.

---

## Overview

You will create one wiki page and keep updating it as your signal moves through the system.

Your page has three parts:
1. **Signal Identity** — who you are and what your signal is
2. **Current State Snapshot** — the live top-of-page summary, updated after every transition
3. **Transition Log** — your history of vector traversals, newest at the top

---

## Creating Your Page

1. Open the [Signal Record Template](10-03-signal_card_template.md)
2. Copy **Part A** (the page header)
3. Create a new wiki page using this naming convention: `Signal-[StudentName]-Loan-[SignalID]`
4. Paste Part A and fill in the Signal Identity fields
5. Leave Current State Snapshot and End-of-Path Synthesis blank for now

---

## Adding a Transition

Each time your signal passes through a vector (an edge between two nodes):

1. Copy **Part B** (the transition entry block) from the template
2. Paste it at the **top** of the Transition Log, above any previous transitions
3. Fill in every field
4. Update the **Current State Snapshot** at the top of the page to reflect where your signal now is

---

## Field-by-Field Guide

### Signal Identity

| Field | What to write |
|-------|--------------|
| Student | Your name |
| Signal Name | A short descriptive name for your signal |
| Scenario | Loan application pathway |
| Signal ID | Loan-01 (or 02 etc. if you track more than one) |
| Status | Active while in progress; Complete when finished |

---

### Current State Snapshot

Update this every time you add a new transition. It should always reflect where the signal is right now.

| Field | What to write |
|-------|--------------|
| Current Node | The node your signal currently occupies |
| Current Representation | A brief description of what form the signal is in now |
| Current Trust Level | The trust score after your most recent transition |
| Total Transitions So Far | Count of transitions completed |
| Cumulative Distortion Level | Low / Moderate / High / Very High |

---

### End-of-Path Synthesis

Leave blank until your signal has completed its path. Then write a concise summary addressing:

- What happened to the signal overall?
- What was lost or distorted that cannot be recovered?
- Where did trust shift most significantly, and why?
- Final answer: how much can D trust S based on V?

---

### Transition Entry Fields

**From Node / To Node**
The nodes on either side of the vector you are reporting on.

**Vector / Edge Description**
A short label for the mechanism of transformation. Examples: "automated scoring model," "form submission," "human review."

---

**SVD**
- S: what the signal is at the start of this vector
- V: the vector (transformative mechanism) itself
- D: what the signal becomes at the end of this vector

---

**Input Signal State**
Describe concretely what the signal looked like before entering this vector. What form was it in? What information did it carry?

**Output Signal State**
Describe concretely what the signal looks like after traversing this vector.

---

**Signal Purpose At This Step**
What is this signal supposed to accomplish at this point in the pathway?

**Raw / Curated / Hybrid**
- Raw: unprocessed, as close to source as possible
- Curated: deliberately shaped for a purpose
- Hybrid: partially processed

---

**Integrity (Pattern Preservation)**
- Preserved: what meaningful information survived the transition intact
- Lost: what meaningful information was dropped, omitted, or made inaccessible
- Distorted: what information was changed in ways that misrepresent the original

---

**EDOCA (Signal)**
Assess the signal itself as it crosses this vector.

| Dimension | What to consider |
|-----------|-----------------|
| Energy | What force or resource drives this transformation? |
| Distortion | How much does the signal change in ways not intended? |
| Observability | How visible is this signal to the actors involved? |
| Control | Who can shape what happens to the signal here? |
| Alignment | How well does the signal's current form serve its stated purpose? |

**EDOCA (Space)**
Assess the space (node) that the signal is entering.

Same dimensions, but now applied to the environment the signal is entering rather than the signal itself.

---

**Actor Influence**
- Name which actors shaped what happened on this vector
- Explain how each actor's goals or constraints affected the signal

---

**Trust Update**
- Previous: trust level before this transition
- Change: positive number if trust increased, negative if decreased
- New: resulting trust level

The starting trust level for this scenario is 70.

Trust changes should be justified by what actually happened to the signal. A small distortion may warrant –5. A major loss of interpretability may warrant –20 or more.

---

**Why This Transition Matters**
Write one short paragraph explaining what this vector reveals about how the system works, and why the change in signal integrity or trust is significant.

---

**Next Node**
Link to the next node page your signal will enter.

---

## Naming Convention

`Signal-[StudentName]-Loan-[SignalID]`

| Part | Format | Example |
|------|--------|---------|
| StudentName | FirstnameLastname, no space | AnaGarcia |
| Loan | fixed label for this pilot | Loan |
| SignalID | two-digit number | 01 |

Full example: `Signal-AnaGarcia-Loan-01`
