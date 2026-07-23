---
title: Osprey Synthesis — Update, July 22, 2026
date: 2026-07-22
tags:
  - osprey
  - synthesis
  - territory
  - print
supersedes: "[[2026-06-30-osprey-synthesis-print]]"
---

# OSPREY SYNTHESIS — UPDATE

**Trends, Paradigms, Design Leadership Problems, and Territory Sharpening**
Updated July 22, 2026. Supersedes [[2026-06-30-osprey-synthesis-print]].

Source notes reviewed since June 30:

- 2026-07-01 Codex usage and action-level AI governance
- 2026-07-02 Controllability, agent governance, and Project Cannes
- 2026-07-14 Magentic-UI, Avenir-UX, and AI design leadership problems
- 2026-07-17 UX leadership — coherence, evidence, adaptability, craft, and trust
- 2026-07-17 Design leadership problems — organized and ranked
- 2026-07-20 Agent permissions, learning debt, and agentic governance

What changed and why is marked **[Updated]** or **[New]** throughout. The June 30 foundation holds. The updates deepen two areas in particular: the behavioral specificity of agent governance, and the capability-atrophy problem.

---

## PART 1 — KEY EMERGENT TRENDS

### Trend 1. From answer engine to delegated actor **[Updated]**

The unit of UX is no longer a single response. It is a delegated work loop: goal, scope, plan, execute, monitor, interrupt, review, recover.

Visible in: Codex-style long-running work, computer-use agents, agentic commerce, Copilot Studio, Agentforce, Rovo, Replit, OpenAI Agents SDK.

**Now with empirical backbone.** The June 25, 2026 Codex usage paper provides the strongest quantitative evidence in the corpus that this shift is real and accelerating, not speculative:

- Active Codex usage grew more than fivefold between January 1 and June 1, 2026.
- The share of individual users submitting tasks estimated to take an experienced human eight or more hours rose from 2.1% in December 2025 to 25.6% by May 2026.
- More than 10% of users manage three or more concurrent agents weekly; within OpenAI, 28.6% managed five or more in a single week.
- Skills — reusable workflow infrastructure — rose from 5.4% to 26.6% of active users across the same window.

The design read is not just growth. It is a structural shift: humans are becoming scopers, assigners, supervisors, reviewers, and integrators. The agent does the production run. That changes what the interface needs to do.

### Trend 2. Context as the new primitive — and the new invisible authority

Apple on-screen awareness, Microsoft work context, Google adaptive cues, Meta social and personal context, enterprise role and permission context.

Local inference does not settle the privacy or authority question. Users increasingly need a legible "what I can see, remember, and do" layer.

### Trend 3. HCI is becoming human-agent supervision **[Updated]**

The human role is shifting from operator to goal-setter, supervisor, reviewer, approver, exception handler, and accountable decision maker.

This is the deepest paradigm shift in the corpus.

**The user is also moving from selector to auditor.** A May 2026 paper measuring Google AI Overviews found AI-generated summaries appeared for 64.7% of question-form queries, and 11.0% of atomic claims were unsupported by cited pages. Users increasingly receive a synthesized answer before choosing sources. Agents increasingly complete work before users inspect it. The result: provenance, contestability, interruption, and review states are becoming primary interface components, not secondary ones. Oversight is no longer just about watching the agent — it is about auditing what it already did.

### Trend 4. Trust as operating architecture, not messaging **[Updated]**

Release authority, evidence packages, post-market monitoring, audit trails, incident response, escalation, reversibility.

Anthropic Public Record (15% trust), EU AI Act, NIST RMF, ISO 42001, and RSP updates all push the same direction: trust is a designed system of conditions, not a tone.

**Frontier model releases are becoming governed access events, not normal product launches.** OpenAI staggered GPT-5.6 access after a U.S. government request, starting with a small trusted-partner preview. U.S. export controls on Anthropic's Fable 5 and Mythos 5 were lifted only after strengthened cyber safeguards and closer government collaboration. The operating question is no longer "who has the strongest model?" It is "who controls release authority, customer access, fallback continuity, and safety evidence when model capabilities cross national-security thresholds?" Release authority is now board, security, policy, customer, and public-trust governance — not only a product decision.

