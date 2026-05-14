# Misinformation, Bad Actors, and Ethical Responsibility in Mediated Systems
## A Conceptual Source Document for SEID 2364

## Purpose

This document explains a set of concepts that help analyze ethical responsibility in mediated socio-technical systems. It is designed to support discussion of misinformation, disinformation, bad actors, and professional responsibility within the broader context of data science ethics.

The central claim is that ethical outcomes in complex systems are not determined only by whether individual participants have good intentions. Ethical outcomes also depend on the frameworks used to evaluate the system, the criteria selected for judgment, the mediation pathways through which information travels, and the distribution of observability, control, and authority across agents.

Many socio-technical systems involve participants who are trying to act responsibly. A software engineer may believe they are improving usability. A platform moderator may believe they are reducing harm. A public-health official may believe they are protecting the public. A user may believe they are sharing important information with their community. Even when intentions are sincere, systems can still produce harm if information is distorted, incentives are misaligned, risks are not visible, or responsibility is distributed in ways that make accountability difficult.

This is one reason ethical frameworks matter. Different frameworks highlight different values: duties, consequences, rights, fairness, professional integrity, public welfare, institutional legitimacy, social stability, or individual freedom. The same action may therefore be evaluated differently depending on which framework is applied and which stakeholders are centered.

However, not every system failure results from good-faith ambiguity. Some actors deliberately exploit systems. Others behave recklessly, negligently, or strategically without accepting responsibility for foreseeable harm. This is where the concept of the **bad actor** becomes important.

---

## 1. Mediated Systems and Ethical Evaluation

In a simple ethical scenario, responsibility may appear to belong to a single person making a single choice. In mediated socio-technical systems, responsibility is rarely so simple.

A mediated system may include human users, software engineers, designers, platform companies, automated classifiers, recommendation systems, databases, moderators, regulators, public institutions, third-party services, infrastructure providers, and affected communities.

Information moves across these actors through pathways. A signal may begin as a human statement, become platform data, be classified by a moderation model, transformed into a risk score, routed through a policy rule, and finally appear to another user as visible, hidden, labeled, downranked, or removed.

At each transition, the signal can change. Context may be lost. Meaning may be compressed. Authority may shift. Observability may decrease. Control may move from one agent to another. Responsibility may become harder to assign.

This is why ethical analysis in this course does not ask only: “Was the final outcome good or bad?” It also asks where the signal originated, through what vectors it moved, who could observe each transition, who could control each transition, who had authority to permit or restrict action, where distortion entered, where distortion was amplified, and which stakeholders were affected but unable to intervene.

This is the connection to BBS and EDOCA. BBS helps describe mediation pathways. EDOCA helps evaluate effort, distortion, observability, control, and authority within those pathways.

---

## 2. Ethical Ambiguity in Good-Faith Systems

Many ethical problems arise in systems where participants are acting in good faith. These are not cases where someone is obviously trying to cause harm.

For example, a platform may remove misinformation because it believes doing so protects public safety. A regulator may require transparency because it believes public accountability is necessary. An engineer may build an automated classifier because manual review cannot operate at the necessary scale. A user may share a claim because they believe it will help their community.

In such cases, ethical evaluation depends heavily on the criteria used.

A consequentialist framework may ask whether the intervention reduces harm overall. A deontological framework may ask whether rights, duties, and legitimate procedures are respected. A virtue-oriented framework may ask whether the actors demonstrate honesty, competence, responsibility, humility, and care. A governance framework may ask whether the system includes oversight, accountability, proportionality, and avenues for redress.

The same system may look more or less ethical depending on which criteria are emphasized.

This does not mean that ethics is arbitrary. It means that ethical judgment in complex systems requires explicit criteria. Students should be able to state what they are prioritizing, why they are prioritizing it, and what their framework makes visible or obscures.

---

## 3. Infodemic and Mediated Information Crisis

The COVID-19 pandemic popularized the term **infodemic**, used by the World Health Organization to describe an overabundance of information, including false or misleading information, during a disease outbreak.

