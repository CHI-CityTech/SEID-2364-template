# SEID2364 Unit 10 Signal Tracking Game
## Master Source: System + Pilot Content

Purpose: this is the single working source for designing, testing, and evaluating the Unit 10 wiki activity.

Use this document for two tasks:
- capability assessment with ChatGPT as primary drafting collaborator
- later splitting into publication documents (assignment instructions, wiki pages, facilitator notes)

---

# 1. System Layer (Stable)

This layer defines the game architecture independent of scenario domain.

## 1.1 Page Types

1. Course wiki home page (`Home`)
2. Exercise home page (`Unit-10-Signal-Tracking-Game`)
3. Node pages (spaces where signals are transformed)
4. Agent pages (reference layer)
5. Student signal cards (student-generated traversal records)

## 1.2 Naming Conventions

- Exercise home: `Unit-10-Signal-Tracking-Game`
- Nodes: `Node-[Space-Name]`
- Agents: `Agent-[Agent-Name]`
- Student signal records: `Signal-[StudentName]-Loan-[SignalID]`

Examples:
- `Signal-AnaGarcia-Loan-01`
- `Signal-JamalIbrahim-Loan-01`

## 1.3 Linking Rules

- Each transition entry should reference its `Parent Transition ID` to preserve lineage.
- Each transition entry should link forward to the next node when known.
- Branch transitions should include `Branch ID` and `Branch Status` to keep divergence explicit.
- Traversal linkage is signal-owned: branch lineage and next-node routing are recorded on the signal record page.
- Node and agent pages are reference layers and may include optional student observations, but they do not prescribe path sequence.

## 1.4 Student Edit Boundaries

- Students create and edit only their own signal record pages.
- Students may append observations to the designated section on node pages.
- Student observation add-ons should be concise and include: observed pattern, likely distortion or temporal issue, and one link back to the relevant transition entry.
- Students do not edit core node definitions.
- Students do not edit agent definitions.

## 1.5 Required Student Output

- One evolving signal record page that tracks every transition taken by the signal
- At least 1 branch decision
- EDOCA at each step (signal and space)
- For each transition, document the vector transmission mechanism and the critical components of the arrival space
- For each transition, document temporal condition, persistence, delay relevance, and temporal trust impact
- For each transition, include explicit links to node, relevant agents, course materials, and authoritative sources, plus Zotero reference links (existing or newly added)
- Final trust reflection: "How much can D trust S based on V?"

---

# 2. Pilot Content Layer (Loan/Lending Scenario)

This layer provides the concrete first scenario used to test the system.

## 2.1 Pilot Signal Definition

- Signal: loan application data representing an applicant
- Primary destination goal: fair and accurate lending decision
- Starting trust level (recommended default for class): 70/100

## 2.2 Pilot Core Pathway

1. `Node-Applicant-Concept`
2. `Node-Application-Form`
3. `Node-AI-Scoring`
4. `Node-Lending-Officer`
5. `Node-Decision`

Optional branch:
- `Node-Appeal`

---

# 3. Fully Defined Node Content (Pilot)

## 3.1 Node-Applicant-Concept

### Space Description
Applicant assembles self-representation before formal submission.

### Accepted Signal Forms
- personal narrative
- informal financial self-assessment
- employment and housing context

### Transformation (Vector)
Unstructured personal context becomes a pre-application conceptual profile.

### Constraints
- incomplete self-knowledge
- unequal literacy about lending criteria
- social pressure to self-edit

### Access
Applicant only.

### Authority
Applicant controls initial framing and disclosure choices.

### Observability
Low institutional observability.

### Relevant Agents
- `Agent-Applicant`

### External Influences
- prior lending experiences
- peer advice
- perceived discrimination risk

### Distortion Risks
- omission of relevant context
- strategic over/understatement
- mismatch between lived reality and expected form categories

### Possible Outputs
- partial profile
- disclosure strategy
- confidence/hesitation state

### Next Nodes
- `Node-Application-Form`

### Observed Patterns (Student Contributions)
Students append only.

## 3.2 Node-Application-Form

### Space Description
Institutional interface where applicant data is encoded into required schema.

### Accepted Signal Forms
- text fields
- dropdown categories
- numeric financial entries
- uploaded documents

### Transformation (Vector)
Context-rich applicant representation is compressed into structured fields.

### Constraints
- rigid field options
- mandatory/optional asymmetry
- UX friction and form assumptions

### Access
Applicant enters; institution configures form.

### Authority
Institution controls schema and validation rules.

### Observability
Medium. Applicant sees interface, not downstream feature engineering.

### Relevant Agents
- `Agent-Applicant`
- `Agent-Lending-Institution`

### External Influences
- compliance requirements
- risk policy
- product design defaults

### Distortion Risks
- category forcing
- missing nuance
- input errors from ambiguity

### Possible Outputs
- structured application record
- validation error logs
- missing-value profile

### Next Nodes
- `Node-AI-Scoring`