### Trend 5. Judgment erosion as a first-order design risk **[Updated]**

Paired evidence on overreliance (MIT misinformation study) and AI persuasion (AI out-persuading expert humans, roughly three times more effective than professional canvassers).

Interactional drift — passivity, conceptual divergence, dependency — emerges through the interaction itself, not through any single model output.

**Knowledge Debt is now a named mechanism for the same erosion.** The July 7, 2026 paper *Agents That Teach* introduces an analogy to technical debt: when AI agents complete tasks that humans used to learn through, the output advances while the human's comprehension lags. A codebase improves while the developer no longer understands the change, the alternatives, or the underlying concept. This generalizes to any AI-assisted domain — analysis, writing, decision preparation, synthesis. The organization may gain short-term throughput while losing human judgment, resilience, and learning capacity.

Knowledge Debt is a more concrete and practitioner-legible name for the same dynamic the June 30 synthesis tracked as interactional drift. Both are now in play as a pair: drift describes the trajectory of the interaction; Knowledge Debt names the capability cost.

### Three secondary trends **[Updated — one added]**

- Proactive AI is becoming its own discipline. Timing, appropriateness, and consent for unsolicited action, not just unsolicited information.
- Evaluation is moving into real workflows. Deployment simulation, post-market monitoring, PerceptUI, UXBench. Synthetic UX evaluation is useful but dangerous if over-trusted.
- **[New] AI personality is a safety-critical design variable, not brand tone.** A May 2026 review argues that affective cues in agents shape trust calibration, delegation, repair, dependence, and governance. Oxford/Nature research found that warmer chatbot tuning produced more mistakes and more validation of false beliefs, especially when users expressed vulnerability. AI warmth is a control layer that can preserve human judgment or erode it. This is a design responsibility, not a brand decision.

---

## PART 2 — PARADIGMS BEING EXPLORED

### Interaction and product paradigms **[Updated]**

- **Coordination zones.** Done-for-me, done-under-me, done-with-me, done-without-me. Replaces "human-in-the-loop" as a slogan.
- **Progressive or earned autonomy.** Replaces the binary autonomy switch.
- **Responsive salience.** AI presence rises and falls with risk, stakes, expertise, and uncertainty. Replaces static UI prominence.
- **Co-planning and co-tasking.** [New] The agent exposes an editable plan before acting; the human and agent can pass control back and forth during execution. Magentic-UI names six concrete mechanisms: co-planning, co-tasking, action approval, answer verification, memory, and multi-tasking. This is more specific than workplan gating — it defines the designed handoff points, not just the fact of pausing.
- **Workplan gating.** Designed pause, ask, approve, escalate points. Replaces one-shot approvals.
- **Action-level graduated authority.** [New] Read, write, send, delete, deploy, pay, publish, and decide are different authority levels requiring different controls. Low-risk reversible actions proceed with logging. Medium-risk actions get preview or batch approval. High-risk, rights-affecting, financial, health, or external-facing actions require named human authority and audit trails. The design problem is expressing this graduated control as actual user experience, not policy language.
- **Schema-driven interaction.** App Intents, MCP. Replaces free-form prompting.
- **Refinement loops.** Iterative co-shaping. Replaces one-shot generation.
- **Cognitive forcing functions.** Deliberate reflective friction. Replaces frictionless flow as a default goal.
- **Learning-aware agent design.** [New] Incidental learning does not automatically survive delegation. Systems can be designed to build it back in: contextual, grounded, ambient, selective, adaptive, and closed-loop learning moments that surface when there is a meaningful comprehension gap — not as interruptions, but as ambient coaching tied to the work just performed.

### Trust, governance, and evaluation paradigms **[Updated]**

