# Example: EDOCA Analysis of Mediation Pathways

**Purpose**: Demonstrate how to decompose a system into individual Source-Vector-Destination (SVD) transitions, identify critical inflection points, and then apply EDOCA analysis to selected transitions.

**Key principle**: EDOCA is applied to **individual SVDs**, not to entire systems or pathways. Before analyzing anything, you must first map all the SVDs in your system.

---

## Step 1: Identify All SVDs in the System

The first step is **decomposition**: break the entire mediation pathway into discrete S → V → D transitions.

### Pathway Overview: Algorithmic Hiring

**What happens (from candidate perspective)**:
```
Candidate submits resume → System processes → Ranking emerges → HR makes decision → Acceptance/rejection
```

But this is too coarse. Each arrow is actually one or more SVDs.

### Decomposing into SVDs

**Processing pathway (candidate-facing):**

| SVD ID | Source | Vector | Destination | Actor/Location |
|---|---|---|---|---|
| **SVD-P1** | Raw resume (unstructured, variable format) | Resume parsing, OCR, field detection | Normalized resume data | Vendor infrastructure |
| **SVD-P2** | Normalized resume data | Feature extraction, embedding, model inference | Scored profile (numeric ranking) | Vendor algorithm |
| **SVD-P3** | Scored profile | Ranking aggregation, tie-breaking, display | Candidate list sorted by score | HR system |
| **SVD-P4** | Candidate list | HR decision-making (manual review, interviews, offers) | Hiring outcome | Hiring team |

**Algorithm creation pathway (usually invisible to candidates):**

| SVD ID | Source | Vector | Destination | Actor/Location |
|---|---|---|---|---|
| **SVD-A1** | Historical hiring decisions + resumes | Data collection, cleaning, labeling | Training dataset | Vendor data team |
| **SVD-A2** | Training dataset | Feature engineering, model architecture choice, hyperparameter tuning | Trained model (weights) | Vendor ML team |
| **SVD-A3** | Trained model + validation dataset | Testing, bias auditing, fairness metrics | Model performance report | Vendor QA team |
| **SVD-A4** | Model performance report + business decision | Deployment approval, threshold setting, integration planning | Deployed system | Vendor + HR leadership |

**Why both pathways matter**: 
- **SVD-P** pathway is what candidates experience
- **SVD-A** pathway is where biases are *baked in*
- Decisions in SVD-A *constrain* outcomes in SVD-P

### The Critical Insight

When analyzing a hiring algorithm incident, you might initially think the problem is in SVD-P2 (the scoring). But the root cause is often in SVD-A1 or SVD-A2 (what data was used, which features were chosen). The processing pathway just *executes* what the creation pathway built.

---

## Step 2: Identify Critical Inflection Points

Not every SVD is equally important. **Select 2–3 critical transitions** where:
- A major transformation occurs
- Multiple actors converge
- Information is distorted or lost
- Responsibility becomes ambiguous

**For the hiring example, critical SVDs are**:

1. **SVD-A1** (Training data creation): What historical data was labeled as "good hire"? Whose successes are represented? Whose are missing?
2. **SVD-P1** (Resume normalization): Format bias, OCR errors, field detection failures
3. **SVD-P2** (Scoring): Feature weighting, interaction effects, emergent bias
4. **SVD-A4** (Deployment decision): Was the system tested on diverse candidate pools? Were known biases accepted?

You would then apply **detailed EDOCA to 2–3 of these**, not all.

---

## Step 3: Apply EDOCA to Selected Critical SVDs

Once you've identified the SVDs and selected 2–3 for deep analysis, apply EDOCA to each one.

### Selected SVD for Detailed Analysis 1: SVD-A1 (Training Data Creation)

**The transition:**
```
Historical hiring decisions + candidate resumes
    ↓ [Vector: Data collection, cleaning, labeling, documentation]
Training dataset (labeled examples of "good hires" and "poor hires")
```

**Actors:**
- **Historical hiring team** (made hiring decisions that created the labels)
- **Vendor data team** (selected which data, how to label it, defined "good hire")
- **Candidates** (provided the source data, but have no voice in labeling)

**Why critical?** This is where the bias gets *embedded*. If the historical hiring decisions were biased (favored Stanford grads, penalized gaps, underrepresented certain demographics), the model will *learn* and amplify those biases.

#### EDOCA for SVD-A1 (Training Data)

