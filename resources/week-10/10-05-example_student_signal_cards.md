# SEID2364 Unit 10
## Example Student Signal Record

This file provides a worked example of what one evolving student signal record might look like in the Unit 10 pilot activity.

The example below is illustrative. It is not the only correct answer.

---

# Example Signal Record

```markdown
# Signal Record: Ana Garcia - Applicant Profile

Page name: Signal-AnaGarcia-Loan-01

## Signal Identity
Student: Ana Garcia
Signal Name: Applicant Profile
Scenario: Loan application pathway
Signal ID: Loan-01
Status: Active

## Current State Snapshot
Current Node: Node-AI-Scoring
Current Representation: Structured application record transformed into a model-ready feature set
Current Trust Level: 45
Total Transitions So Far: 2
Cumulative Distortion Level: Moderate to High

## End-of-Path Synthesis
Overall Pathway Summary: [complete when the signal finishes its path]
What accumulated along the way? [complete at the end]
Where did trust degrade, stabilize, or recover? [complete at the end]
How much can D trust S based on V? [complete at the end]

## Transition Log

### Transition 02
From Node: Node-Application-Form
To Node: Node-AI-Scoring
Vector / Edge Description: Automated feature processing and model scoring

#### SVD
S: Structured application record
V: Automated feature processing and model scoring
D: Risk score and recommendation band

#### Input Signal State
Ana's application exists as a structured institutional record with categorized fields and uploaded documentation.

#### Output Signal State
Ana's application is translated into a feature vector and output as a risk score plus recommendation band.

#### Temporal Mediation Notes
Temporal Condition (fresh / delayed / stale / expired): Delayed
Persistence State (ephemeral / stored / archived): Stored
Delay Characterization (none / short / moderate / high, with context): Moderate; batch scoring introduces delay relative to applicant expectations
Expiration Risk (none / low / moderate / high): Moderate; profile can become stale if underlying circumstances change before review
Retrieval Context (who can retrieve this signal, when, and under what conditions): Internal lending systems can retrieve continuously; applicant access is limited to summarized outputs
Temporal Trust Impact (how timing changed trust at this step): Trust drops because asynchronous scoring and limited retrieval rights reduce contestability in real time

#### Signal Purpose At This Step
To estimate lending risk in a standardized and scalable way.

#### Raw / Curated / Hybrid
Curated

#### Integrity (Pattern Preservation)
Preserved:
- debt-to-income relationship
- credit history proxies
- standardized income and obligation fields

Lost:
- explanation for recent income volatility
- contextual differences hidden by proxy variables
- applicant intent and future trajectory

Distorted:
- historical patterns may substitute for present circumstances
- proxy variables may overstate risk for structurally disadvantaged applicants

#### EDOCA (Signal)
Energy: High computational and institutional energy; low applicant energy at this stage
Distortion: High
Observability: Low for applicant, high internally
Control: Low for applicant, high institutional control over deployment
Authority: High institutional authority over scoring criteria and deployment

#### EDOCA (Space)
Energy: High system energy concentrated in model execution and policy thresholds
Distortion: High risk
Observability: Uneven
Control: High institutional control
Authority: Centralized institutional authority with limited external contestability

#### Agent Influence
Which agents influenced this transformation?
The AI model, the lending institution, and external credit data providers all shaped the output.

How did their goals affect the signal?
The institution sought efficient risk sorting, while the model translated prior patterns into present judgments. This can increase consistency, but it can also carry forward hidden historical bias.

#### Trust Update
Previous: 60
Change: -15
New: 45

#### Why This Transition Matters
The score may be useful, but it is further removed from the applicant's lived reality than the original signal. Trust decreases because the signal becomes more legible to the institution while becoming less interpretable and less contestable for the applicant.

#### Next Node
[Node-Lending-Officer]

### Transition 01
From Node: Node-Applicant-Concept
To Node: Node-Application-Form
Vector / Edge Description: Translation into a formal lending application form

#### SVD
S: Applicant self-understanding of her financial situation
V: Translation into a formal lending application form
D: Structured application record

#### Input Signal State
Ana's financial reality is held as a mix of narrative self-understanding, informal budgeting knowledge, and partial assumptions about what the lender wants to know.

#### Output Signal State
Ana's financial reality is represented as a mix of narrative, categorical selections, and numeric form entries.

#### Temporal Mediation Notes
Temporal Condition (fresh / delayed / stale / expired): Fresh
Persistence State (ephemeral / stored / archived): Stored
Delay Characterization (none / short / moderate / high, with context): Short; immediate form capture but downstream review may lag
Expiration Risk (none / low / moderate / high): Low at submission, rising if review is delayed
Retrieval Context (who can retrieve this signal, when, and under what conditions): Applicant can review during completion; institution can retrieve after submission under internal access controls
Temporal Trust Impact (how timing changed trust at this step): Small trust decrease due to expected lag between submission and downstream interpretation

#### Signal Purpose At This Step
To convert lived financial circumstances into a form the lending system can process.

#### Raw / Curated / Hybrid
Hybrid

#### Integrity (Pattern Preservation)
Preserved:
- employment status
- monthly income estimate
- declared housing costs

Lost:
- context about irregular gig income
- informal family support network
- recent improvement in financial stability

Distorted:
- financial precarity is made to look more static than it really is
- dropdown categories flatten differences in employment type

#### EDOCA (Signal)
Energy: Moderate applicant and institutional energy focused on data entry and normalization
Distortion: Moderate
Observability: Medium
Control: Shared between applicant and institution
Authority: Institution defines submission schema and validation standards

#### EDOCA (Space)
Energy: Moderate procedural energy through interface constraints and validation rules
Distortion: Moderate
Observability: Medium
Control: High institutional control
Authority: Institution controls form architecture and acceptable inputs

#### Agent Influence
Which agents influenced this transformation?
The applicant chose what to disclose, but the lending institution shaped the structure through the form design.

How did their goals affect the signal?
Ana aimed to present herself accurately and favorably. The institution aimed to standardize inputs for downstream review and scoring.

#### Trust Update
Previous: 70
Change: -10
New: 60

#### Why This Transition Matters
Some important information is preserved, but the form compresses Ana's situation into categories that miss important nuance. The destination can still trust the signal somewhat, but less than at the source because context has already been thinned.

#### Next Node
[Node-AI-Scoring]
```

---

## Teaching Note

This example is intentionally concise. In practice, students may produce shorter or longer entries, but they should always make the vector transition, the losses, and the trust update explicit.

The newest transition appears at the top of the transition log, while older transitions remain below as part of the signal's accumulated history.