- **Graduated transparency.** Depth of explanation matches task risk and user expertise. Replaces one-size explainability.
- **Interaction-centered evaluation.** Trajectory, drift, repair, participation balance. Replaces model-centric benchmarks.
- **Release-authority evidence packages.** Risk reports, system cards, capability thresholds, escalation pathways. Replaces vague safety claims. Now includes the release decision itself as a governance act.
- **Context manifests and memory controls.** Live, user-facing inventory of access and memory. Replaces implicit context capture.
- **Scoped mandates.** Especially for agentic commerce. Replaces open-ended agent authority.
- **Synthetic user evaluation paired with human validation.** Replaces either-or research methods.
- **Adoption as workflow redesign.** Replaces tool rollout and generic training.
- **Runtime controllability as distinct from model alignment.** [New] A model can be broadly aligned and still fail once it is acting across tools, long workflows, conflicting instructions, or adversarial inputs. Controllability — whether the system can be reliably interrupted, overridden, redirected, and constrained while running — is a separate design requirement. Stop, undo, redirect, and do-not-cross-this-boundary must bind execution, not function as decorative UI controls.
- **Product-level vs. user-level permissions.** [New] Product-level policies are broad defaults set by the system provider. They cannot represent every user's context, risk tolerance, relationship, or task boundary. As agents act across tools, files, email, calendars, databases, and transactions, permission must become part of the user experience — expressive, persistent, inspectable, and enforceable — not only a back-office policy setting.
- **Differentiated governance by agent type.** [New] Applying uniform governance across all AI agents leads to failure (Gartner, May 2026). Governance must vary by autonomy level, tool access, data sensitivity, reversibility, business criticality, and oversight model. A lightweight summarizer does not need the same controls as an autonomous agent with access to customer records and payment systems.
- **Multi-agent governance gaps.** [New] Current interoperability protocols (MCP, A2A, ACP, ANP) support agent connection but not governance. Voting, dissent preservation, human escalation, and audit/replay are absent from all reviewed protocols. Organizations deploying coordinating agent systems will need to see which agent is acting, why it has authority, what evidence it used, who dissented, and how a decision can be reconstructed.

### The unifying structure: a five-layer trust stack

1. Release authority and evidence — who decides what can ship, run, or pause. Now includes the release decision as a governance act.
2. Context and permission model — what the AI can access, infer, remember, and do. Now includes the product-level vs. user-level permissions distinction.
3. Judgment-preserving interaction — how the experience keeps humans capable, skeptical, and responsible. Now includes Knowledge Debt and learning-aware design.
4. Post-launch governance — how teams monitor, learn, correct, roll back, and remain accountable. Now includes differentiated governance and multi-agent coordination.
5. Adoption system — how leaders redesign work, incentives, skills, and culture so trust is earned through evidence.

Almost every paradigm above is a tool for one of these five layers.

---

## PART 3 — DESIGN LEADERSHIP PROBLEMS

Filtered for what the corpus repeatedly returns to, what is under-owned by the major platforms, and what is defensible as Tam-specific territory.

The problems below span two types: **AI solutions problems** — about the craft and architecture of AI experiences — and **organizational dynamics problems** — about how organizations build, adopt, and govern AI work. Both matter for the territory.

### AI Solutions Problems

#### Problem 1. Designing the AI authority model

**The question.** How do people — users, admins, customers, auditors — know what an AI system is allowed to see, infer, remember, decide, and do, and how do they revoke it?

**Why it matters.** This is the single recurring spine across the full corpus. It connects Apple App Intents, EU AI Act Articles 13 and 14, agentic commerce mandates, computer-use agents, and enterprise role and permission context. Current permission dialogs are too blunt for AI behavior. No platform publicly owns this fully. The July notes sharpen it further: the shift is from "prompt UX" to **authority UX** — from screen and prompt design toward access, consent, and revocation as the primary interface concerns.

#### Problem 2. Making delegation legible and bounded

**The question.** How does a human delegate work to AI without losing situational awareness or accountability?

**Why it matters.** Delegation is the new core interaction loop: scopes, plans, checkpoints, approvals, status, review states, handoffs. The 37.8 percentage-point preference lift for high-transparency prototypes is empirical backing. Magentic-UI formalizes this as six concrete interaction mechanisms. The "user as auditor" framing from the AI Overviews data adds urgency: legibility must extend to work the agent already completed, not only work it is about to do.