### Observed Patterns (Student Contributions)
Students append only.

## 3.3 Node-AI-Scoring

### Space Description
Automated risk estimation from structured application features.

### Accepted Signal Forms
- tabular feature vectors
- engineered variables
- bureau-derived indicators

### Transformation (Vector)
Application features are transformed into a score, rank, or risk class.

### Constraints
- model architecture and training data limits
- threshold policy
- feature availability and quality

### Access
Institutional system and model operators.

### Authority
Institution defines model use and cutoffs; model executes scoring logic.

### Observability
Variable. High internal telemetry; low external transparency.

### Relevant Agents
- `Agent-AI-Model`
- `Agent-Lending-Institution`
- `Agent-Credit-Bureau`

### External Influences
- historical bias in training data
- vendor constraints
- regulatory scrutiny

### Distortion Risks
- proxy discrimination
- data drift
- confidence overstatement

### Possible Outputs
- risk score
- recommendation band
- explanation artifact (if available)

### Next Nodes
- `Node-Lending-Officer`
- `Node-Decision` (automated path, if policy allows)

### Observed Patterns (Student Contributions)
Students append only.

## 3.4 Node-Lending-Officer

### Space Description
Human decision review combining model output and contextual judgment.

### Accepted Signal Forms
- model score
- application summary
- notes and exceptions

### Transformation (Vector)
Model output is interpreted, weighted, and translated into a recommendation.

### Constraints
- workload pressure
- policy targets
- incomplete explanation access

### Access
Loan officers and authorized managers.

### Authority
Officer may approve, deny, or request additional documentation within policy bounds.

### Observability
Medium. Internal notes may be visible internally, limited externally.

### Relevant Agents
- `Agent-Loan-Officer`
- `Agent-Lending-Institution`
- `Agent-AI-Model`

### External Influences
- productivity metrics
- institution risk appetite
- fairness oversight climate

### Distortion Risks
- automation bias
- selective override behavior
- inconsistent exception handling

### Possible Outputs
- approve recommendation
- deny recommendation
- conditional or pending recommendation

### Next Nodes
- `Node-Decision`
- `Node-Appeal` (if reconsideration path exists)

### Observed Patterns (Student Contributions)
Students append only.

## 3.5 Node-Decision

### Space Description
Formal institutional outcome communication to applicant.

### Accepted Signal Forms
- final decision code
- summary reason statement
- terms and conditions

### Transformation (Vector)
Internal recommendation and policy logic become an externally communicated decision.

### Constraints
- legal communication requirements
- template reason language
- explainability limits

### Access
Institution sends; applicant receives.

### Authority
Institution finalizes and issues outcome.

### Observability
High for outcome, low for full process provenance.

### Relevant Agents
- `Agent-Lending-Institution`
- `Agent-Applicant`

### External Influences
- adverse action disclosure rules
- product constraints
- communication policy

### Distortion Risks
- reason abstraction hides causal chain
- ambiguous denial rationale
- trust collapse from opaque outcomes

### Possible Outputs
- approval
- denial
- conditional approval
- referral to appeal

### Next Nodes
- `Node-Appeal`

### Observed Patterns (Student Contributions)
Students append only.

## 3.6 Node-Appeal (Optional Branch)

### Space Description
Post-decision pathway for contesting or re-evaluating outcomes.

### Accepted Signal Forms
- applicant rebuttal
- corrected documents
- supplementary context

### Transformation (Vector)
Decision outcome is challenged and re-contextualized through additional evidence.

### Constraints
- strict deadlines
- burden of proof asymmetry
- limited applicant guidance

### Access
Applicant initiates; institution adjudicates.

### Authority
Institution may uphold, modify, or reverse prior decision.

### Observability
Medium; process visibility varies by institution.

### Relevant Agents
- `Agent-Applicant`
- `Agent-Lending-Institution`
- `Agent-Loan-Officer`

### External Influences
- ombudsperson or complaint channels
- legal counsel availability
- regulator complaint processes

### Distortion Risks
- evidentiary mismatch
- inconsistent reconsideration standards
- procedural opacity

### Possible Outputs
- decision upheld
- decision modified
- decision reversed

### Next Nodes
- `Node-Decision`

### Observed Patterns (Student Contributions)
Students append only.

---

# 4. Fully Defined Agent Content (Pilot)

## 4.1 Agent-Applicant

### Role
Originating party whose life context is encoded into the lending process.

### Goals
- obtain fair access to credit
- preserve dignity and agency
- understand outcome rationale

### Authority
Controls disclosure choices and appeal initiation.

### Access
Own documents, personal financial context, application interface.

### Observability
High visibility of own context; low visibility into institutional modeling.

### Constraints
- information asymmetry
- time and documentation burden
- digital literacy differences

### Typical Effects on Signals
- contextual enrichment
- selective disclosure
- corrective updates during appeal

## 4.2 Agent-Lending-Institution

