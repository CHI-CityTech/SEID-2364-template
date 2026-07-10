# Wiki Implementation Guide

## Signal Integrity: Mediation Pathway Activity

This document defines the required Wiki structure, page types, and implementation instructions for deploying the asynchronous Signal Integrity activity.

This guide is separate from the Rulebook. The Rulebook defines concepts. This document defines how the system is built and used.

The activity should be understood as having two separate layers:

- The game system: the page structure, naming conventions, linking rules, traversal logic, and contribution workflow
- The game content: the specific scenario, nodes, agents, and signal transformations used in a given run

For the first pilot, the game system remains stable while the game content is built around a loan or lending pathway.

---

# 1. System Overview

The activity is implemented as a **graph of linked Wiki pages**.

There are four primary page types:

1. Wiki Home Page
2. Exercise Home Page
3. Node Pages (Spaces)
4. Agent Pages (Reference Layer)
5. Signal Records (Student-generated pages)

The Wiki Home Page is the landing page for the course wiki as a whole.

The Exercise Home Page is the landing page for this specific activity. It is linked from the Wiki Home Page and can also be distributed directly to students.

Students traverse the system by updating one evolving Signal Record as they move through Node Pages.

---

# 2. Required Wiki Structure

Use a **flat, self-documenting page structure** rather than relying on folders as the primary navigation system.

Create the following top-level pages:

- Home
- Unit-10-Signal-Tracking-Game
- Node-Applicant-Concept
- Node-Application-Form
- Node-AI-Scoring
- Node-Lending-Officer
- Node-Decision
- Node-Appeal (optional branch)
- Agent-Applicant
- Agent-Lending-Institution
- Agent-AI-Model
- Agent-Loan-Officer
- Agent-Regulator
- Agent-Credit-Bureau

Student-created pages should use one evolving signal-record name, for example:

- Signal-AnaGarcia-Loan-01

Path linkage is recorded on the Signal Record page (transition lineage + next node). Node and Agent pages are reference layers and do not enforce a single global sequence.

---

# 3. Exercise Home Page

The Exercise Home Page should be named:

- Unit-10-Signal-Tracking-Game

This page is the home of the exercise, not the home of the wiki.

It must include:

- Activity introduction (you are the signal)
- Use case description (loan system)
- Signal definition
- Signal purpose
- Starting trust level
- Instructions for copying the Signal Record template from the assignment or course resource
- Link to first Node page

This page is the primary entry point for the activity.

It should be linked from the wiki Home page and may also be shared directly with students.

---

# 4. Signal Record Template

Students must copy this template once per signal and then add transitions to the same page.

The template does not need to live as a Wiki page. It can be distributed in the Assignment page or in a repository resource linked from the activity page.

Students copy the template, create one new Wiki page for the signal, and continue through the activity by adding transition entries.

```markdown
# Signal Record: [Student Name] - [Signal Name]

Page name: U10SG-Signal-[StudentName]-Loan-[SignalID]

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

## Branch Registry (update as needed)
- Branch A:
- Branch B:
- Branch C:

### Transition [ID]
Parent Transition ID (or START):
Branch ID:
Branch Status (active / merged / closed):
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

## Temporal Mediation Notes
Temporal Condition:
Persistence State:
Delay Characterization:
Expiration Risk:
Retrieval Context:
Temporal Trust Impact:

#### Signal Purpose At This Step

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

#### Required Links and Research Evidence
Node Page Link:
Relevant Agent Page Link(s):
Course Material Link(s):
Authoritative Source Link(s):
Zotero Link(s) (existing item/collection or newly added item):
```

---

# 5. Node Pages (Spaces)

Each Node represents a **Space**.

Nodes must be pre-created for the use case.

## Required Nodes (Loan Use Case)

- Node-Applicant-Concept
- Node-Application-Form
- Node-AI-Scoring
- Node-Lending-Officer
- Node-Decision
- Node-Appeal (optional branch)

---

## Node Page Template