#### Problem 3. Designing for proportional oversight by risk

**The question.** When should AI act automatically, when should it ask, when should it require approval, and when should it hand off to a human?

**Why it matters.** This operationalizes Problem 2. The July notes add action-level specificity: read, write, send, delete, deploy, pay, publish, and decide are different authority levels, not a single permission dial. Without this graduated design, AI is either unusable (constant approval friction) or unsafe (blanket automation).

#### Problem 4. Preserving human judgment and capability while improving speed

**The question.** Do users become more capable over time, or more dependent?

**Why it matters.** This is now backed by three distinct mechanisms: interactional drift (Davis), AI persuasion (three times more effective than professional canvassers), and Knowledge Debt (Agents That Teach). The differentiated framing: AI productivity must be measured against long-term human capability, not short-term output. The signature review question — *"After using this system for a month, is the person more capable, equally capable, or dependent?"* — should be treated as a published evaluative standard, not only a workshop prompt.

#### Problem 5. Detecting and designing against interactional drift **[Elevated]**

**The question.** How do design and evaluation practices track the trajectory of human-AI interaction over time, not just the quality of individual outputs?

**Why it matters.** Drift failure modes — passivity, over-reliance, conceptual divergence, interactional rigidity, failed repair — emerge through the interaction itself. A chatbot can appear successful in single-turn evals while training the user into passivity over weeks. Knowledge Debt is now a concrete, named version of this: the comprehension gap that accumulates as delegation eliminates the learning that used to happen through effortful work. Evaluation and design need to track trajectories, not just outputs. This is the most open writing territory in the corpus — zero practitioner translation exists.

#### Problem 6. Governing proactive AI initiation **[New]**

**The question.** When is it appropriate for AI to initiate action or attention without being explicitly asked?

**Why it matters.** Proactive AI is the moment when all authority, delegation, and oversight problems converge at once. When the system acts without being asked, every gap in the design becomes immediately visible. The major platforms are competing here — Apple Intelligence, Google's CC agent, Microsoft Copilot proactivity — which means design leaders need vocabulary for timing, appropriateness, consent, and silence as its own discipline. The product trend is well-covered; the design governance of when and how AI initiates is not.

#### Problem 7. Agent controllability during execution **[New]**

**The question.** Can a running agent be reliably interrupted, overridden, redirected, and constrained mid-task?

**Why it matters.** Controllability is distinct from alignment. A model can be broadly aligned and still fail once it is acting across tools, long workflows, conflicting instructions, or adversarial inputs. The May 2026 controllability paper defines the design requirement: a real control plane with visible authority hierarchy, runtime intervention points, persistent safety states, and audit trails. Stop and undo cannot be decorative.

#### Problem 8. Governing multi-agent coordination **[New]**

**The question.** When agents coordinate with other agents, how do people know which agent acted, why it had authority, who dissented, and how the decision can be reconstructed?

**Why it matters.** Current protocols support connection, not governance. Voting, dissent, human escalation, and audit/replay are absent. This is the next-generation governance UX problem: not just governing one agent, but governing the coordination of many.

---

### Organizational Dynamics Problems

#### Problem 9. Connecting builder experience to customer trust

**The question.** How do internal design, governance, eval, and monitoring practices show up in the customer experience?

**Why it matters.** This is the strongest Tam-specific problem. If builders cannot design, govern, test, and explain AI behavior, customers inherit that uncertainty as mistrust. None of Apple, Google, Meta, or Microsoft public guidance fully owns the internal-to-external trust chain. The clearest defensible claim: trust is built upstream, in the builder experience, and felt downstream, in the customer experience.

#### Problem 10. Owning the admin, approver, and auditor experience **[New]**

**The question.** Who is designing the experience for the people responsible for making AI governance function?

**Why it matters.** Enterprise AI creates first-class users who are almost never designed for: admins, managers, reviewers, auditors, compliance teams, support staff. If these people cannot function under real pressure, governance fails regardless of how good the end-user product is. The governance interfaces consistently lag behind end-user AI features. This is high-value and chronically under-designed. There is essentially no design leadership writing that treats these users as primary.

