# SEID 2364 Case Study Documentation Standard
## Structural Requirements for All Case Study Documents

This document specifies the required structure, sections, and metadata for all case studies used in SEID 2364. All case study documents (both standardized and lite versions) must follow this standard for consistency, usability, and pedagogical effectiveness.

---

## UNIVERSAL METADATA (All Cases)

Every case study document must begin with a metadata block before the title:

```
---
title: [Case Study Title]
domain: [Primary domain/field]
primary_stakeholders: [List 3-5 key stakeholder categories]
frameworks_addressed: [Which frameworks apply: ACM, IEEE, BBS, EDOCA, EU AI Act, etc.]
version: [standardized or lite]
last_updated: [date]
pedagogical_depth: [lite/teaching/advanced]
suitable_for_weeks: [Week numbers]
assignment_connections: [Which assignments can use this case]
---
```

**Example**:
```
---
title: COVID-19 Misinformation Moderation
domain: Information systems, platform governance, public health
primary_stakeholders: Platform operators, health institutions, content moderators, disinformation actors, communities
frameworks_addressed: ACM, IEEE, BBS mediation pathways, EDOCA, EU governance
version: standardized
last_updated: May 2026
pedagogical_depth: teaching
suitable_for_weeks: Week 11
assignment_connections: Assignment 11 (ACM/IEEE), Assignment 10 (synthesis)
---
```

---

## STRUCTURE FOR STANDARDIZED CASE STUDIES

Standardized cases are fully scaffolded for classroom teaching and discussion. They provide rich context to support analytical work.

### Required Sections (In Order)

#### 1. CASE TITLE & SUBTITLE
**Format**: 
```
# Case Study: [Title]
## [Subtitle or thematic focus]
```

**Purpose**: Introduce domain and central ethical tension in one phrase

**Example**:
```
# Case Study: COVID-19 Misinformation Moderation
## Platform Governance, Information Crisis, and Professional Responsibility
```

**Guidance**:
- Title should be specific (not "AI Ethics Case")
- Subtitle should name the ethical tension or domain focus

---

#### 2. CASE AT A GLANCE
**Format**: Bullet-point summary of core case elements

```
## Case At a Glance
- **Domain:** [Primary field/industry]
- **Primary system/intervention:** [What is being analyzed]
- **Primary stakeholders:** [3-5 key stakeholder categories]
- **Core ethical tension:** [One-sentence articulation of central conflict]
- **Suggested use:** [How this case fits into course]
```

**Length**: 100–150 words total

**Guidance**:
- Make this scannable; students often read this first to decide if case is relevant
- Ethical tension must be stated as a genuine conflict (not a settled question)
- Suggest use should connect to course concepts (BBS, frameworks, etc.)

**Example**:
```
## Case At a Glance
- **Domain:** Generative AI, cultural heritage, creative systems governance
- **Primary system/intervention:** Meta-Mozart model training on Mozart compositions (public domain), AI-generated outputs, and living composer contributions
- **Primary stakeholders:** Living composers, model developers, rights holders, audiences, cultural institutions, regulators
- **Core ethical tension:** Open cultural inheritance and creative innovation versus attribution ambiguity, consent obligations, and possible re-privatization of shared heritage
- **Suggested use:** Comparative analysis of authorship, consent, transparency, and governance in human-AI co-creation
```

---

#### 3. NARRATIVE INTRODUCTION (Situating the Case)
**Format**: 2–4 paragraphs of narrative framing

**Purpose**: Establish context, key actors, and tension before diving into analysis

**Length**: 250–400 words

**Required elements**:
- Opening: What is happening and why it matters
- Key actors: Who is involved and their roles
- Scope: What is being designed, deployed, or governed
- Tension: What makes this ethically significant (foreshadow complexity)

**Guidance**:
- Write in third-person, narrative style (not list-based)
- Avoid jargon; use accessible language for Week 1–2 students
- Paint the picture: help students *see* the system, not just understand it abstractly
- End with: "Here's why this matters ethically and how it became complicated"

**Example Opening**:
```
Quantum Musico frames musical creation as a mediated process among historical, human, and computational intelligences. In this case, the Meta-Mozart model is trained using three layers of input: public-domain Mozart compositions, AI-generated Mozart-like improvisations, and works from living composer-performers. This layered design produces a recursive generative system in which outputs can later re-enter training, blurring boundaries between source material, derivative signals, and newly generated style.

The case is attractive pedagogically because it is not reducible to a simple legal answer...
```

---

#### 4. MEDIATION PATHWAY(S) OR SYSTEM ARCHITECTURE
**Format**: Text description + visual/diagram if available