**Effort / Energy**
- Historical hiring team's hiring decisions (already made, cost is sunk)
- Vendor data team: time to extract historical data, clean it, label it
- HR/hiring organization: providing access to historical records

**Distortion / Fidelity**
- **Selection bias**: Which historical data was retained? (Fired employees may be purged; promotions may be incomplete)
- **Labeling bias**: What counts as a "good hire"? (Stayed long enough? Revenue generated? Got promoted? By whose standards?)
- **Representation bias**: Whose resumes are in the dataset? (If women, non-binary candidates, or diverse backgrounds were underrepresented in past hiring, they're underrepresented in training data)
- **Temporal bias**: Did hiring criteria change over time? (Training data may mix old and new standards)
- **Outcome bias**: Only "successful" outcomes may be labeled; unsuccessful hires may be missing

**Result**: Training dataset *inherits and encodes* the biases from historical hiring decisions. Model learns from a *biased reflection of reality*, not from reality itself.

**Observability**
- **Vendor data team**: Can see which resumes were selected, how labeling was done
- **HR/organization**: Gave access but may not have visibility into how data was cleaned/labeled
- **Candidates**: Have zero visibility into whether their hire/non-hire was included, labeled fairly, or represents them accurately
- **Future hiring manager**: Will receive a "trained model" but will not know what biases were baked in

**Control: Who Can Alter the Training Dataset?**
- **Vendor data team**: Can choose which data to include, how to label, which candidates to include/exclude
- **Historical hiring team**: Cannot go back and change historical decisions
- **Organization leadership**: Can request data be rebuilt with different criteria, but often doesn't
- **Candidates**: Have zero control over whether their data is included or how they're labeled

**Authority**
- **Organization**: Owns historical data, decides what can be shared with vendor
- **Vendor**: Has authority to define labeling criteria, decide what counts as "good hire"
- **Data protection regulations** (GDPR, etc.): Increasingly require transparency on training data

**Key insight**: The moment the training dataset is frozen, the model's bias is *locked in*. All downstream decisions (SVD-P2, SVD-P3) will execute that locked-in bias.

---

### Selected SVD for Detailed Analysis 2: SVD-P1 (Resume Normalization)

**The transition:**
```
Raw resume (PDF, Word, text, various formats/structures)
    ↓ [Vector: Parsing, OCR, field detection, standardization]
Normalized resume data (structured fields)
```

**Actors:**
- **Candidate** (submits resume in whatever format they used)
- **Vendor infrastructure** (runs the parsing pipeline)
- **Hiring team** (receives normalized data, often doesn't see original)

**Why critical?** This is the **hidden failure point** where format bias is introduced. Many students think "the algorithm" starts with structured data, but normalization is where the first distortion enters.

#### EDOCA for SVD-P1 (Resume Normalization)

### **Effort / Energy**

**What resources enable normalization?**

- Candidate effort: formatting resume, saving in some format (PDF, Word, Google Docs, etc.)
- Vendor effort: building parsers for multiple formats, training OCR systems, designing field detection
- Infrastructure: servers running parsers, OCR engines, storage
- Ongoing effort: maintaining parsers as formats change (new Word versions, Apple Pages, ATS exports, etc.)

**Who provides each?**

- Candidate provides the raw artifact (often in whatever format they used)
- Vendor designed the parser pipeline
- Cloud provider (AWS/Azure/Google) runs OCR and inference
- Hiring team provides labor (spot-checking if parsing worked)

**Cost asymmetry**: Vendor built it once; candidate pays every time with format risk.

---

### **Distortion / Fidelity in Normalization**

**Sources of distortion**:

1. **Format-specific failures**:
   - PDF with embedded images? OCR fails, education history invisible
   - Word file with custom fonts? Parser skips them
   - Google Docs with comments? Comments become data or are lost
   - ATS export? Data is pre-structured but often mangled
   - Non-Latin characters (name, education location)? OCR or encoding errors

2. **Field detection errors**:
   - "Skills" section detected as "Experience"
   - Dates parsed incorrectly (2 months = 0 years; "present" mishandled)
   - Education level inferred wrong (trade school vs. university)
   - Gaps or career changes not detected as intentional (parental leave, illness, sabbatical)

3. **Representation loss**:
   - Relative weight and visual hierarchy lost (what candidate emphasized is invisible)
   - Narrative explanation ("took time off to care for family") becomes missing data
   - Context stripped ("Top performer in fast-growing startup" → just "startup")

4. **Downstream cascade**:
   - Errors in normalization feed into scoring (garbage in → garbage out)
   - Once a field is wrong (education, years of experience), downstream scoring cannot correct it

**Does effort reduce distortion?**

- Candidate effort (polished resume, standard format) *may* help, but only if they happen to use a format the parser handles well
- Vendor effort (multiple parsers, OCR, error checking) *could* reduce distortion, but:
  - Costs money (they often use cheap OCR)
  - Requires ongoing maintenance (new formats emerge constantly)
  - Often deprioritized (not a revenue driver)

**Result**: Distortion is **high, patterned, and invisible**. Candidates from privileged backgrounds may use standard Word/PDF; candidates from global/low-resource contexts may submit screenshots, phone images, or formats the parser doesn't handle.

---

### **Observability in Normalization**

| Actor | Sees Raw Resume? | Sees Normalized Fields? | Sees Parsing Errors? | Sees OCR Output? |
|---|---|---|---|---|
| **Candidate** | Yes (their own) | Almost never | No | No |
| **Hiring Team** | Maybe (in ATS) | Maybe (summary display) | Only if obvious | No |
| **Algorithm** | No (already normalized) | Yes | No | No |
| **Vendor** | If logged | If logged | Only if monitored | Only if monitored |
| **Infrastructure** | Data in transit | Data in transit | Not visible | Raw output in logs (maybe) |

**Critical gap**: Candidate has no visibility into how their resume was parsed or where errors occurred. If their resume failed to parse correctly, they have no way to know or correct it.

---

### **Control in Normalization**

**Who can alter the intermediate state (normalized fields)?**

1. **Vendor**: 
   - Can choose which parsers, OCR engines, field templates
   - Can update parsers
   - But this is done *globally* for all candidates, not per-resume

2. **Hiring team**:
   - Can (in some ATS systems) manually edit normalized fields
   - But this is rare and labor-intensive
   - Often not allowed ("trust the system")

3. **Candidate**:
   - Can resubmit resume in different format (hope it parses better)
   - Cannot directly control how it's parsed
   - Cannot see or fix parsing errors

4. **Algorithm**:
   - Cannot fix normalization errors (they're upstream)
   - Must accept whatever normalized data it receives

**Control reality**: Vendor designs once; everyone else lives with the consequences.

---

### **Authority in Normalization**

- **Vendor**: Authority to choose parsing approach, update parsers, set field requirements
- **Hiring team**: Authority to deploy system, but limited authority to override or inspect
- **Regulations**: Increasingly (EU AI Act), vendors must show they tested parsers on diverse inputs
- **Candidate**: No authority; cannot demand manual review or format accommodation

**Authority gap**: Vendor has authority to build the parser but little incentive to make it robust.

---

## EDOCA Analysis: Transition 2 (Scoring)

Now, *given* normalized resume data, the algorithm scores it.

### **Effort / Energy**

**What resources enable scoring?**

- Model training: historical resumes, hiring decisions, compute
- Deployment: APIs, servers, monitoring
- Maintenance: retraining, updating weights

**Result**: High upfront vendor effort; candidate bears no cost.

---

### **Distortion / Fidelity in Scoring**

**Sources of distortion**:

1. **Feature loss**:
   - "Top performer at fast-growing startup" → just "startup" experience
   - Normalized fields lose context, nuance, narrative

2. **Feature bias**:
   - Model trained on historical hires (biased dataset)
   - Learns: "graduates from Stanford → higher performer"
   - Learns: "gap in employment history → less reliable"
   - Learns: "female-coded names → lower technical score" (if training data was male-biased)

3. **Interaction effects**:
   - Same resume gets different scores based on competition (relative ranking)
   - Same resume rescored if model is updated
   - Hidden interactions: "female + engineering field" triggers different weighting than "male + engineering field"

**Critical: Distortion is cumulative**
- If normalization failed (e.g., OCR dropped "PhD" → looks like high school grad), scoring cannot recover
- Distortion from Transition 1 *amplifies* in Transition 2

**Result**: Multiple failure points, compounding errors.

---

### **Observability in Scoring**

(Same as before—algorithm sees everything, candidate sees nothing, hiring team sees only final ranking)

---

### **Control in Scoring**

**Who can alter the final score/ranking?**

- **Vendor**: Can retrain, update features, change weights
- **Hiring team**: Can override score, manually adjust ranking
- **Algorithm**: Cannot change its own logic (absent autonomous redesign)
- **Candidate**: Cannot challenge score (no transparency)

**Emergent control**: Algorithm may find unintended patterns in data, amplifying bias in ways not explicitly programmed.

---

## Step 4: Understand How Upstream SVDs Constrain Downstream SVDs

This is the critical insight most students miss: **Decisions made in the creation pathway (SVD-A) lock in constraints that determine what's possible in the processing pathway (SVD-P).**

### Pathway Constraints: SVD-A1 → SVD-P2

**In SVD-A1** (Training data), the vendor data team decides:
- Which historical hiring decisions to include (e.g., only those marked "successful")
- How to label "good hire" (e.g., "stayed 2+ years")
- Which candidates' resumes are included (e.g., those still in the system)

**This constrains SVD-P2** (Scoring) because:
- The model can only learn patterns from the data it was given
- If training data overrepresented Stanford graduates, model learns "Stanford → good hire"
- If training data underrepresented women in certain roles, model won't learn to recognize their qualifications
- If "success" was defined narrowly (stayed long, got promoted), model won't recognize other success patterns

**The model cannot "fix" biases that were baked in at the data level.** It can only execute what it learned.

### Pathway Constraints: SVD-P1 → SVD-A2 → SVD-P2

**In SVD-P1** (Normalization), parsing errors introduce distortion (OCR fails, fields misdetected).

**In SVD-A2** (Model training), the model learns from the *normalized* data, which already includes those distortions.

**In SVD-P2** (Scoring), when a new candidate submits a resume in the same problematic format, the same parsing errors occur, and the model's learned patterns (which were trained on similar errors) execute.

**Result**: Format bias gets *baked in* at training time, then *replayed* at inference time.

### The Responsibility Trap

This is where responsibility becomes diffuse:

- **Vendor data team** (SVD-A1): "We just used the data the organization gave us"
- **Vendor ML team** (SVD-A2): "We trained on the data we received; bias was in the source"
- **Vendor deployment team** (SVD-A4): "The model passed our tests"
- **Hiring team** (SVD-P4): "We're just using the tool"
- **Candidate**: Harmed by a system where no single decision-maker explicitly chose to discriminate

But collectively, each SVD's decisions constrained the next, locking in bias systematically.

---

## Cumulative Distortion Across Both Transitions

This is the key insight:

```
Raw resume (rich context) 
    → Parsing/normalization errors (format bias, OCR failures, field detection misses)
    → Normalized data (already degraded)
    → Scoring (learns from degraded + biased training data)
    → Final score (distortion compounded)
```

**Where does distortion first appear?** Parsing (Transition 1)  
**Where is it amplified?** Scoring (Transition 2), which cannot see or correct Transition 1 errors  
**Where is it most invisible?** Both—candidates see neither stage

---

## Observability Across Both Transitions

| Actor | Visibility to T1 (Parsing)? | Visibility to T2 (Scoring)? | Overall Visibility? |
|---|---|---|---|
| **Candidate** | No | No | Zero |
| **Hiring Team** | Partial (ATS display) | Partial (score only) | Minimal |
| **Algorithm** | N/A (accepts normalized input) | High (internal) | Partial (can't see T1 errors) |
| **Vendor** | High (if monitored) | High (if monitored) | High (but scattered) |

**Asymmetry**: System has maximal observability at design/infrastructure level; candidate has zero; hiring team has token visibility.

---



---

## Part 4 Connection: Where Does Control Assumption Break?

**Starting assumption**: Algorithm applies fixed logic; vendor designed it; hiring team uses it; candidate has no control.

**Where assumption breaks down**:
1. Algorithm transcends design (finds exploits, generates emergent bias)
2. Vendor has contractual limits on transparency (can't fully audit their own system)
3. Hiring team lacks authority to override (pressured to trust the ranking)
4. Candidate discovers bias exists but cannot request manual review

**When does this matter for harm?**
- If algorithm works as designed → vendor + hiring team share responsibility
- If algorithm transcends design and vendor didn't test for it → unclear responsibility (vendor claims "unintended," algorithm doesn't claim anything)
- If hiring team knows algorithm is biased but uses it anyway → hiring team responsible
- If candidate excluded because of emergent bias they could never have prevented → harm, but whose fault?

---

## Part 7 Connection: Responsibility Distribution Across Both Transitions

### Stated Responsibility

- **Vendor**: "We provide tools; you use them how you choose"
- **Hiring Team**: "We use the technology we're given; the system is objective"
- **Algorithm**: (has no voice)
- **Candidate**: (has no voice)

### Actual Responsibility (Where It Sits)

**Transition 1 (Normalization)**:
- **Vendor**: Built parser with known limitations (chose cheap OCR, limited format support)
- **Candidate**: Harmed by format bias despite doing nothing wrong
- **Hiring Team**: Often unaware this stage exists; assumes data is clean

**Transition 2 (Scoring)**:
- **Vendor**: Built model trained on biased historical data; made feature/architecture choices
- **Hiring Team**: Deployed at scale despite fairness warnings
- **Algorithm**: Executes; amplifies biases from training data and Transition 1 errors
- **Candidate**: Harmed by two layers of compounded distortion

### Mismatches

| Dimension | Mismatch | Why It Matters |
|---|---|---|
| **Visibility** | Candidate sees nothing; algorithm sees everything | Candidate cannot contest or correct |
| **Control** | Vendor has design control; candidate has zero | System is optimized for vendor efficiency, not candidate equity |
| **Authority** | Hiring team has formal authority; lacks visibility to use it | Authority without information is nominal |
| **Responsibility** | Distributed across vendor, hiring team, algorithm | No single actor feels responsible for outcomes |
| **Leverage** | Vendor has most leverage; candidate has none | Power asymmetry with no countervailing force |

### Where Responsibility Disappears

- **Transition 1 errors**: "Just an artifact of resume submission format"
- **Transition 2 errors**: "The model learned from historical data"
- **Combined**: "Unintended consequences of complex systems"

But responsibility doesn't disappear—it **diffuses** into a space where no one explicitly chose to create harm, yet harm emerges systematically.

---

## TL;DR for Students: The Three-Step EDOCA Process

### Step 1: Decompose into SVDs (First!)

Before analyzing anything, break the entire system into discrete S → V → D transitions. Include:
- **Processing pathway** (what happens to the candidate/input)
- **Creation pathway** (how the algorithm was built and deployed)
- **Other pathways** (feedback, updates, accountability)

Don't try to EDOCA the whole system at once.

### Step 2: Identify Critical Inflection Points

Select 2–3 SVDs for deep analysis. Choose ones where:
- Major transformations occur
- Multiple actors converge
- Information is distorted or lost
- Responsibility becomes ambiguous

Look for both upstream (creation) and downstream (processing) SVDs.

### Step 3: Apply EDOCA to Selected SVDs

For each selected SVD, analyze:
1. **Effort**: What resources enable it? Who provides them?
2. **Distortion**: What signal is lost, transformed, or hidden?
3. **Observability**: Who can see what's happening?
4. **Control**: Who can alter the destination state?
5. **Authority**: Who can permit, restrict, or halt it?

### Step 4: Trace Pathway Constraints

**This is critical**: Show how decisions in upstream SVDs (creation pathway) lock in constraints that determine outcomes in downstream SVDs (processing pathway).

- **SVD-A1 choices** (training data) → constrain **SVD-P2 learning** (what patterns the model can learn)
- **SVD-A2 choices** (model architecture, features) → constrain **SVD-P2 execution** (how scores are calculated)
- **SVD-P1 errors** (format parsing) → become **SVD-P2 inputs** (distortion compounds)

### Key Insight

Responsibility diffuses across multiple SVDs because:
- Each SVD has a different set of actors
- Each SVD's decisions constrain but don't determine the next SVD
- No single decision-maker chose to create harm—it emerged from the chain

This is why it's critical to map **all the SVDs first** before analyzing any single one. Only then can you see where responsibility actually sits and where it disappears.

---

## Key Takeaways for Assignment 9

When you analyze your incident:

1. **Start by identifying all SVDs** — don't jump straight to EDOCA
2. **Include both creation and processing pathways** — upstream decisions determine downstream constraints
3. **Select 2–3 critical SVDs for deep analysis** — not the whole system
4. **Apply full EDOCA to each selected SVD** — Effort, Distortion, Observability, Control, Authority
5. **Trace distortion cumulatively** — errors from early SVDs feed into and amplify in later SVDs
6. **Show where responsibility diffuses** — how multiple actors' decisions combine to create harm no single actor fully chose
7. **Distinguish** whether harm is truly unintended, foreseeable but not prevented, or designed with plausible deniability (Part 6 of the assignment)