```markdown
# Node: [Name]

## Space Description

## Accepted Signal Forms

## Transformation (Vector)

## Constraints

## Access

## Authority

## Observability

## Relevant Agents
- [Agent Name] → link
- [Agent Name] → link

## External Influences
- regulation
- market competition
- external data sources

## Distortion Risks

## Possible Outputs

## Next Nodes
- [Node A]
- [Node B]

## Observed Patterns (Student Contributions)
```

Students may only append to the final section. This is a course rule rather than a technical restriction enforced by GitHub Wiki.

Student add-on comments on Node pages should include:
- Observed pattern in this space
- Likely distortion or temporal issue seen in this space
- One link back to the student's relevant transition entry

Student add-on comments on Node pages should include:
- Observed pattern in this space
- Likely distortion or temporal issue seen in this space
- One link back to the student's relevant transition entry

---

# 6. Agent Pages (Reference Layer)

Agent Pages describe agents that influence transformations.

## Required Agent Pages

- Agent-Applicant
- Agent-Lending-Institution
- Agent-AI-Model
- Agent-Loan-Officer
- Agent-Regulator
- Agent-Credit-Bureau

---

## Agent Page Template

```markdown
# Agent: [Name]

## Role

## Goals

## Authority

## Access

## Observability

## Constraints

## Typical Effects on Signals
```

Agent Pages are NOT traversal nodes.

Student add-on comments on Agent pages should include:
- Observed influence pattern for that agent
- Authority boundary or control pattern observed
- One link back to the student's relevant transition entry

---

# 7. Student Workflow

Each student must:

1. Start at the Exercise Home Page
2. Open the template from the assignment or linked course resource
3. Create one Signal Record page using the required naming convention
4. Enter first Node
5. Apply transformation
6. Add a transition entry at the top of Transition Log
7. Include required links to node/agents/materials/sources and Zotero references
8. Continue until the pathway ends, tracking every transition taken by the signal
9. Make at least one branching decision

---

# 8. Required Deliverables

Each student must submit:

- One evolving Signal Record that tracks every transition taken by the signal
- Completed EDOCA analysis at each step
- Required links and research evidence at each step (node, agent, course material, authoritative source, Zotero)
- Final evaluation answering:

> How much can D trust S based on V?

---

# 9. System Behavior

This system is:

- asynchronous
- student-driven
- cumulative
- evolving

Students do not modify core Node definitions. Students contribute observations to Node pages.

Because signals may traverse different nodes in different ways, pathway linkage must remain on each signal record (not on node or agent reference pages). Page naming and transition linkage are part of the assignment requirements, not optional formatting details.

---

# 10. Pilot Content Definition (Loan System)

The signal is the **loan application data** representing an applicant.

The system transforms this signal through:

- data structuring
- algorithmic scoring
- human interpretation
- institutional decision-making

The purpose of the signal is:

> to preserve sufficient structural information about the applicant to support a fair and accurate lending decision.

This loan pathway is the first pilot content set for the activity. It is not the only possible content model for the game system.

---

# 11. Key Design Principles

- Nodes are Spaces
- Agents operate within Spaces
- Signals carry state
- Transformations are mappings
- Integrity is pattern preservation
- Mediation occurs across both space and time
- Storage and retrieval are active mediation, not passive background
- Trust is probabilistic
- The system evolves through use
- System design and scenario content should be documented separately when the activity expands beyond the first pilot

---

# 12. Implementation Notes (VSC + GitHub Wiki)

- Use Markdown for all pages
- Use self-documenting flat page names rather than folder-dependent navigation
- Enforce naming conventions for Signal Records
- Require backward links (provenance chain)
- Require forward links when known
- Use internal Wiki links for navigation
- Link to the exercise from Home and, when useful, distribute the direct exercise URL
- Store the Signal Record template in the assignment materials or linked repository resources
- Require authoritative source links and Zotero references in transition entries

Do NOT automate in this version.

---

# End of Document