**Purpose**: Show how information, authority, and responsibility flow through the system

**Length**: 200–300 words + 1 visual if possible

**Guidance**:
- If visual pathway exists (image, diagram), embed it with caption
- Describe the pathway in language accessible to students unfamiliar with BBS
- Identify key transitions: where does distortion happen? Where does responsibility shift?
- Name actors/nodes explicitly

**Required for BBS-heavy cases** (Quantum Musico, COVID, Social Media)

**Optional for other cases** (may be replaced by detailed system description)

**Example**:
```
## BBS Mediation Pathway Snapshot

This case should remain interpretable without requiring students to open additional materials first. The pathway below gives a shared baseline for discussion while still leaving full pathway construction as a student output activity.

Condensed pathway: Mozart (historical source) → corpus and editorial tradition (vectors) → Quantum Musico/Meta-Mozart model (computational mediator) → living composers and listeners (destinations and secondary sources).

![Quantum Musico BBS mediation pathway](../images/Quantum_Music_Research_Flow.png)

The image can be used as a starting frame; students can then expand, challenge, or redraw the pathway to reflect different assumptions about authorship, control, and responsibility.
```

---

#### 5. GOVERNANCE CONTEXT & INSTITUTIONAL LANDSCAPE
**Format**: Descriptive paragraphs or structured summary

**Purpose**: Explain the regulatory, institutional, and professional context

**Length**: 200–300 words