An infodemic is not simply a collection of false claims. It is an information environment in which accurate, false, misleading, outdated, uncertain, emotionally charged, and deliberately manipulative information may circulate simultaneously.

The problem is not only that some claims are false. The deeper problem is that individuals and institutions may struggle to determine what is true, what is uncertain, what is outdated, which sources are trustworthy, who has authority, what action is appropriate, and who is responsible for consequences.

Although the term infodemic emerged in a public-health context, the structure is not limited to health. Similar conditions appear in elections, climate communication, war reporting, financial panic, disaster response, scientific controversies, public safety emergencies, and AI-generated media environments.

For this broader structure, we can use the term **mediated information crisis**.

A mediated information crisis occurs when information moves through technical, institutional, and social systems in ways that make it difficult for affected agents to determine what is true, who has authority, what action is appropriate, and who is responsible for consequences.

In BBS terms, a mediated information crisis is a high-distortion, low-trust, multi-agent communication environment. Signals travel through many sources, vectors, destinations, platforms, institutions, and communities. Bad actors may exploit the system, but even good-faith actors may contribute to confusion if they amplify uncertain or poorly contextualized information.

---

## 4. Information Disorder and Informational Distortion

The word “misinformation” is often used casually to describe any false or misleading claim. For ethical analysis, more precise distinctions are useful.

Not all information problems are identical. Some involve the informational content itself. Others involve framing, context, uncertainty, mediation, amplification, or strategic deployment.

This section focuses on forms of **informational distortion**: situations in which information becomes misleading, deceptive, harmful, unstable, or difficult to interpret.

### False Information

**False information** is information that is factually incorrect.

False information is a broad descriptive category rather than a complete ethical explanation. False information may be created or shared accidentally, negligently, strategically, maliciously, jokingly, speculatively, computationally, or sincerely.

False information alone does not explain intent, responsibility, or mediation context.

### Misinformation

**Misinformation** is false or misleading information shared without necessarily intending harm.

A person may sincerely believe the claim is true. They may trust the person or community from which they received it. They may be confused, frightened, uncertain, or working from incomplete information.

### Disinformation

**Disinformation** is false or misleading information shared deliberately to deceive, manipulate, destabilize, profit, or gain strategic advantage.

Disinformation involves intentional deceptive use of information.

### Malinformation

**Malinformation** is information that may be true or partially true but is used in a harmful, misleading, or contextually manipulative way.

For example, a true fact may be stripped of context, selectively emphasized, emotionally framed, misleadingly compared, or strategically deployed to create a false impression.

### Incomplete and Speculative Information

Incomplete information is not automatically misinformation.

In many real-world systems, information is necessarily partial, uncertain, evolving, compressed, provisional, or speculative.

For example, a scientist may communicate preliminary findings before all evidence is available, a journalist may summarize only part of a developing event, a public-health authority may issue guidance while evidence is still changing, or a user may repost information without full context.

None of these situations automatically constitute misinformation.

However, incomplete, selectively presented, poorly contextualized, prematurely interpreted, or strategically framed information may become misleading depending on how it is amplified, interpreted, or deployed within a mediated system.

A technically true statement may still create a misleading impression if important contextual information is omitted, uncertainty is hidden, comparative risk is ignored, emotionally charged framing distorts interpretation, or audiences are encouraged to draw conclusions unsupported by the available evidence.

Speculative information is particularly important during crises, emerging scientific research, disaster response, financial instability, political conflict, and AI-generated media environments.

Speculation is not automatically misinformation. However, speculation may become misinformation or disinformation when uncertainty is hidden, exaggerated certainty is presented, or provisional claims are treated as established fact.

### Decontextualized Information

Information may become misleading because it is separated from the context necessary for accurate interpretation.

Examples include clipped video excerpts, screenshots without surrounding discussion, isolated statistics, graphs without labels, quotations removed from context, AI-generated summaries, and short-form social-media fragments.

The information itself may not be false, but the mediation pathway introduces distortion.

### Synthetic Information

