# SEID 2364 Case Studies Inventory
## Development Status, Usage, and Pedagogical Role

This document inventories all case studies, scenarios, and case-based materials used in SEID 2364. For each case, it describes:
- **Pedagogical role** — which weeks/assignments use this material
- **Development stage** — full case vs template vs scenario
- **Current versions** — what formats exist (original, standardized, lite, etc.)
- **Key content** — what makes this case distinctive
- **Typical depth** — how much complexity/scaffolding students encounter

---

## MASTER FLAT LIST: ALL CASE STUDY IDEAS AND CLASSROOM USE

This is the single list of case-study ideas across the course, regardless of development level.

Ordering rule for Master UID assignment: cases are ordered by first introduced week; ties are ordered alphabetically by case title.

| **Master UID** | **Case Idea** | **First Introduced Week** | **Current Material Type** | **Development Level** | **Used in Class/Assignment?** | **Week(s) Used** | **How Used (or Not Used)** | **Primary Source** |
|---|---|---|---|---|---|---|---|---|
| CS-001 | Moral Machine (Autonomous Vehicle Ethics) | 1 | Foundational dataset + activity | Fully developed | **Yes** | 1 | Assignment 1 opening ethics exercise and journal grounding | `resources/datasets/doi_10_5061_dryad_d7wm37q6v__v20230921/` and `../assignments/SEID2364_Assignment01_moral_machine_ethics_journal.md` |
| CS-002 | Emergency Room Triage | 3 | Scenario (multi-risk) | Basic | **Yes** | 3-4 | Early harm-analysis example (Assignments 3-4 support) | `case-studies/multi_risk_scenarios.md` and `case-studies/seid2364_part1_example_scenarios.md` |
| CS-003 | Eminent Domain for Infrastructure | 3 | Scenario (multi-risk) | Basic | **Yes** | 3-4 | Early harm-analysis example (Assignments 3-4 support) | `case-studies/multi_risk_scenarios.md` and `case-studies/seid2364_part1_example_scenarios.md` |
| CS-004 | Grading Curves in Competitive Programs | 3 | Scenario (multi-risk) | Basic | **Yes** | 3-4 | Early harm-analysis example (Assignments 3-4 support) | `case-studies/multi_risk_scenarios.md` and `case-studies/seid2364_part1_example_scenarios.md` |
| CS-005 | Mandatory Vaccination Policy | 3 | Scenario (multi-risk) | Basic | **Yes** | 3-4 | Early harm-analysis example (Assignments 3-4 support) | `case-studies/multi_risk_scenarios.md` and `case-studies/seid2364_part1_example_scenarios.md` |
| CS-006 | AI Academic Writing Assistant | 8 | System template | Template | **Yes** | 8 | Assignment 8 selectable system option | `resources/08-SEID2364_usecase_system_set.md` |
| CS-007 | AI Hiring Assistant | 8 | System template | Template | **Yes** | 8 | Assignment 8 selectable system option | `resources/08-SEID2364_usecase_system_set.md` |
| CS-008 | AI Loan / Credit Advisor | 8 | System template | Template | **Yes** | 8 and 10 | Assignment 8 selectable system option; also overlaps with loan pathway activity usage | `resources/08-SEID2364_usecase_system_set.md` |
| CS-009 | AI Medical Triage Chatbot | 8 | System template | Template | **Yes** | 8 | Assignment 8 selectable system option | `resources/08-SEID2364_usecase_system_set.md` |
| CS-010 | Loan Signal-Tracking Scenario | 10 | Interactive scenario | Active development (pilot) | **Yes** | 10 | Pathway/trust activity in wiki format | `resources/week-10/10-01-signal_tracking_game_master_source.md` |
| CS-011 | COVID-19 Misinformation Moderation | 11 | Full case | Fully developed | **Yes** | 11 | Week 11 lesson + Assignment 11 primary case; used for ACM/IEEE analysis and governance comparison | `case-studies/case_study-covid_misinformation.md` |
| CS-012 | OptiRate Workplace Analytics | unknown | Full case | Fully developed | **Partially / limited explicit assignment use** | - | Present in case library and used for case-standardization workflow; not currently the explicit required case in a named assignment | `case-studies/optirate_ethics_case_study_acm_ieee.md` |
| CS-013 | Quantum Musico / Meta-Mozart | unknown | Full case | Fully developed | **Partially / thematic use** | - | Used as emerging-tech and authorship/heritage ethics case material; not currently the explicit required case in a named assignment | `case-studies/quantum_musico.md` |
| CS-014 | Social Media Ethics | unknown | Full case | Fully developed | **Partially / thematic use** | - | Used as platform-governance case material; not currently the explicit required case in a named assignment | `case-studies/social_media_ethics.md` |