### Role
System owner defining policy, workflow, and final adjudication environment.

### Goals
- manage default risk
- meet compliance obligations
- maintain operational efficiency

### Authority
Sets criteria, thresholds, workflow controls, and communication templates.

### Access
Full internal application pipeline and outcome controls.

### Observability
High internal observability, especially at aggregate level.

### Constraints
- regulation
- market competition
- legacy infrastructure and governance quality

### Typical Effects on Signals
- schema standardization
- thresholding
- explanation compression in outbound messaging

## 4.3 Agent-AI-Model

### Role
Operational scoring mechanism translating input features into risk estimates.

### Goals
Optimize target performance under institutional objectives.

### Authority
No independent authority; executes within configured policy and deployment context.

### Access
Model input features and internal inference state.

### Observability
Potentially high internal telemetry; externally constrained interpretability.

### Constraints
- training data history
- feature engineering choices
- model drift and monitoring maturity

### Typical Effects on Signals
- numerical reduction of complex context
- amplification of historical patterns
- confidence shaping for downstream humans

## 4.4 Agent-Loan-Officer

### Role
Human reviewer translating model outputs and policy rules into case-level decisions.

### Goals
- make consistent decisions
- balance efficiency with fairness
- reduce avoidable harms and reversals

### Authority
Can approve/deny/request-info within policy boundaries.

### Access
Application dossier, score outputs, limited explanation artifacts.

### Observability
Case-level visibility higher than applicant, lower than full system owner.

### Constraints
- time pressure
- institutional incentives
- partial transparency into model internals

### Typical Effects on Signals
- interpretive weighting
- selective overrides
- note-based contextual adjustments

## 4.5 Agent-Regulator

### Role
External governance agent setting legal and supervisory boundaries.

### Goals
- enforce fairness and disclosure standards
- reduce systemic discrimination
- maintain trust in lending institutions

### Authority
Can investigate, require disclosures, and impose corrective actions.

### Access
Often episodic and indirect; depends on reporting and audit powers.

### Observability
Macro-level observability generally higher than case-level immediacy.

### Constraints
- legal mandate boundaries
- resource limits
- lag between harm and enforcement response

### Typical Effects on Signals
- compliance pressure on feature use
- disclosure requirements
- process redesign incentives

## 4.6 Agent-Credit-Bureau

### Role
External data provider supplying historical credit indicators.

### Goals
- provide standardized risk-relevant data
- maintain data reliability and market trust

### Authority
Controls data collection and correction workflows for bureau records.

### Access
Large historical credit datasets and correction systems.

### Observability
Strong record-level observability, limited visibility into lender-specific model usage.

### Constraints
- data accuracy disputes
- update latency
- legal obligations for correction handling

### Typical Effects on Signals
- normalization of applicant history
- persistence of historical errors
- baseline framing of risk before lender modeling

---

# 5. Signal Card Template (Operational)

Students copy this template from assignment materials and create one evolving wiki page per signal.

```markdown
# Signal Record: [Student Name] - [Signal Name]

Page name: Signal-[StudentName]-Loan-[SignalID]

## Signal Identity
Student:
Signal Name:
Scenario:
Signal ID:
Status: Active

## Current State Snapshot
Current Node:
Current Representation:
Current Trust Level:
Total Transitions So Far:
Cumulative Distortion Level:

## End-of-Path Synthesis
Overall Pathway Summary:
What accumulated along the way?
Where did trust degrade, stabilize, or recover?
How much can D trust S based on V?

## Transition Log

### Transition [Number]
From Node:
To Node:
Vector / Edge Transmission Description:
What is being transmitted across this edge:
How this vector transforms the signal:

#### SVD
S:
V:
D:

#### Input Signal State

#### Output Signal State

#### Signal Purpose At This Step

#### Temporal Mediation Notes
Temporal Condition:
Persistence State:
Delay Characterization:
Expiration Risk:
Retrieval Context:
Temporal Trust Impact:

#### Raw / Curated / Hybrid

#### Integrity (Pattern Preservation)
Preserved:
Lost:
Distorted:

#### EDOCA (Signal)
Energy:
Distortion:
Observability:
Control:
Authority:

#### EDOCA (Space)
Energy:
Distortion:
Observability:
Control:
Authority:

#### Arrival Space Critical Components
Space Type (conceptual / physical / virtual / institutional / blended):
Space Description:
Constraints:
Access:
Authority:
Relevant Agents:
Distortion Risks:
How this space connects to other spaces and agents:

#### Agent Influence
Which agents influenced this transformation?
How did their goals affect the signal?

#### Trust Update
Previous:
Change:
New:

#### Why This Transition Matters

#### Next Node
[link]
```

---

# 6. Publication Split Plan (Later)

When ready to publish, split this master source into:

1. Student assignment instructions
2. Wiki exercise home page
3. Node pages
4. Agent pages
5. Facilitator notes and evaluation rubric

This master file remains the source of truth for future iterations and domain variants.