Synthetic information is information generated artificially through computational systems.

Examples include AI-generated images, synthetic voices, deepfakes, generated text, AI-generated personas, and synthetic media environments.

Synthetic information is not automatically false or deceptive.

A synthetic image may be artistic, illustrative, fictional, educational, deceptive, propagandistic, or manipulative.

Synthetic information becomes ethically significant because it complicates provenance, trust, attribution, authenticity, observability, and verification.

### Informational Distortion in Mediated Systems

Mediated systems often structurally incentivize incomplete, compressed, emotionally engaging, or decontextualized information.

Headlines compress complexity. Recommendation systems reward engagement. Social media encourages rapid sharing before verification. Algorithms summarize, rank, clip, restate, and amplify information. Users frequently encounter fragments of information separated from their original context.

As a result, harmful distortion may emerge not only from outright falsehood, but also from oversimplification, omission, decontextualization, selective emphasis, uncertainty collapse, amplification pressure, and premature certainty.

These distinctions matter because the same false or misleading claim can move through a system by very different forms of agency.

A claim may be sincerely believed, socially reinforced, negligently amplified, strategically exploited, algorithmically amplified, institutionally tolerated, computationally transformed, or deliberately manufactured.

A platform may observe the claim without reliably observing the intent, context, or pathway conditions surrounding it.

This creates a technical and ethical problem. If two users share the same false claim, but one sincerely believes it and the other is deliberately manipulating people, should the system treat them the same way? If the system cannot tell the difference, what should it do?

---

## 4A. Systemic Distortion

Not all distortion emerges from the informational content itself.

Some distortion emerges from the systems through which information moves.

Systemic distortion concerns the exploitation, optimization, amplification, transformation, or destabilization of mediation pathways, infrastructures, algorithms, institutions, and communication systems.

The central question is not only:

“What is happening to the information?”

but also:

“What is happening to the system through which the information moves?”

Examples of systemic distortion include adversarial manipulation, algorithmic amplification, coordinated engagement attacks, optimization pressure, exploitative recommendation dynamics, prompt injection, data poisoning, opaque moderation systems, institutional incentive distortion, procedural opacity, and infrastructure vulnerabilities.

### Adversarial Manipulation

Adversarial manipulation involves the strategic exploitation of systems, infrastructures, algorithms, incentives, or mediation pathways in order to distort visibility, amplification, interpretation, trust, or system behavior.

Unlike disinformation, which primarily concerns deceptive informational content, adversarial manipulation primarily concerns strategic exploitation of systems.

Examples include coordinated brigading, recommendation-system gaming, prompt injection attacks, coordinated engagement manipulation, bot amplification networks, adversarial data poisoning, and strategic exploitation of ranking systems.

Adversarial manipulation may use true information, false information, synthetic information, emotionally charged information, or selectively framed information.

The manipulation resides not only in the content, but in the strategic exploitation of mediation pathways.

### Algorithmic Amplification

Algorithmic amplification occurs when computational systems increase the visibility, circulation, emotional intensity, or persistence of information.

Examples include recommendation systems, ranking systems, engagement optimization systems, trending systems, algorithmic feeds, and automated reposting systems.

Amplification systems may reward outrage, certainty, emotional engagement, novelty, divisiveness, or repetition.

As a result, systems may amplify distortion even when no single participant intends the final harmful outcome.

### Systemic Incentive Distortion

Systems may also become distorted because incentives reward harmful behavior.

Examples include engagement-based advertising systems, metrics rewarding controversy, attention economies, poorly aligned moderation incentives, or institutional structures prioritizing growth over accuracy.

These systems may systematically reward harmful informational behavior even when many individual participants believe they are acting responsibly.

---

## 5. Introducing the Bad Actor

A **bad actor** is an agent whose behavior degrades the integrity, safety, trust, fairness, or accountability of a system.

The phrase “bad actor” is intentionally retained because it is immediately recognizable from popular culture, cybersecurity, governance, media studies, and professional ethics. However, popular culture often imagines bad actors only as villains, criminals, propagandists, hackers, or obviously malicious individuals.