#### Problem 11. Psychological safety as a product quality system **[New]**

**The question.** How do team conditions determine whether quality problems surface before they reach production?

**Why it matters.** If teams cannot expose uncertainty, disclose mistakes, or challenge momentum, quality problems become invisible until they ship. AI amplifies this: confident-looking AI output can suppress the human signals that would otherwise flag a bad decision before it reaches customers. Edmondson and Seth (HBR, 2026) noted that AI erodes team trust when the gap between warranted and actual trust in AI becomes undiscussable. Psychological safety is not a culture attribute that sits alongside quality — it is the organizational mechanism that makes quality visible and correctable.

---

## PART 4 — SHARPENING THE CLAIMS AND TERRITORY

### Current operating claim

> I design the trust layer that turns AI capability into human adoption and organizational value.

Still the right altitude. The July notes give it stronger legs in two directions.

### Five original sharpening moves — still valid

A. Replace "trust layer" with operational language at least half the time.
B. Name the boundary more aggressively.
C. Add the builder-to-customer chain as the unique defensible claim.
D. Stake judgment-preservation as a measurable territory.
E. Pick a vocabulary and commit.

### Two new sharpening moves **[New]**

**F. Add "authority UX" as a named vocabulary shift.**

The July notes make a paradigm-level naming move: the shift is from **prompt UX** — screen and prompt design — toward **authority UX** — access, consent, scope, and revocation as primary interface concerns. This is a useful vocabulary move for external positioning, workshops, and product reviews. It lands well alongside delegation and judgment in the primary spine.

**G. Sharpen the long-game framing with the atrophy test.**

The July 20 note proposes a line worth promoting to primary positioning:

> AI design leadership is becoming the discipline of making delegated work governable without making it unusable, and making automation productive without letting human judgment atrophy.

This is more bilateral than the existing sharpened statement. It names both failure modes — the governance failure and the capability-atrophy failure — in a single sentence. Consider whether it strengthens or replaces the existing territory statement, or whether it becomes the sharpest version of the long-game test.

### Sharpened territory statement — updated

> I design the authority, delegation, and judgment systems that determine whether AI capability becomes durable human and organizational value. My work sits where builder experience meets customer trust — the seam most platforms publish around but do not own.

This holds. The July notes add specificity to "authority" (authority UX, action-level governance, runtime controllability) and to "judgment" (Knowledge Debt, drift, the atrophy test). The territory statement does not need to change, but the operational frames behind it are now richer.

### Updated primary vocabulary spine

**Delegation. Authority. Judgment.** — still the recommended spine.

Supporting terms added by the July notes: **authority UX**, **Knowledge Debt**, **interactional drift**, **action-level governance**, **runtime controllability**, **builder-to-customer chain**.

### Signature review question — promote to primary evaluative standard

> After using this system for a month, is the person more capable, equally capable, or dependent?

This should move from a workshop prompt to a published heuristic — the kind of thing others adopt and credit. The July notes give it additional empirical backing through Knowledge Debt (the capability-loss mechanism) and drift (the interaction trajectory that leads there).

---

## PART 5 — WHAT TO WRITE NEXT

The July notes add three strong new writing opportunities to the original four.

### Original four — still valid, with updated framing

1. **A short piece on the delegation loop.** Use Coordination Zones as scaffold, with the builder-to-customer extension. Magentic-UI's six mechanisms provide concrete structure.

2. **A design-review heuristic kit.** Proportional oversight by risk, with the "more capable, equally capable, or dependent?" question as the centerpiece. Now add Knowledge Debt as the mechanism the heuristic is designed to prevent.

3. **A piece on context as invisible authority.** Use the EU AI Act, Apple App Intents, and "Local Is Not a Sufficient Privacy Boundary" as the evidence base. Now add the product-level vs. user-level permissions distinction.

4. **A piece naming "interactional drift" for an enterprise audience.** Translate Davis into product-review language. Still the most open territory. Now pair with Knowledge Debt — drift is the trajectory, Knowledge Debt is the named cost.

### Three new writing opportunities **[New]**