### Notes on Duplicate/Parallel Framing Files
- `case-studies/seid2364_part1_example_scenarios.md` repeats the same four early scenarios in a shorter format for assignment framing.
- It is best treated as an instructional framing companion, not as four additional unique case ideas.

---

## CASE ID AND METADATA FIELD DEFINITIONS

This section defines the fields to use when implementing and maintaining the case ID system.

### ID Structure

- **Master Case UID**
	- Purpose: stable identifier for the underlying case idea, independent of format.
	- Format (display): `CS-001`
	- Rule: never changes once assigned.

- **Variant UID**
	- Purpose: identifier for a specific artifact/version of a master case.
	- Format (display): `CS-001-F`, `CS-001-L`, `CS-001-S`, `CS-001-T`, `CS-001-A`
	- Variant codes:
		- `F` = full/standardized case
		- `L` = lite case
		- `S` = scenario version
		- `T` = template version
		- `A` = activity/dataset framing

- **Canonical (optional compact) ID**
	- Purpose: machine-compact form if needed in scripts.
	- Format: `CS001F`
	- Rule: if used, it must be a direct transform of the display Variant UID.

### Core Tracking Fields

- **case_title**
	- Human-readable case name used in teaching materials.

- **case_type**
	- One of: `full`, `lite`, `scenario`, `template`, `activity`.

- **development_level**
	- Current maturity state (for example: `basic`, `template`, `active development`, `fully developed`).

- **used_in_class**
	- Allowed values: `yes`, `partial`, `no`.
	- Meaning:
		- `yes` = explicitly used in a class session and/or named assignment.
		- `partial` = referenced thematically or available in library, but not clearly required in a named assignment.
		- `no` = planned/available but not yet used.

- **weeks_used**
	- Week number(s) where used (for example: `1`, `3-4`, `8 and 10`, `11`).
	- Use `-` when no explicit week is currently documented.

- **first_introduced_week**
	- First known week the case was introduced to students.
	- Use `unknown` if evidence is incomplete.

- **first_assigned_in**
	- First named assignment/activity where required (for example: `Assignment 11`).
	- Use `none documented` if not explicitly assigned.

- **registry_order**
	- Chronological order in which the case was entered into the inventory/registry.
	- Purpose: operational tracking only; does not define teaching sequence.

- **pedagogical_order**
	- Intended instructional sequence order.
	- Purpose: curriculum planning and flow.

- **primary_source_paths**
	- Canonical file(s) that define the case.
	- If duplicate framings exist, include all relevant paths in one row.

- **notes_on_use**
	- Short, concrete description of how the case was used (or why not used yet).

### Governance Rules

1. UIDs are permanent and never renumbered.
2. New master cases always get the next available `CS-###`.
3. Pedagogical timing is tracked in fields, not encoded in UID numbers.
4. If historical week data is uncertain, mark as `unknown` rather than guessing.
5. Duplicate case framings should share one Master Case UID and list multiple source references.

---

## TIER 0: FOUNDATIONAL DATASETS & OPENING ACTIVITIES

These are the entry point materials that establish ethical reasoning habits before case-based analysis begins.