In mediated socio-technical systems, harmful agency is usually more complicated.

One purpose of this discussion is therefore to “pull back the curtain” on the idea of the bad actor. Harmful system behavior may emerge through sincere misinformation, negligence, laziness, recklessness, poor documentation, institutional incentives, optimization pressure, adversarial exploitation, computational drift, strategic manipulation, or deliberate malicious intent.

The same harmful outcome may therefore involve many different agents operating at different points in the mediation pathway.

This definition is operational rather than purely moral. A bad actor is not always a bad person. The term describes how an agent functions within a system, not necessarily the actor’s inner character.

Bad actors may be malicious, but they may also be negligent, reckless, misinformed, strategically self-interested, institutionally constrained, or procedurally evasive.

This distinction is important because many harmful systems do not contain a single villain. A system may become harmful through a combination of small decisions, poor documentation, weak oversight, hidden incentives, unclear authority, lack of testing, unexamined assumptions, or failure to anticipate foreseeable misuse.

At the same time, some systems really do contain malicious actors. Hackers, scammers, propagandists, fraudsters, and hostile networks may deliberately exploit vulnerabilities, trust relationships, or information pathways.

Ethical system design must therefore account for both good-faith ambiguity and bad-faith exploitation.

This also means that harmful behavior cannot always be reduced to a single individual making a malicious choice. Harm may emerge from interactions among people, institutions, platforms, recommendation systems, automated classifiers, optimization systems, and communication pathways.

For example, a user may sincerely believe a false claim, a recommendation system may amplify the claim because it increases engagement, an influencer may strategically repeat it because controversy produces attention, a platform may fail to intervene because moderation is expensive or politically risky, and a malicious network may intentionally exploit the confusion.

No single participant necessarily “owns” the entire harmful outcome, yet the mediated pathway still produces real harm.

---

## 6. Types of Bad Actors

The following categories are not mutually exclusive. They are tools for analysis.

### Misinformed Actor

A misinformed actor shares false or misleading information while believing it to be true.

Example: A user shares a false medical claim because a trusted family member, community leader, or online group endorses it.

The actor may cause harm, but the harm does not arise from deliberate deception. Ethical response may require correction, education, context, or trust-building rather than punishment alone.

### Negligent Actor

A negligent actor fails to meet a reasonable standard of care.

Example: A software engineer fails to validate input properly and unintentionally leaves a vulnerability in a system. The engineer did not intend harm, but their failure to follow reasonable security practices creates a pathway for harm.

Negligence matters because professional responsibility includes duties of testing, documentation, review, and risk awareness. Good intentions do not erase foreseeable failures.

### Reckless Actor

A reckless actor proceeds despite foreseeable risk.

Example: A platform deploys an automated moderation classifier at large scale even though internal testing shows high error rates for certain languages or communities.

The actor may not intend harm, but they knowingly accept a risk that others will bear.

### Strategic Actor

A strategic actor exploits system incentives or information asymmetries for advantage, even if harm is not the primary goal.

Example: An influencer amplifies misleading claims because controversy increases attention, followers, and revenue.

Strategic actors may not care whether a claim is true. They care that the system rewards the claim’s circulation.

### Malicious Actor

A malicious actor deliberately seeks to deceive, steal, damage, destabilize, manipulate, or extract value.

Example: A hacker deliberately searches for a software back door, enters a system without authorization, and steals data or money.

This differs from the engineer who accidentally created the vulnerability. The engineer may be negligent. The hacker is malicious.

### Computational or Algorithmic Actor

A computational or algorithmic actor is a system that participates in harmful mediation pathways through optimization, amplification, filtering, generation, ranking, classification, or automated response.

Example: A recommendation system learns that outrage-producing content increases engagement and therefore amplifies emotionally charged misinformation because the optimization metric rewards attention rather than accuracy.

Another example: A generative AI system hallucinates dangerous medical advice and repeatedly reproduces it because the underlying model predicts plausible language rather than factual correctness.