**Required elements**:
- What governing bodies or institutions are relevant?
- What regulatory frameworks apply (or don't)?
- What professional or ethical codes are in play?
- What authority is distributed where?

**Guidance**:
- This section makes governance analysis concrete (not abstract)
- Reference specific regulations or codes if they apply
- Explain gaps: what *isn't* governed and why that matters
- Foreshadow: why governance frameworks might conflict or be incomplete

**Example**:
```
## Governance and Context Notes

This case is best treated as a governance design problem spanning intellectual history, technical architecture, and institutional accountability. The main governance question is how to sustain openness and traceability while supporting creative experimentation.

Key governance dimensions include consent, attribution, transparency, reversibility, and public access. Because data sources cross legal and cultural categories, ethically robust governance should exceed minimum legal compliance and include procedural protections for contributors and audiences.
```

---

#### 6. STAKEHOLDER TAXONOMY
**Format**: Grouped stakeholder categories with descriptions

**Purpose**: Map who is involved, affected, and responsible

**Length**: 200–250 words (4–6 stakeholder groups)

**Required structure**:
- Organize by relationship to system or by proximity to harm
- Use consistent categories across all cases (direct, economic, governance, design/accountability)
- For each group: 1–2 sentences explaining role and stakes

**Guidance**:
- Go beyond obvious actors (include overlooked/distant stakeholders)
- Show divergent interests: not all actors want the same outcome
- Name specific roles (e.g., "content moderators" not just "platform employees")
- Use parallel structure across all cases

**Example**:
```
## Stakeholders

Stakeholders can be grouped by how they contribute to or are affected by cultural and technical mediation.

- **Direct contributors and affected creators:** living composer-performers, music producers, and collaborative artists whose work and identity may be represented or transformed by the model.
- **System operators and economic actors:** model developers, platform operators, investors, and organizations distributing generated outputs.
- **Cultural and public-interest actors:** audiences, educators, archivists, cultural institutions, and communities concerned with heritage integrity and access.
- **Governance and oversight actors:** regulators, rights organizations, legal institutions, and independent auditors.
```

---

#### 7. RISK AND HARM MAP (Bidirectional)
**Format**: Structured into three subsections (Implementation, Non-Implementation, Bidirectional Tradeoffs)

**Purpose**: Show that harm can arise from action *and* inaction; identify unavoidable tradeoffs

**Length**: 300–400 words total

**Required structure**:

**7a. Implementation Risks** (if system/intervention proceeds)
- Bullet-point list of potential harms
- Brief explanation of each (1–2 sentences)
- Focus on: what could go wrong if we do this?

**7b. Non-Implementation Risks** (if system/intervention is constrained or abandoned)
- Bullet-point list of potential harms from inaction
- Brief explanation of each
- Focus on: what could go wrong if we don't do this?

**7c. Bidirectional Tradeoff Risks** (unavoidable tensions)
- Harms that persist regardless of choice
- Must be managed through governance design
- Shows the case is not reducible to "yes or no"

**Guidance**:
- Make risks **concrete and specific** (not vague)
- Use consistent language across all cases
- Show that **every choice has costs**
- Foreshadow: which frameworks will prioritize which risks?

**Example**:
```
## Risk and Harm Map

Risk in this case is also bidirectional. Harm can arise from aggressive model expansion without safeguards, or from overly restrictive governance that blocks legitimate innovation and access.

### Implementation Risks (if recursive Meta-Mozart development proceeds quickly)

If growth is prioritized over controls, creative capacity may expand while transparency and fairness decline.

- **Attribution harm:** unclear lineage can obscure who contributed what.
- **Consent harm:** living contributors may lack meaningful control over downstream use.
- **Cultural stewardship harm:** heritage may be reframed in ways that distort context or imply false authenticity.

### Non-Implementation Risks (if system development is heavily constrained or abandoned)

If experimentation is halted entirely, important educational, artistic, and methodological opportunities may be lost.

- **Innovation loss risk:** reduced exploration of ethically guided human-AI co-creation.
- **Research stagnation risk:** fewer opportunities to test governance mechanisms...

### Bidirectional Tradeoff Risks

Some harms persist across both permissive and restrictive approaches...

- **Openness-control tradeoff:** open access can enable creativity and misuse simultaneously.
```

---

#### 8. DISCUSSION QUESTIONS (Tiered)
**Format**: Numbered list, organized by analytical layer (optional)

**Purpose**: Guide student analysis and classroom discussion

**Length**: 8–12 questions

**Required types** (represent multiple frameworks and analytical levels):

- **Conceptual questions** (what is this case about?)
- **Stakeholder questions** (who is affected and how?)
- **Framework questions** (how do different ethical approaches evaluate this?)
- **Governance questions** (what should be done and by whom?)
- **Tradeoff questions** (what are we choosing between?)
- **Professional responsibility questions** (what do professionals owe?)

**Guidance**:
- Move from understanding → analysis → synthesis
- Avoid yes/no questions; ask "how" and "why"
- Connect to course concepts (BBS, EDOCA, frameworks)
- Make questions answerable from the case (not requiring outside research)
- Frame some questions as genuine dilemmas (not settled)

**Example**:
```
## Discussion Questions

These questions are intended to move students beyond abstract authorship debates toward concrete governance decisions.

1. What obligations arise when public-domain cultural material is transformed by large-scale generative systems?
2. How should living contributors' consent and withdrawal rights be implemented technically and contractually?
3. At what point does iterative style transfer become ethically misleading representation?
4. What documentation standard is sufficient for provenance in recursive model pipelines?
5. Should models built on public-domain heritage be required to preserve some level of public access?
6. How should benefits and recognition be distributed among historical source communities, living contributors, and developers?
```

---

#### 9. ANALYTICAL LENSES / FRAMEWORKS TO APPLY
**Format**: Bullet list with brief descriptions

**Purpose**: Signal which frameworks are most relevant; suggest comparison points

**Length**: 200–250 words (4–6 frameworks)

**Required elements**:
- Name of framework or analytical approach
- Brief description (1–2 sentences) of what it emphasizes
- Why it's useful for *this* case

**Guidance**:
- Include at least 2–3 professional codes (ACM, IEEE, etc.) when applicable
- Include structural frameworks (BBS, EDOCA)
- Include ethical traditions (consequentialism, deontology, virtue ethics) if relevant
- Suggest comparison: which frameworks see different harms as primary?

**Example**:
```
## Suggested Analytical Lenses

No single framework resolves this case fully. Students should compare creative-ethics, governance, and professional responsibility frameworks to identify where tradeoffs are unavoidable.

- **ACM Code of Ethics** — emphasizes transparency, avoidance of deception, respect for privacy and autonomy
- **IEEE Code of Ethics** — emphasizes professional integrity, public welfare, and acknowledgment of limitations
- **BBS mediation pathway analysis** — maps how cultural, computational, and social intelligences interact
- **EDOCA diagnostic dimensions** — evaluates effort, distortion, observability, control, authority at each transition
- **Cultural stewardship ethics** — examines obligations to heritage communities and living contributors
```

---

#### 10. SOURCES & REFERENCES
**Format**: Markdown list or bibliography

**Purpose**: Provide citations and suggest additional reading

**Length**: Flexible (depends on case)

**Required**:
- Sources *used to construct the case* (must be cited)
- Sources for factual claims in the case narrative
- Optional: recommended reading for instructors/advanced students

**Guidance**:
- Always note if case is constructed from academic research, news reports, or fictional scenario
- For real incidents: use primary sources when possible
- For hypothetical cases: note that
- Include institutional/regulatory documents if referenced (EU AI Act, ACM Code, etc.)

**Example**:
```
## Sources

No external references were provided in the original source case file.

Original source used for this standardized version:
- ../quantum_musico.md

---
```

---

## STRUCTURE FOR LITE CASE STUDIES

Lite cases are minimally scaffolded student-facing materials for final projects. They provide the core scenario but require students to do the analysis work.

### Required Sections (In Order)

#### 1. METADATA (Same as standardized)

```
---
title: [Case Study Title]
domain: [Primary domain/field]
primary_stakeholders: [List 3-5]
frameworks_addressed: [Which frameworks apply]
version: lite
last_updated: [date]
pedagogical_depth: lite (final project)
suitable_for_weeks: Week 11–14 (final projects)
assignment_connections: [Which final project assignments use this]
---
```

---

#### 2. CASE TITLE & SUBTITLE
**Format**: Same as standardized

---

#### 3. BRIEF SCENARIO (Not full narrative)
**Format**: 1–2 paragraphs, fact-focused

**Purpose**: Establish context quickly without scaffolding analysis

**Length**: 100–150 words

**Guidance**:
- State facts: what is the system, who operates it, who is affected
- Avoid: governance notes, ethical interpretation, discussion framing
- Provide enough context for students to ask their own questions

**Example** (lite version):
```
## Scenario

Quantum Musico is an AI music generation system trained on three types of input: public-domain Mozart compositions, AI-generated Mozart-like variations, and works submitted by contemporary composers and musicians. The system generates new musical compositions that blend historical, computational, and human creative elements.

The company plans to release both the model weights and a user-facing generation interface. Questions have emerged about attribution, consent from living contributors, and whether the public-domain heritage used for training should result in public-domain outputs.
```

---

#### 4. CORE QUESTIONS FOR ANALYSIS
**Format**: 4–6 guiding questions (NOT answered by case)

**Purpose**: Direct student analysis without providing scaffolding

**Length**: 200–250 words

**Required elements**:
- Questions about stakeholders (who is involved?)
- Questions about mediation pathways (how does information flow?)
- Questions about governance (what framework applies?)
- Questions about tradeoffs (what conflicts exist?)

**Guidance**:
- These are genuine open questions (case does not answer them)
- Grounded in the case (answerable from scenario + research)
- Require students to construct stakeholder maps, pathways, harm analysis

**Example**:
```
## Core Questions for Your Analysis

1. Who are all the stakeholders affected by Quantum Musico, and how are their interests aligned or in conflict?
2. How does the training data (historical + AI + contemporary) move through the system, and where does information get lost or distorted?
3. What governance frameworks (professional codes, regulatory, consent) should apply to this system, and where do they conflict?
4. What are the harms that result from aggressively releasing the model? From heavily constraining it? From restricting access?
5. What would ethical governance of Quantum Musico look like in practice?
```

---

#### 5. REQUIRED STUDENT ANALYSIS OUTPUTS
**Format**: Clear specification of what students must produce

**Purpose**: Define minimum depth requirements (prevents oversimplification)

**Length**: 150–200 words

**Required**: Students must include analysis of:
- **Stakeholder map** — who is involved and how
- **Mediation pathway(s)** — how does information/authority flow?
- **Risk and harm analysis** — bidirectional (if/if not) analysis
- **Framework analysis** — how do different frameworks evaluate this?
- **Governance recommendation** — what should be done and by whom?

**Guidance**:
- Be explicit: students *cannot* submit summaries or descriptions
- Require *construction* (students build pathways, identify risks, compare frameworks)
- Tie to course tools (BBS, EDOCA, professional codes)

**Example**:
```
## Required Student Analysis

Your analysis must include:

1. **Stakeholder taxonomy** — map at least 4 stakeholder categories and explain their stakes
2. **Mediation pathway(s)** — trace how training data and model outputs move through the system; identify at least 2 distinct pathways
3. **Bidirectional risk analysis** — what harms arise from aggressive deployment vs. restrictive governance? What tradeoffs are unavoidable?
4. **Framework comparison** — compare at least 2 ethical frameworks (ACM, IEEE, BBS/EDOCA, consequentialist, deontological, virtue ethics); show how they prioritize different stakeholders/risks
5. **Governance position** — articulate a defensible governance approach that addresses the case's core tensions; explain trade-offs you're accepting
```

---

#### 6. SOURCES & RESOURCES FOR FURTHER RESEARCH
**Format**: Markdown list

**Purpose**: Point students toward evidence and context

**Length**: Flexible (5–10 sources)

**Required**:
- At least 1–2 academic or policy sources on the domain
- At least 1–2 news/incident reports (if case is based on real events)
- At least 1 professional code or governance document

**Guidance**:
- Lite cases should not require extensive research, but students should verify facts
- Point to reputable sources (academic, news, government, professional organizations)
- Avoid overwhelming; 5–10 sources is sufficient

---

## QUICK REFERENCE: STANDARDIZED vs. LITE STRUCTURE

| **Section** | **Standardized** | **Lite** | **Purpose** |
|---|---|---|---|
| Metadata | ✅ Required | ✅ Required | Track context and pedagogical use |
| Title & Subtitle | ✅ Required | ✅ Required | Orient reader |
| Case at a Glance | ✅ Required | ❌ Omitted | Standardized only; lite avoids summary |
| Narrative Intro | ✅ Required (400w) | ❌ Replaced with brief scenario (150w) | Standardized scaffolds; lite requires student synthesis |
| Mediation Pathway | ✅ Required | ❌ Omitted | Standardized scaffolds; lite requires student construction |
| Governance Context | ✅ Required | ❌ Omitted | Standardized scaffolds; lite requires student research |
| Stakeholder Taxonomy | ✅ Required (with roles explained) | ❌ Omitted | Standardized scaffolds; lite requires student mapping |
| Risk/Harm Map | ✅ Required (detailed) | ❌ Omitted | Standardized scaffolds; lite requires student analysis |
| Discussion Questions | ✅ 8–12 questions (tiered) | ❌ Replaced with "Core Questions for Analysis" | Standardized for discussion; lite prompts independent analysis |
| Analytical Lenses | ✅ Required (with context) | ❌ Omitted | Standardized scaffolds; lite requires student selection |
| Sources | ✅ Complete citations | ✅ Research starting points | Both provide reference materials |

---

## COMPLIANCE CHECKLIST

**Before finalizing any case study, verify**:

### Standardized Cases
- [ ] Metadata block is present and complete
- [ ] Title and subtitle clearly name domain and central tension
- [ ] Case at a Glance is scannable and specific
- [ ] Narrative intro is 250–400 words and accessible to new students
- [ ] Mediation pathway (or system architecture) is described and visualized if possible
- [ ] Governance context explains regulatory/institutional landscape
- [ ] Stakeholder taxonomy has 4–6 groups with clear descriptions
- [ ] Risk/harm map includes implementation, non-implementation, and bidirectional tradeoffs
- [ ] Discussion questions are 8–12 and tiered (understanding → synthesis)
- [ ] Analytical lenses include at least 2–3 professional codes and structural frameworks
- [ ] Sources are cited for all factual claims
- [ ] Case length is 2000–3000 words (fits one class session + homework)

### Lite Cases
- [ ] Metadata block is present and complete
- [ ] Title and subtitle are clear
- [ ] Scenario brief is 100–150 words and fact-focused
- [ ] Core questions for analysis are 4–6 and genuinely open
- [ ] Required student outputs are specific and tied to course tools
- [ ] Research sources are provided (5–10)
- [ ] Case can be analyzed in 3–5 hours (reasonable final project scope)
- [ ] No scaffolding is provided; students do the analysis work

---

## APPLYING THIS STANDARD

### Creating a New Standardized Case
1. Identify domain and central ethical tension
2. Draft metadata block
3. Follow the 10 required sections in order
4. Ensure narrative is accessible to Week 1–2 students
5. Make stakeholder taxonomy consistent with other cases
6. Use bidirectional risk framework (implementation + non-implementation + tradeoff)
7. Tie discussion questions to course frameworks (BBS, EDOCA, professional codes)
8. Draft both standardized AND lite versions
9. Verify against compliance checklist

### Converting an Existing Case to Standardized Format
1. Review original case for core content and sources
2. Create metadata block reflecting pedagogical use
3. Reorganize content into 10-section structure
4. Expand narrative intro if needed (should be 250–400 words)
5. Extract/create stakeholder taxonomy (4–6 groups)
6. Build bidirectional risk map (implementation + non-implementation + tradeoff)
7. Generate discussion questions (8–12, tiered)
8. Add analytical lenses (tie to frameworks)
9. Verify sources are cited
10. Create lite version (remove scaffolding)

---

## MAINTENANCE & VERSIONING

- **Version field in metadata** — tracks when case was last updated
- **Pedagogical depth field** — allows quick filtering (lite vs. teaching vs. advanced)
- **Suitable for weeks** — helps instructors find cases for their units
- **Assignment connections** — clarifies which assignments use this case
- **Review cycle** — cases should be reviewed annually for accuracy and currency

---

Last updated: May 16, 2026
