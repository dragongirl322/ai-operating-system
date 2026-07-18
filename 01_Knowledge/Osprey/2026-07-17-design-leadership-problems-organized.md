---
title: Design Leadership Problems — Organized and Ranked
date: 2026-07-17
tags:
  - osprey
  - design-leadership
  - ai-experience
  - organizational-design
  - synthesis
  - territory
---

# Design Leadership Problems — Organized and Ranked

Synthesized July 17, 2026 from all Osprey vault notes (June 18 – July 17, 2026).

Source notes:
- [[2026-06-18-osprey-ai-overnight-brief-and-follow-up]]
- [[2026-06-18-osprey-ai-design-patterns-and-territory-compare]]
- [[2026-06-20-ai-ux-research-detail]]
- [[2026-06-22-osprey-ai-design-leadership-problems]]
- [[2026-06-26-osprey-ai-experience-design-leadership-synthesis]]
- [[2026-06-29-ai-coordination-and-interaction-centered-intelligence]]
- [[2026-06-30-osprey-synthesis-print]]
- [[2026-07-01-codex-usage-and-action-level-ai-governance]]
- [[2026-07-02-osprey-controllability-agent-governance-project-cannes]]
- [[2026-07-14-magentic-ui-avenir-ux-design-leadership]]
- [[2026-07-17-ux-leadership-coherence-evidence-adaptability-trust]]

---

## Part 1 — AI Solutions: Design Leadership Problems

Problems about the craft, mechanics, and architecture of AI experiences themselves.

---

### Cluster A — Authority & Permission

The foundational layer. Before delegation, oversight, or transparency can work, people need to know what the AI is allowed to do.

**Designing the AI authority model.**
How do users, admins, auditors, and customers know what an AI system is allowed to see, infer, remember, decide, and do — and how do they revoke it? Current permission dialogs are too blunt for AI behavior. No platform publicly owns this fully. It appears across every note as the single most recurring spine.

**Designing context and memory transparency.**
How can users inspect, control, and correct what the AI knows about them, their work, and their permissions? Context-aware AI is becoming the default across Apple, Microsoft, Google, Meta, and enterprise agents. The risk is invisible context assembly — what the corpus calls "context as invisible authority." A design leader can own the "what I can see / what I can remember / what I can do" layer.

**Making AI action governable without making it unusable.**
Governance must live at the action level, not only in policy docs or broad permission screens. Read, write, send, delete, deploy, pay, publish are different authority levels requiring different controls. The design problem is graduated autonomy: low-risk actions with logging, high-risk actions with named human authority — rather than blanket approval friction.

---

### Cluster B — Delegation & Oversight

How humans assign work, monitor it, intervene, and remain accountable.

**Making delegation legible and bounded.**
How does a human safely delegate work to AI without losing situational awareness or accountability? The unit of UX is no longer a single response — it is the full loop: goal, scope, plan, execute, monitor, interrupt, review, recover. The empirical backing is strong: the business-context UX paper found a 37.8 percentage-point preference lift for high-transparency prototypes.

**Designing proportional oversight by risk.**
When should AI act automatically, when should it ask, when should it require approval, and when should it hand off to a human? One-size-fits-all oversight makes AI either unusable or unsafe. The answer is graduated control calibrated to reversibility, stakes, and user expertise: low-risk automation, medium-risk review, high-risk approval, sensitive-domain human handoff.

**Building intervention and recovery as core UX.**
How do users stop, correct, undo, redirect, resume, or escalate when something goes wrong? Magentic-UI formalizes this as co-planning, co-tasking, action approval, answer verification, memory, and multi-tasking — but most products still treat recovery as an afterthought. Recovery design is also where accountability becomes tangible.