Computational actors may not possess human intent, but they still alter mediation pathways and can produce harmful outcomes.

### Hybrid Actor

A hybrid actor combines cognitive and computational agency.

Example: A coordinated propaganda campaign uses generative AI systems to rapidly create persuasive synthetic content while human operators strategically target specific communities and exploit algorithmic amplification systems.

In hybrid systems, harmful behavior may emerge from interactions among many agents rather than from a single source.

### Institutional Actor

An institutional bad actor is an organization whose incentives, policies, or structures produce harm even when individuals inside the organization believe they are doing their jobs.

Example: A company rewards engagement growth while publicly claiming to reduce harmful misinformation. Employees may follow internal metrics, but the institution may still amplify harmful content.

Institutional bad acting often emerges when incentives are misaligned with public responsibility.

### Procedural Actor

A procedural bad actor follows rules narrowly while undermining the purpose of those rules.

Example: A platform technically publishes transparency reports but provides them in a form that users, researchers, or regulators cannot meaningfully interpret.

The actor may claim compliance, but the procedure does not create real accountability.

---

## 6A. Harmful System Components

Not every harmful element in a mediated system is best understood as an intentional actor or agent.

Some system components may systematically produce dangerous, distorted, insecure, unfair, or exploitable outcomes even when no single participant deliberately intends harm.

These components may still function as persistent sources of distortion, vulnerability, amplification, opacity, or systemic instability.

Examples include insecure architectures, poorly designed interfaces, opaque recommendation systems, biased datasets, flawed optimization metrics, undocumented APIs, unmonitored adaptive systems, insecure defaults, hidden feedback loops, exploitative engagement metrics, inadequate moderation tooling, and poorly designed incentive structures.

For example, a recommendation system optimized primarily for engagement may systematically amplify emotionally charged misinformation even if no engineer explicitly intends that outcome. The harmful behavior emerges from the structure of the optimization system itself.

Similarly, a poorly documented API may create conditions for misuse, security failure, or unintended access. A biased training dataset may produce discriminatory outputs even if individual developers believe they are acting fairly.

These cases are important because harmful outcomes may emerge from system structure rather than from isolated malicious intent.

This means ethical analysis must evaluate not only agents, but also architectures, protocols, interfaces, datasets, optimization functions, incentive systems, feedback loops, and infrastructure conditions.

In BBS terms, harmful mediation may emerge through the structure of the pathway itself.

A vector does not need to contain a malicious agent in order to produce harmful distortion. The pathway may itself be poorly designed, unstable, opaque, exploitable, or optimized toward harmful outcomes.

This distinction matters because modern socio-technical harm often emerges from interactions among human agents, computational agents, institutional incentives, and harmful system structures.

A harmful system may therefore persist even when many participants believe they are acting responsibly.

---

## 7. Back Doors, Negligence, and Malicious Exploitation

The distinction between negligence and malicious action can be illustrated through a software back door.

Imagine a software engineer working on a login system. The engineer writes code that unintentionally leaves an insecure administrative access pathway. The engineer does not intend to create a back door. They may be rushed, undertrained, poorly supervised, or working in an organization without adequate code review. The vulnerability exists because of negligence, weak process, or institutional failure.

Now imagine a malicious hacker discovers the vulnerability. The hacker deliberately uses it to enter the system and steal customer data. This is a different ethical category. The hacker is not merely participating in a flawed system. The hacker is intentionally exploiting the system for harm or gain.

Both actors are part of the harm pathway.

The engineer may have created the vulnerable vector. The hacker may have exploited it. The organization may have failed to provide review, testing, security culture, or accountability. A regulator may have lacked observability. Users may bear the harm without having any control over the system.

This example shows why ethical analysis should avoid overly simple blame.

The question is not only:

Who did the bad thing?

The better questions are who created the vulnerability, who exploited it, who could have observed it, who controlled the relevant system transition, who had authority to prevent or correct it, who benefited, who was harmed, and what professional standards should have prevented the failure.