### Foundational Material 1: Moral Machine Dataset & Analysis
**Primary Files**: 
- Assignment: `../assignments/SEID2364_Assignment01_moral_machine_ethics_journal.md`
- Dataset: `resources/datasets/doi_10_5061_dryad_d7wm37q6v__v20230921/`
- Source: [https://doi.org/10.5061/dryad.d7wm37q6v](https://doi.org/10.5061/dryad.d7wm37q6v)

**Pedagogical Usage**:
- **Assignment 1 (Week 1)** — Opening ethical reasoning activity
- **In-class activity** — Students engage with interactive Moral Machine scenarios before studying dataset
- **Foundational journal entry** — Students record their initial ethical framing and refine it

**Development Status**: ✅ **Fully Developed**

**Dataset Content**:
- **Version**: v20230921 (LLM study: ChatGPT, PaLM 2, Llama 2 responses to autonomous vehicle scenarios)
- **Source**: Recent academic study testing large language models on trolley-problem variants
- **Includes**: Python scripts for scenario generation, R code for analysis/visualization, processed results

**Pedagogical Function**:
- **Immediate engagement** with real ethical decision data (not hypothetical)
- **Distinction-building**: Separates descriptive patterns (what people/models chose) from normative claims (what is right)
- **Critical perspective**: Examines ethics of using crowd/model data to inform policy
- **Journal grounding**: Anchors personal ethical framework development in observed data

**Core Assignment Structure**:
- **Part A**: Dataset analysis addressing what data represents, notable patterns, interpretive caution, and ethics of use
- **Part B**: Journal Entry 1 recording exact first-class prompts, responding to three core framing questions ("What is ethics," "How do you decide ethical actions," "How do you decide right/wrong"), and refining ethical framing questions

**Extent of Development**:
- Full assignment (900–1200 words analysis + journal entry)
- Real dataset with code/methodology transparency
- Integrated with Week 1 lesson on foundational ethical vocabulary
- Required scaffolding: journal entry forces explicit articulation before framework learning

**Connection to Autonomous Vehicle Ethics**:
This dataset anchors all subsequent autonomous vehicle ethics analysis. Students see actual behavioral/model responses to vehicle allocation dilemmas before studying governance, professional codes, or stakeholder analysis.

---

## TIER 1: FULL CASE STUDIES (Fully Developed, Multi-Context)

These cases are complete, richly contextualized, and used across multiple assignments or weeks.

### Case Study 1: COVID-19 Misinformation Moderation
**Primary File**: `case_study-covid_misinformation.md`

**Pedagogical Usage**:
- **Assignment 11 (Week 11)** — Primary case for professional codes analysis (ACM/IEEE)
- **Lesson Plan** — Week 11 lesson on "bad actors, professional codes, framework disagreement"
- **Introduction** — Short case card used in opening in-class provocation (reveals staged through lecture)
- **Governance contexts** — Comparative analysis across U.S., EU, China regulatory frameworks

**Development Status**: ✅ **Fully Developed**

**Available Versions**:
- Original: `case_study-covid_misinformation.md` (full case with governance contexts)
- Teacher reference: `case_study-covid_misinformation_teacher.md`
- Standardized: `standardized_case_studies/case_study-covid_misinformation-standardized.md`
- Lite (student final project): `lite_case_studies/case_study-covid_misinformation-lite.md`

**Core Content**:
- **Domain**: Information ecosystems, platform governance, public health crisis response
- **Tension**: Balancing content moderation (harm reduction) vs. free expression and transparency
- **Stakeholders**: Platform operators, health institutions, content moderators, disinformation actors, affected communities, regulators
- **Frameworks**: ACM Code of Ethics, IEEE Code of Ethics, EU governance concepts, professional responsibility
- **Governance dimensions**: Authority, control, observability, accountability, proportionality

**Unique Features**:
- Explicitly frames "bad actors" concept (malicious vs. negligent vs. reckless vs. institutional behavior)
- Comparative governance (regulatory vs. professional vs. institutional approaches)
- Mediated information crisis as organizing framework
- Clear intervention strategies students can analyze independently

**Extent of Development**: 
- **Standardized version**: narrative intro, case at a glance, governance notes, stakeholder taxonomy, bidirectional risks (implementation/non-implementation/tradeoff), discussion questions, analytical lenses
- **Lite version**: minimal brief, core facts, evidence packet links, required student outputs, constraints

---

### Case Study 2: OptiRate (Algorithmic Hiring/Recommendation Ethics)
**Primary File**: `optirate_ethics_case_study_acm_ieee.md`

**Pedagogical Usage**:
- Early assignments (implied from ACM/IEEE framing)
- May appear in assignment options for system selection
- Now used as exemplar for standardized case structure

**Development Status**: ✅ **Fully Developed**

**Available Versions**:
- Original: `optirate_ethics_case_study_acm_ieee.md`
- Standardized: `standardized_case_studies/case_study-optirate-standardized.md`
- Lite (student final project): `lite_case_studies/case_study-optirate-lite.md`

**Core Content**:
- **Domain**: Algorithmic hiring, candidate evaluation, recommendation systems
- **Tension**: Efficiency and scale vs. fairness, transparency, and human judgment
- **Stakeholders**: Job applicants, hiring teams, organizational leadership, candidates who don't advance, job market communities
- **Frameworks**: ACM Code of Ethics, IEEE Code of Ethics, fairness in hiring, professional responsibility

**Unique Features**:
- Accessible to students (hiring is widely understood)
- Clear technical-to-ethical translation (algorithm output → hiring decision)
- Layered stakeholder taxonomy (direct, economic/institutional, governance/oversight actors)
- Discussion questions move from abstract to concrete governance decisions

**Extent of Development**:
- **Standardized version**: narrative framing, at-a-glance summary, case narrative with context, governance notes, layered stakeholder taxonomy, implementation/non-implementation/tradeoff risks, 12 discussion questions, analytical lenses (ACM, IEEE, BBS, EDOCA, fairness frameworks)
- **Lite version**: brief scenario, core facts, decision points, required student outputs

---

### Case Study 3: Quantum Musico (AI Creativity, Cultural Heritage, Authorship)
**Primary File**: `quantum_musico.md`

**Pedagogical Usage**:
- Emerging technologies and future capacity planning
- Authorship and attribution in human-AI co-creation
- Cultural stewardship and consent ethics
- Comparative analysis with other cases (similar depth to COVID)

**Development Status**: ✅ **Fully Developed**

**Available Versions**:
- Original: `quantum_musico.md`
- Standardized: `standardized_case_studies/case_study-quantum_musico-standardized.md` (includes embedded BBS pathway image)
- Lite (student final project): `lite_case_studies/case_study-quantum_musico-lite.md`

**Core Content**:
- **Domain**: Generative AI, cultural heritage systems, creative governance
- **Tension**: Open cultural inheritance and innovation vs. attribution, consent, and re-privatization of shared heritage
- **Stakeholders**: Living composers, model developers, rights holders, audiences, cultural institutions, regulators
- **Frameworks**: ACM Code of Ethics, IEEE Code of Ethics, BBS mediation pathways, EDOCA, cultural stewardship ethics

**Unique Features**:
- Multi-layered data sources (historical, AI-generated, contemporary human)
- Recursive training (outputs become inputs, provenance degrades)
- Governance spans intellectual history, technical architecture, institutional accountability
- BBS pathway visualization (Quantum Music Research Flow diagram embedded)
- Forces students beyond legal compliance to ethical governance design

**Extent of Development**:
- **Standardized version**: narrative intro, case at a glance, BBS mediation pathway snapshot with image, intervention strategies, governance notes, stakeholder taxonomy (direct, system operators, cultural/public, governance/oversight), bidirectional risks, 10 discussion questions, analytical lenses
- **Lite version**: scenario framing, core technical elements, governance questions, required analysis structure

---

### Case Study 4: Social Media Ethics (Platform Governance, Content Moderation, Virtual Localities)
**Primary File**: `social_media_ethics.md`

**Pedagogical Usage**:
- Platform ethics and algorithmic accountability
- Virtual vs. physical space mediation
- Context collapse and nested localities
- Comparative analysis with other governance cases

**Development Status**: ✅ **Fully Developed**

**Available Versions**:
- Original: `social_media_ethics.md`
- Standardized: `standardized_case_studies/case_study-social_media_ethics-standardized.md`
- Lite (student final project): `lite_case_studies/case_study-social_media_ethics-lite.md`

**Core Content**:
- **Domain**: Social media platforms, algorithmic content delivery, community governance
- **Tension**: User autonomy and community expression vs. platform safety and institutional control
- **Stakeholders**: Users, content creators, platform operators, advertisers, algorithm designers, affected communities, regulators
- **Frameworks**: ACM/IEEE codes, BBS virtual-locality framing, EDOCA, governance ethics

**Unique Features**:
- Nested locality hierarchy (personal circles → communities → platform → ecosystems)
- Ethical distance concept (proximity to harm affects responsibility)
- Context-collapse risks across different social contexts
- Cross-platform accountability distribution

**Extent of Development**:
- **Standardized version**: narrative intro, case at a glance, virtual-locality conceptual framing, case narrative with context, governance notes, stakeholder taxonomy, bidirectional risks, 10 discussion questions, analytical lenses
- **Lite version**: scenario framing, key platform features, nested locality hierarchy, required student outputs

---

## TIER 2: SCENARIO-BASED MATERIALS (Generic, Multi-Purpose)

These materials provide structured scenarios for learning specific concepts. They are not domain-specific cases but rather examples of harm types and ethical tensions.

### Scenario Set 1: Multi-Risk Scenarios (4 Scenarios)
**Primary File**: `multi_risk_scenarios.md`

**Pedagogical Usage**:
- **Assignments 3–4** — Harm identification and ethical framework analysis
- Examples students can use to understand "scope and level of description" expected
- Support material for ethical reasoning practice

**Development Status**: ⚠️ **Basic Level (Generic Examples)**

**Available Versions**:
- Single file with all four scenarios

**Core Scenarios**:
1. **Emergency Room Triage** — Resource scarcity, life-and-death allocation, multiple harm types
2. **Mandatory Vaccination Policy** — Individual autonomy vs. collective safety, perceived vs. statistical harm
3. **Eminent Domain for Infrastructure** — Economic displacement, community harm, distributed benefits
4. **Academic Grading Curves** — Psychological stress, competitive dynamics, structural inequity

**Pedagogical Function**:
- Introduce harm as **multidimensional** (physical, psychological, moral, systemic)
- Show how harms are **unevenly distributed** (immediate vs. diffuse, concentrated vs. dispersed)
- Support early ethical reasoning without domain-specific complexity
- Provide options for students who need to select an assignment case

**Extent of Development**: 
- Each scenario: 150–200 words
- Description of situation, types of harm present, discussion prompts
- Not full cases; intended as starting points

---

### Scenario Set 2: Part 1 Example Scenarios (same 4 scenarios, different framing)
**Primary File**: `seid2364_part1_example_scenarios.md`

**Pedagogical Usage**:
- **Assignment 3–4 Part 1** — Illustrating "scope and level of description"
- Students may select one example or define their own
- Used to calibrate expectation for system complexity in early assignments

**Development Status**: ⚠️ **Basic Level (Instructional Support)**

**Available Versions**:
- Single file with all four scenarios

**Core Content**:
- Same four scenarios as multi-risk set
- Framed as **examples** students can choose from
- Emphasis on: does **not** evaluate, does **not** resolve, shows plausible real-world contexts

**Pedagogical Function**:
- Help students understand assignment scope (not too simple, not too ambitious)
- Provide safety net for students who lack a clear system idea
- Show what "different types of harm may arise or conflict" means in practice

**Extent of Development**: 
- ~50 words each scenario (briefer than multi-risk framing)
- No explicit harm taxonomy; focus on decision context

---

## TIER 3: SYSTEM TEMPLATES & INTERACTIVE SCENARIOS

These are not full cases but rather structural templates or interactive activities designed to teach system analysis.

### Template Set 1: Assignment 8 System Selection Set (4 Templates)
**Primary File**: `08-SEID2364_usecase_system_set.md` (in resources)

**Pedagogical Usage**:
- **Assignment 8** — System selection and bias analysis
- Students choose one, describe deployment context, analyze through EU AI Act lens
- Used as fresh analytical start (if student already analyzed a system in A4–A7, must pick different one)

**Development Status**: 🔧 **Template Level (Structural, Not Full Case)**

**Available Versions**:
- Single document with four templates

**Core Templates**:
1. **AI Hiring Assistant** — Resume analysis, ranking, recommendations
2. **AI Loan/Credit Advisor** — Creditworthiness evaluation, risk scoring
3. **AI Medical Triage Chatbot** — Symptom classification, care routing
4. **AI Academic Writing Assistant** — Text generation, editing, summarization

**Pedagogical Function**:
- Provide **structures** students can deploy in different contexts
- Force students to make decisions about **deployment, authority, and consequence**
- Support bias analysis by varying one element (user group, decision authority, institutional context)
- Teach how **context changes classification** (same system, different governance contexts)

**Extent of Development**: 
- Each template: ~250 words
- Describes typical capabilities, possible operations, data sources, key mediation features
- Students add: deployment, governance context, risk analysis

---

### Interactive Activity 1: Week 10 Signal Tracking Game (Loan/Lending Scenario)
**Primary Files**: 
- Master source: `10-01-signal_tracking_game_master_source.md` (resources/week-10)
- Implementation guide: `10-02-wiki_implementation_guide_signal_integrity_activity.md`
- Student template: `10-03-signal_card_template.md`
- Instructions: `10-04-signal_record_instructions.md`
- Worked example: `10-05-example_student_signal_cards.md`

**Pedagogical Usage**:
- **Week 10 Activity** — Temporal dynamics, signal transformation, trust in mediated systems
- Students track a loan application through a 5-node system
- Optional branch (appeal) allows for divergent pathways
- Wiki-based collaborative activity (students create/edit their own signal records)

**Development Status**: 🔧 **Active Development (Pilot Content)**

**Available Versions**:
- Modular: system layer (game mechanics), pilot content layer (loan scenario), node definitions, agent definitions
- Designed to be replicable with different scenarios

**Core System**:
- **Signal**: loan application data
- **Starting trust**: 70/100
- **Pathway**: Applicant Concept → Application Form → AI Scoring → Lending Officer → Decision (+ Optional Appeal)

**Pedagogical Function**:
- Practice **mediation pathway tracing** in a controlled interactive environment
- Learn how signals **transform** at each node
- Understand **temporal conditions** and trust degradation
- Apply EDOCA at each transition
- Connect course materials (BBS, frameworks, sources) to specific pathway moments

**Extent of Development**: 
- **System layer**: 5 stable page types, naming conventions, linking rules, student edit boundaries, required outputs
- **Pilot content**: 5+ fully defined nodes with signal transformation logic, agent definitions, vector descriptions
- **Student support**: template, instructions, worked example showing multi-transition signal record with branches

**Notes on Development**:
- Designed as replicable template (can be adapted for hiring, medical triage, writing assessment scenarios)
- Currently in pilot stage with loan scenario
- Intended to scale to other domain applications

---

## TIER 4: IN-CLASS ACTIVITIES & PROVOCATIONS

These are shorter materials used for immediate classroom learning and discussion.

### Activity 1: Week 6 Mediation Pathway Worksheets
**Primary Files**: `week-06/worksheet-instructions.md`, Worksheet A (Provocation PDF), Worksheet C (Student Sheet PDF)

**Pedagogical Usage**:
- **Week 6** — Support for Assignment 6 (mediation pathways)
- Reactivates Assignment 5 case selected by student
- Structured practice reconstructing one pathway
- One-pathway focus (not full BBS analysis)

**Development Status**: ✅ **Complete (Classroom-Ready)**

**Core Structure**:
- Worksheet A: Provocation to reactivate context
- Worksheet C: Structured pathway reconstruction template (duplicable for multiple pathways)

**Pedagogical Function**:
- Scaffolded transition from system description (A5) to pathway tracing (A6)
- Classroom-sized collaborative work (not individual homework)
- Preparatory for full mediation pathway assignment

**Extent of Development**: 
- Two worksheets per week (one provocation, one student working sheet)
- Archive includes development drafts and alternate versions

---

### Activity 2: Week 8 Bias Probe Exercise
**Primary File**: `08_in_class_activity_bias_probe_exercise.md` (in resources)

**Pedagogical Usage**:
- **Week 8** — Classroom activity before Assignment 8
- Uses student's own system from Assignment 7
- Controlled-variation methodology (change one element, observe result)
- Introduces EU AI Act classification bias

**Development Status**: ✅ **Complete (Classroom-Ready)**

**Core Structure**:
- Step 1: Baseline (submit system to AI, get classification)
- Step 2: Controlled Variation (change ONE element: user group, decision authority, institutional context, or consequences)
- Step 3: Comparison (what changed in AI's response?)
- Step 4: Bias Identification (where did bias enter?)

**Pedagogical Function**:
- Empirical demonstration of how **system framing affects ethical judgment**
- Bridge to Assignment 8 (system variation and risk classification)
- Practice using EU AI Act as analytical framework
- Show that ethical classification is not neutral (it depends on context, framing, and criteria)

**Extent of Development**: 
- 4-step structured process with example for each step
- Requires use of specific prompt template (ensures consistency, reveals classification sensitivity)
- Ready for classroom use

---

### Activity 3: Lesson Plan for Week 11 (COVID Misinformation Case with Professional Codes)
**Primary Files**: 
- Lesson plan: `resources/lecture notes/seid_2364_week_11_lesson_plan_bad_actors_professional_codes.md`
- Case card: `resources/week-11/week11_covid_misinformation_case_card.md`
- Conceptual source: `resources/week-11/SEID2364_misinformation_bad_actors_mediated_systems.md`

**Pedagogical Usage**:
- **Week 11 Lesson** — Applied ethical analysis, professional responsibility, framework disagreement
- Short case card used at lesson opening (staged reveal through provocations)
- Full COVID case study used after provocations for detailed framework analysis
- ACM, IEEE professional codes introduced during lesson (not pre-assigned)

**Development Status**: ✅ **Complete (Lesson-Ready)**

**Core Structure**:
- Opening: short case card + staged provocations (students respond with existing vocabulary)
- Middle: introduce infodemic, bad actors, professional codes concepts
- Post-class: expanded case study + ACM/IEEE detailed analysis

**Pedagogical Function**:
- Demonstrate how **professional codes operationalize ethical reasoning**
- Show that ethical frameworks make **different stakeholders and values visible**
- Practice **ethically ambiguous judgment** (good-faith actors, competing frameworks)
- Analyze **bad actors** (malicious vs. negligent vs. strategic vs. institutional)
- Examine distribution of **responsibility, control, observability, authority** (EDOCA)

**Extent of Development**: 
- Lesson plan: full instructional sequence with timing, materials, framing notes
- Case card: 1-page brief for immediate classroom use
- Conceptual source: 5K+ word foundational document on mediated systems, infodemic, information disorder, bad actors

---

## SUMMARY TABLE: ALL CASE MATERIALS BY DEVELOPMENT & USAGE

| **Title** | **Type** | **Stage** | **Weeks Used** | **Versions** | **Tier** |
|---|---|---|---|---|---|
| Moral Machine Dataset & Analysis | Foundational Dataset | ✅ Fully Developed | 1 | Original dataset (v20230921), Scripts, Results | 0 |
| COVID-19 Misinformation Moderation | Full Case | ✅ Fully Developed | 11, Lesson | Original, Teacher, Standardized, Lite | 1 |
| OptiRate | Full Case | ✅ Fully Developed | Early, Exemplar | Original, Standardized, Lite | 1 |
| Quantum Musico | Full Case | ✅ Fully Developed | Emerging Tech | Original, Standardized, Lite | 1 |
| Social Media Ethics | Full Case | ✅ Fully Developed | Platform Governance | Original, Standardized, Lite | 1 |
| Multi-Risk Scenarios (4) | Scenario Set | ⚠️ Basic | 3–4 | Single file | 2 |
| Part 1 Example Scenarios (4) | Scenario Set | ⚠️ Basic | 3–4 | Single file | 2 |
| Assignment 8 System Templates (4) | Templates | 🔧 Template | 8 | Single document | 3 |
| Week 10 Signal Tracking Game | Interactive Activity | 🔧 Active Dev | 10 | Modular (system + content) | 3 |
| Week 6 Worksheets | In-Class Activity | ✅ Complete | 6 | 2 PDFs + instructions | 4 |
| Week 8 Bias Probe Exercise | In-Class Activity | ✅ Complete | 8 | Single document | 4 |
| Week 11 Lesson Plan | Lesson Structure | ✅ Complete | 11 | 3 documents | 4 |

---

## RECOMMENDATIONS FOR EXEMPLAR SELECTION

**If selecting an exemplar for standardized case structure:**
- **Recommend**: Use **OptiRate** or **COVID-19 Misinformation Moderation**
- **Why OptiRate**: Accessible domain, clear AI-to-decision pathway, good for teaching systems thinking
- **Why COVID**: Richer governance contexts, professional code integration, teaches ambiguity and framework comparison
- **Both** now have standardized + lite pairs ready for classroom use

**If selecting an exemplar for student analysis process:**
- **Recommend**: Use **COVID-19 Misinformation Moderation**
- **Why**: Full framework comparison (ACM/IEEE), explicit bad-actor analysis, EDOCA integration, governance contexts, professional responsibility focus

**If creating a new exemplar:**
- **Structure**: Use standardized templates now in place (see protocol document)
- **Research/documentation**: Include sufficient background for instructors to teach context; scaffold student analysis to require students to reconstruct understanding

---

## FUTURE DEVELOPMENT OPPORTUNITIES

### Potential New Case Study: Autonomous Vehicle Ethics (Full Case)
**Suggested development**: Create a comprehensive case study anchoring autonomous vehicle decision-making, governance, and stakeholder analysis.

**Rationale**:
- **Moral Machine provides foundational data** (Week 1 dataset exercise)
- **Environment spans technical, policy, institutional, and stakeholder complexity** (ideal for BBS + EDOCA analysis)
- **Real-world implementations exist** (Tesla Autopilot, Waymo, regulatory frameworks) with documented incidents
- **Multiple governance contexts** (U.S., EU, China regulatory differences, professional responsibility, liability)
- **Professional responsibility dimensions** (IEEE, ACM codes apply; manufacturer responsibility; user trust)
- **Stakeholder diversity** (manufacturers, users, pedestrians, insurers, regulators, ethicists)

**Suggested structure** (using standardized case template):
- Opening narrative: Moral Machine context + real incident (e.g., Tesla Autopilot failure, Waymo incident)
- Case at a glance: technical capability, regulatory landscape, stakeholder conflicts
- Mediation pathways: data collection → training → deployment decision → user interaction → outcome → liability
- Stakeholder taxonomy: direct (drivers, pedestrians), economic (manufacturers, insurers), governance (regulators, ethicists), design (engineers, ethicists)
- Bidirectional risks: aggressive deployment vs. overly cautious constraints
- Professional responsibility: IEEE/ACM codes applied to autonomous system designers
- Discussion questions: tying back to Moral Machine data patterns, governance trade-offs, stakeholder conflicts

**Development status**: ⏸️ **Planned (Not yet developed)**

---

## NOTES ON DOCUMENT MAINTENANCE

This inventory should be updated whenever:
1. New case studies are developed
2. Cases are used in new assignments or contexts
3. Development status changes (e.g., Tier 3 → Tier 1)
4. New versions are created (standardized, lite, translated, domain-adapted)
5. Pedagogical usage patterns shift

Last updated: May 16, 2026