**Agent controllability during execution.**
Can a running agent be reliably interrupted, overridden, redirected, and constrained mid-task? The May 2026 controllability paper separates alignment (a model's values) from runtime authority (whether a user can actually stop it). A model can be broadly aligned and still fail once it is acting across tools, long workflows, conflicting instructions, or adversarial inputs. "Stop" and "undo" cannot be decorative UI controls.

**Governing multi-agent coordination.**
When agents coordinate with other agents via protocols like MCP or A2A, current standards support connection but not governance. Voting, dissent, human escalation, and audit/replay are absent. Organizations will need to see which agent is acting, why it has authority, who dissented, and how a decision can be reconstructed later.

---

### Cluster C — Human Judgment & Agency

The long-game problems: whether AI erodes or strengthens human capability over time.

**Preserving human judgment while improving speed.**
Do users become more capable over time, or more dependent? Backed by the MIT misinformation study, the AI persuasion research (AI nearly 3× more effective than professional canvassers), and Davis's interactional drift framework. The signature review question: *"After using this system for a month, is the person more capable, equally capable, or dependent?"*

**Governing proactive AI initiation.**
When is it appropriate for AI to initiate action or attention without being explicitly asked? Proactive AI can feel magical when right and invasive when wrong. Designing timing, appropriateness, consent, and silence as its own design discipline is under-owned. The concept of proactive AI is well-covered in product writing; the design governance of when and how AI initiates is not.

**Detecting and designing against interactional drift.**
Participatory imbalance, temporal drift, conceptual divergence, interactional rigidity — these failure modes emerge through the interaction itself, not through any single output. A chatbot can appear successful in single turns while training the user into passivity over weeks. Evaluation and design need to track trajectories, not just outputs. Drift patterns to watch: passivity, over-reliance, conceptual divergence from the user's actual goal, repetitive loops, and failed repair.

---

### Cluster D — Evidence & Transparency

What people actually need in order to trust, challenge, or act on AI output.

**Turning transparency into usable evidence.**
What evidence does a user, admin, reviewer, or customer actually need to trust, challenge, or approve an AI output or action? Not chain-of-thought — usable claim-level provenance, uncertainty display, source quality, and action basis. This appears across health, science, enterprise agents, release governance, and AI Overviews liability. The need for graduated transparency: lightweight status by default, deeper reasoning when risk rises or the user asks.

**Validating AI-mediated UX evaluation.**
Avenir-UX, PerceptUI, and UXBench show AI entering UX evaluation itself. Simulated users can accelerate early critique and variant screening, but they don't carry real stakes, habits, or organizational consequences. Teams need evidence standards: what synthetic findings are directional-only, when human research is mandatory, and who is accountable when a simulation drives a product decision.

---

### Cluster E — Consequential Action & Safety

Where AI takes actions with real-world stakes.

**Governing safe agentic commerce and consequential transactions.**
Shopping agents collapse discovery, recommendation, carting, and payment into a single conversational loop. Personalization can silently become a purchasing mandate. Design needs scoped mandates, spending caps, approval thresholds, verifiable identity, audit trails, and dispute paths — with clear separation between recommendation authority and purchase authority.

**Safety testing also needs governance.**
Meta's Project Cannes illustrates the problem: even the process of evaluating AI safety can become ethically messy without defined consent boundaries, worker protections, red-team authorization, and clear separation between public-interest safety evaluation and competitive intelligence.

---

### ★ Top 3 — AI Solutions List

Rankings based on two criteria: (1) foundational impact — solving these enables solving others; (2) writing differentiation — others are not writing about these.

#### 1. Detecting and designing against interactional drift *(Cluster C)*

**Why it's foundational.** Drift is the long-run outcome of every other failure in this list. Weak delegation produces drift. Poor oversight produces drift. Missing judgment-preservation produces drift. It is the canary for system health — what the interaction looks like after weeks of use, not after a single turn.

**Why it's open to write about.** The concept of interactional drift was introduced in Davis's May 2026 arXiv paper and has had zero translation into practitioner writing. The term does not appear in Medium, Substack, or LinkedIn design circles. No one is writing about how to instrument for it, design against it, or make it legible to enterprise product teams. This is the most open territory on the AI list.

#### 2. Designing the AI authority model *(Cluster A)*

**Why it's foundational.** It is the literal precondition for everything else. You cannot design delegation without authority, oversight without knowing what the AI can do, or transparency without a model of what the AI can access. Every other problem in Cluster A and B branches from this one.

**Why it's open to write about.** Surface-level coverage exists: Smashing Magazine's agentic UX patterns piece, Medium's trustworthy-agent lists. But none of it synthesizes a coherent design leadership framework around the authority layer. The specific framing — "what I can see / what I can remember / what I can do" as a designed, user-facing, revocable layer — is not being written about as a distinct design problem.

#### 3. Governing proactive AI initiation *(Cluster C)*

**Why it's foundational.** Proactive AI is the moment when all authority, delegation, and oversight problems converge at once. When the system acts without being asked, every gap in the design becomes immediately visible. It is also the frontier where all the major platforms are competing — Apple Intelligence, Google's CC agent, Microsoft Copilot proactivity — which means design leaders need vocabulary for it now.

**Why it's open to write about.** "Proactive AI" is being covered extensively as a product trend. What is not being covered is the design discipline of governing when and how AI initiates — timing, appropriateness, consent, silence, the ladder from observe → suggest → prepare → act. That governance framing is open.

---

## Part 2 — Organizational Dynamics: Design Leadership Problems

Problems about how organizations build, adopt, govern, and sustain AI work — and how design leaders operate inside those systems.

---

### Cluster A — Governance Architecture

How organizations establish authority, monitor AI in production, and make governance feel like work rather than compliance.

**Who has release authority, and on what evidence?**
Model release decisions require credible evidence, clear decision rights, emergency mechanisms, customer continuity handling, and dispute resolution among government, labs, customers, employees, and the public. The Anthropic Fable/Mythos suspension makes this concrete. Release authority is now board, security, policy, customer, and public-trust governance — not only a product question. The design problem is making the release-evidence package legible: who needs to understand what, which evidence is decision-grade, and what users are told when access changes suddenly.

**Post-launch governance as experience architecture.**
NIST RMF, ISO 42001, and EU AI Act Article 72 all make post-market monitoring an explicit obligation. The experience is not complete at launch — it includes what happens when the system drifts, harms, oversteps, fails silently, or requires escalation. Agent telemetry, audit trails, incident review loops, drift monitoring, and rollback paths belong inside the experience architecture, not bolted on afterward.

**Turning governance into workflow.**
AI governance fails when it stays abstract. Teams need governance expressed as actual product behavior and operating cadence: approval queues, escalation states, exception handling, permission ladders, human handoff protocols, review checkpoints, and recovery paths. If people cannot use the governance path under real pressure, the system is not governed in practice.

---

### Cluster B — Adoption & Workforce

How organizations and people actually change — not just which tools get deployed.

**Building adoption systems, not rollout campaigns.**
AI value does not appear because tools are available. The Microsoft 2026 Work Trend Index found that culture, manager support, and talent practices account for more than twice the reported AI impact of individual effort. Adoption requires workflow redesign, shared quality standards for AI-assisted work, manager modeling, incentives that reward judgment, and protected human skill. Nearly 48% of organizations have introduced AI without redesigning the workflows or roles it sits within.

**Managing AI sprawl and fragmented adoption.**
Without shared standards, organizations accumulate duplicate outputs, hidden botsitting, and fragmented private workflows. Workers may be ahead of their organizations, but without shared quality bars their gains do not compound. AI sprawl is an organizational design problem, not just a tool-management problem.

**Designing workforce transition pathways.**
Capturing AI value depends on redesigning workflows, roles, skills, culture, and metrics — not just deploying agents. Workforce transition requires designed pathways and role clarity, not vague reskilling language. Preserving human craft requires explicit practice modes, review standards, and protected time away from AI-assisted work.

---

### Cluster C — Trust Infrastructure

The designed conditions that determine whether organizations and customers can actually rely on AI.

**Connecting builder experience to customer trust.**
If internal teams cannot design, govern, test, and explain AI behavior, customers inherit that uncertainty as mistrust. None of the major platforms publicly own this internal-to-external trust chain. The central claim: trust is built upstream, in the builder experience, and felt downstream, in the customer experience. This is the strongest and most defensible territory in the corpus.

**Owning the admin, approver, and auditor experience.**
The person affected by AI is not always the person typing into the chat box. Enterprise AI creates first-class users who are almost never designed for: admins, managers, reviewers, auditors, compliance teams, support staff. Governance interfaces consistently lag behind end-user AI features. This is high-value and chronically under-designed.

**Making trust operational, not a message.**
Only 15% of Americans trust AI companies to make AI decisions. Trust cannot be messaged into existence — it is a designed system of conditions: release evidence, context and permission models, judgment-preserving interactions, monitoring, and adoption systems. The five-layer trust stack is the designable surface: (1) release authority, (2) context and permission, (3) judgment-preserving interaction, (4) post-launch governance, (5) adoption system.

---

### Cluster D — Leadership Capabilities

How design leaders build the organizational conditions for quality — their own authority, team strength, and the systems that connect human understanding to delivered outcomes.

**Maintaining the steel thread through complex organizations.**
Organizations routinely break the thread between human need, strategic intent, product decisions, implementation, delivery, and evidence. Research does not influence strategy. Strategy does not survive prioritization. Design intent does not survive implementation. The leadership work is keeping intent, decisions, delivery, and learning connected — systems thinking made operational.

**UX owning the evidence layer across the organization.**
UX should own the synthesis that integrates behavioral, attitudinal, experiential, business, system, longitudinal, and equity evidence — not to claim exclusive ownership of customer knowledge, but to be the discipline that integrates it. Conversion, engagement, and satisfaction can conceal declining trust, manipulation, accessibility failures, or long-term harm.

**Building adaptable teams without losing specialist depth.**
The goal is breadth that allows following the steel thread combined with enough depth to make an expert contribution — not shallow generalism. There is no universal ideal team structure; the leadership question is what configuration of people, authority, and expertise will create the most value for this specific system, given its risks, dependencies, maturity, and business model.

**Trust as the mechanism for UX influence.**
Evidence does not automatically produce influence; expertise does not automatically produce authority. UX leaders gain practical decision-making authority through relationships built on the integrity of their evidence, their ability to separate facts from assumptions, and their commitment to shared outcomes over functional territory.

**Psychological safety as a product quality system.**
Teams must be able to expose uncertainty, disclose mistakes, request help, challenge weak assumptions, and show unfinished work. This is not a culture nicety — it is the mechanism through which quality problems surface before they reach production. Edmondson and Seth noted in HBR in 2026 that AI erodes team trust when the gap between warranted and actual trust in AI becomes undiscussable.

---

### ★ Top 3 — Organizational Dynamics List

Rankings based on two criteria: (1) foundational impact — solving these enables solving others; (2) writing differentiation — others are not writing about these.

#### 1. Owning the admin, approver, and auditor experience *(Cluster C)*

**Why it's foundational.** If the people responsible for governance don't have well-designed experiences, governance fails regardless of how good the end-user product is. This is where AI goes wrong at organizational scale — not in the chatbox, but in the invisible approval queue that nobody designed. The entire governance architecture depends on whether these users can actually function.

**Why it's open to write about.** Governance writing exists from IT, legal, and compliance angles. HR writing exists on team AI adoption. But there is essentially no design leadership writing that treats admins, auditors, and approvers as first-class users whose experience determines whether AI governance functions at all. The angle is wide open and directly adjacent to the dominant enterprise AI conversation.

#### 2. Connecting builder experience to customer trust *(Cluster C)*

**Why it's foundational.** It is the bridge between every AI-specific problem and every organizational problem. Internal design, governance, eval, and monitoring quality is what customers eventually feel. Without this frame, organizations address the user interface and the compliance layer as separate concerns and miss the causal connection between them.

**Why it's open to write about.** "AI trust" is written about everywhere. What is not being written is the specific claim that the builder's experience — the design, governance, eval, and monitoring conditions inside the team — determines what customers inherit. MIT Technology Review, CMSwire, and NN/g are all circling "trust as the benchmark," but none of them own the upstream-to-downstream chain as a design leadership frame. This is the most distinctive organizational territory in the corpus.

#### 3. Psychological safety as a product quality system *(Cluster D)*

**Why it's foundational.** If teams cannot expose uncertainty, disclose mistakes, or challenge momentum, quality problems become invisible until they are in production. AI amplifies this: confident-looking outputs from AI tools can suppress the human signals that would otherwise surface a bad decision before it ships.

**Why it's open to write about.** Forbes, MIT Technology Review, and HR publications are writing about psychological safety in AI-enabled teams from a leadership and culture angle. What is not being written is the more specific argument that psychological safety *is* the product quality mechanism — not a cultural attribute that sits alongside quality, but the organizational system that makes quality visible and correctable before it ships. That reframe is not being made in design circles.

---

## Research note on writing differentiation

The topics with the clearest writing opportunity share a common characteristic: they address the *interior* of the AI experience rather than its surface. The practitioner AI design discourse in 2025–2026 is heavily focused on end-user interface work — transparency patterns, agentic UX, trust signals in the product. What is almost entirely absent is writing about the humans and systems *behind* the product: the people who approve, audit, and recover; the teams whose internal conditions determine what customers receive; and the long-run trajectory of human capability under AI use. That is where the open territory is.