This is where BBS and EDOCA become useful. A back door is not only a technical flaw. It is a mediation pathway that allows unauthorized transition from one state to another. Ethical analysis must evaluate how that transition became possible and who had responsibility at each stage.

---

## 8. Bad Actors and Mediation Pathways

In BBS terms, a harmful system event can often be described as a pathway:

Source → Vector → Destination

A bad actor may intervene at any point in that pathway.

A bad actor may manipulate the Source by creating false or misleading input.

A bad actor may manipulate the Vector by exploiting a transformation, communication channel, algorithm, API, interface, or security vulnerability.

A bad actor may manipulate the Destination by targeting how a person, institution, or system interprets the signal.

For example:

- A disinformation network creates false claims at the source.
- A recommendation algorithm amplifies them through the vector.
- A generative AI system restates them persuasively.
- A ranking algorithm increases their visibility because controversy drives engagement.
- A user community receives and interprets them as trusted information at the destination.

The harm may not reside in any single component. It emerges through the pathway.

This is why ethical analysis must consider both agency and mediation. Bad actors exploit pathways. Negligent actors may create exploitable pathways. Institutions may tolerate pathways because they serve organizational goals. Automated systems may amplify the pathway without understanding the harm.

---

## 9. Observability, Control, and Authority

Bad-actor analysis depends on observability, control, and authority.

**Observability** asks who can see what is happening.

A platform may observe a post but not the intent behind it. A user may observe that content was removed but not why. A regulator may observe a transparency report but not the internal classifier decisions. An engineer may observe system logs but not social consequences.

**Control** asks who can change what is happening.

A platform may control ranking, labeling, removal, appeal mechanisms, and moderation policies. A user may control what they post but not how the system distributes it. A regulator may influence policy but not directly operate the platform.

**Authority** asks who has legitimate permission to act.

A public-health agency may have expertise but not direct control over a platform. A platform may have technical control but contested legitimacy over public discourse. A court may have formal authority but limited real-time operational capacity.

In complex systems, observability, control, and authority often do not align.

That misalignment is ethically significant. An actor may have control without legitimate authority. Another actor may have authority without operational control. A third actor may be harmed without observability or recourse.

Bad actors often exploit exactly these gaps.

---

## 10. Why Professional Responsibility Matters

The concept of the bad actor helps explain why professional responsibility matters.

Professional ethics is not only about avoiding intentional wrongdoing. It is also about avoiding negligence, recklessness, avoidable opacity, poor design, inadequate testing, misleading communication, and failure to consider foreseeable misuse.

A professional may become part of a harmful pathway without intending harm.

A data scientist may choose a dataset without examining representational bias. An engineer may release a feature without adequate security review. A designer may create an interface that hides meaningful user choice. A platform team may optimize for engagement while claiming neutrality. A researcher may publish results without disclosing limitations.

In each case, the actor may not be malicious. But professional responsibility requires more than absence of malice.

It requires care, competence, honesty, documentation, testing, transparency, and attention to the consequences of system design.

This is why professional codes of conduct become important later in the course. They help define standards that reduce the likelihood that professionals and institutions become sources of harm.

---

## 11. Conclusion

Misinformation, disinformation, and bad actors cannot be analyzed only by asking whether a claim is true or false. Ethical analysis must also ask how information moves, who moves it, who benefits, who is harmed, who can observe the pathway, who can control it, and who has authority over it.

In mediated systems, harm may arise from sincere error, social trust, negligence, recklessness, strategic exploitation, malicious action, institutional incentives, or procedural evasion.

The concept of the bad actor helps identify harmful agency, but it should not be used simplistically. A bad actor is not always a villain. Sometimes the actor is malicious. Sometimes the actor is careless. Sometimes the actor is trapped inside an institution that rewards harmful behavior. Sometimes the actor follows rules while undermining the purpose of those rules.

For data science ethics, the central challenge is to design and evaluate systems that can handle both good-faith ambiguity and bad-faith exploitation.

That requires more than ethical intention. It requires mediation-aware analysis, professional responsibility, and attention to observability, control, authority, and accountability.