5. **Knowledge Debt as the hidden cost of AI productivity.**
Why teams may ship faster while understanding less — and how learning-aware systems can protect long-term capability. The concept was introduced in a July 7, 2026 arXiv paper and has had zero practitioner translation. It lands in every domain where people delegate reasoning, synthesis, troubleshooting, or decision preparation. This is the strongest new writing opportunity: high differentiation, no current competition, and direct extension of the judgment-preservation territory.

6. **The new UX is permission architecture.**
Why agentic AI shifts design from screens and prompts to authority, access, consent, and revocation. The distinction between product-level policies and user-level permissions gives this a concrete analytical spine. The "authority UX" framing is new vocabulary that could anchor a widely-shared piece. Nobody in practitioner design writing is owning this framing yet.

7. **The admin, approver, and auditor are your most important AI users.**
Why AI governance fails at organizational scale when the people responsible for it don't have well-designed experiences. Governance interfaces consistently lag behind end-user AI features. This is directly adjacent to the dominant enterprise AI conversation and entirely open as a design leadership claim.

---

## ONE-PAGE SUMMARY — UPDATED

**Trends.** Delegated actor (empirically confirmed, 5× usage growth). Context as invisible authority. HCI becoming supervision — and auditing. Trust as architecture — including the release decision itself. Judgment erosion: interactional drift and Knowledge Debt. AI personality as safety variable.

**Paradigms.** Coordination zones. Progressive autonomy. Responsive salience. Co-planning and co-tasking. Workplan gating. Action-level graduated authority. Schema-driven interaction. Refinement loops. Cognitive forcing functions. Learning-aware agent design. Graduated transparency. Interaction-centered evaluation. Release-evidence packages. Context manifests. Scoped mandates. Synthetic evaluation with human validation. Adoption as workflow redesign. Runtime controllability. Product vs. user-level permissions. Differentiated governance by agent type. Multi-agent governance.

**Five-layer trust stack.** Release authority (now including release as governance act). Context and permission (now including user-level permissions). Judgment-preserving interaction (now including Knowledge Debt and learning-aware design). Post-launch governance (now including differentiated governance and multi-agent coordination). Adoption system.

**Design leadership problems — AI solutions.**

1. Designing the AI authority model.
2. Making delegation legible and bounded.
3. Designing for proportional oversight by risk.
4. Preserving human judgment and capability while improving speed.
5. Detecting and designing against interactional drift. *(Elevated — top open writing territory)*
6. Governing proactive AI initiation. *(New)*
7. Agent controllability during execution. *(New)*
8. Governing multi-agent coordination. *(New)*

**Design leadership problems — organizational dynamics.**

9. Connecting builder experience to customer trust.
10. Owning the admin, approver, and auditor experience. *(New)*
11. Psychological safety as a product quality system. *(New)*

**Sharpened territory statement.**

> I design the authority, delegation, and judgment systems that determine whether AI capability becomes durable human and organizational value. My work sits where builder experience meets customer trust — the seam most platforms publish around but do not own.

**Long-game framing added.**

> AI design leadership is becoming the discipline of making delegated work governable without making it unusable, and making automation productive without letting human judgment atrophy.

**Primary vocabulary spine.** Delegation. Authority. Judgment.
**Supporting terms added.** Authority UX. Knowledge Debt. Interactional drift. Action-level governance. Runtime controllability. Builder-to-customer chain.

**Signature review question.** After using this system for a month, is the person more capable, equally capable, or dependent?

**What to write — full list.**

1. The delegation loop (Coordination Zones + Magentic-UI mechanisms + builder-to-customer extension).
2. The design-review heuristic kit (proportional oversight + Knowledge Debt as the mechanism to prevent).
3. Context as invisible authority (EU AI Act + App Intents + user-level permissions).
4. Interactional drift for enterprise (Davis + Knowledge Debt as paired concepts).
5. Knowledge Debt as the hidden cost of AI productivity. *(New — strongest differentiation)*
6. The new UX is permission architecture. *(New — "authority UX" as named frame)*
7. The admin, approver, and auditor are your most important AI users. *(New — open territory)*
