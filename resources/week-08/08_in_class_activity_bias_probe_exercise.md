# SEID 2364 – In-Class Activity
## Bias Probe Exercise

---

## Purpose

This activity introduces a controlled method for observing how bias operates within AI-mediated systems.

You will apply **one small, intentional change** to a system description and observe how outputs shift. The goal is not to determine correctness, but to identify how variation affects outcomes.

This exercise prepares you for **Assignment 08**, where you will analyze how systems change across different deployments.

---

## Setup

Use the system you developed in Assignment 7.

You will interact with an AI system (e.g., ChatGPT or equivalent) to evaluate your system description.

**Required Prompt Template (use for all submissions in this activity):**

> Using the EU AI Act, classify the following system and explain your reasoning. Identify the relevant risk category and justify your answer using the structure of the Act. Cite relevant articles or categories where possible.

**Important:**
- You must use this exact prompt for both the baseline and the modified version
- Do not ask for general ethical analysis
- Do not change the wording of the prompt

---

## Instructions (with Example)

### Step 1 — Baseline

Write a clear description of your system and submit it to the AI using the required prompt template above.

**Example (Bank Loan System):**

> Using the EU AI Act, classify the following system and explain your reasoning. Identify the relevant risk category and justify your answer using the structure of the Act. Cite relevant articles or categories where possible.
> 
> A bank uses an AI system to evaluate loan applications based on applicant financial data and credit history. The system produces a recommendation for approval or denial.

Record the response.

Capture:
- classification (if given)
- reasoning or explanation
- tone or confidence

---

### Step 2 — Controlled Variation (One Change Only)

Modify **one element only** of your system.

**Do not rewrite the system. Do not change multiple variables.**

Valid types of changes:
- user group
- decision authority (advisory → automated)
- institutional context
- level of consequence

**Example (Change: Decision Authority Only):**

Baseline:
> AI provides a recommendation to a human loan officer

Modified:
> AI automatically approves or denies the loan without human review

Submit the modified version to the AI using the **same required prompt template** (unchanged).

---

### Step 3 — Comparison

Compare the baseline and modified outputs.

Identify:
- What changed?
- What stayed the same?
- Did classification shift?
- Did justification change?

**Example Observations:**
- AI shifts from "decision support" language to "automated decision"
- Increased confidence in outcome
- Possible shift toward higher risk classification

---

### Step 4 — Bias Identification

Based on the difference, identify:

- Where bias may be entering the system
- Whether the bias is:
  - introduced
  - inherited
  - emergent

- Whether the change produced:
  - uneven outcomes
  - different assumptions
  - shifts in reasoning or tone

**Example:**
- Removal of human oversight may amplify existing bias in training data
- System assumes data is sufficient for decision-making
- Applicants may be treated differently without recourse

---

### Step 5 — Reflection (Short)

Respond briefly:

- What does this suggest about how the system operates?
- Where in the system might this change be occurring?
- Does this change increase or decrease trust in the system?

**Example:**
- Trust may decrease due to lack of human oversight
- Bias may become less visible but more impactful

---

## Output (for Google Doc or Submission)

Each student should provide:

- Baseline prompt (short)
- Modified prompt (short)
- Key difference observed (1–2 sentences)

---

## Notes

- This is a **controlled experiment**, not an optimization task
- Only change **one variable at a time**
- Do not iterate repeatedly
- Focus on observing differences, not improving results

---

## Time Allocation

Total: ~20 minutes

- Baseline + variation: 10 minutes
- Comparison + reflection: 10 minutes

---

## Optional Extension (If Time Permits)

Apply a **second, different single-variable change** and compare results again.

Example:
- Change user group (individual applicant → small business applicant)

Observe whether effects are consistent or different.

---

End of Activity

