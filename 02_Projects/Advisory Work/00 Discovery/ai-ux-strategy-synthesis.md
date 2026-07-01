# AI UX Strategy Synthesis

## Part 1 — Key Emergent Trends

Five trends recur across every note, in increasing order of strategic stakes.

### Trend 1. From answer engine to delegated actor

The unit of UX is no longer a single response. It is a delegated work loop: goal, scope, plan, execute, monitor, interrupt, review, recover.

Visible in: Codex-style long-running work, computer-use agents, agentic commerce, Copilot Studio, Agentforce, Rovo, Replit, OpenAI Agents SDK.

### Trend 2. Context as the new primitive — and the new invisible authority

Apple on-screen awareness, Microsoft work context, Google adaptive cues, Meta social and personal context, enterprise role and permission context.

Local inference does not settle the privacy or authority question. Users increasingly need a legible "what I can see, remember, and do" layer.

### Trend 3. HCI is becoming human-agent supervision

The human role is shifting from operator to goal-setter, supervisor, reviewer, approver, exception handler, and accountable decision maker.

This is the deepest paradigm shift in the corpus.

### Trend 4. Trust as operating architecture, not messaging

Release authority, evidence packages, post-market monitoring, audit trails, incident response, escalation, reversibility.

Anthropic Public Record (15% trust), EU AI Act, NIST RMF, ISO 42001, and RSP updates all push the same direction: trust is a designed system of conditions, not a tone.

### Trend 5. Judgment erosion as a first-order design risk

Paired evidence on overreliance (MIT misinformation study) and AI persuasion (AI out-persuading expert humans, roughly three times more effective than professional canvassers).

Interactional drift — passivity, conceptual divergence, dependency — emerges through the interaction itself, not through any single model output.

### Two secondary trends

- Proactive AI is becoming its own discipline. Timing, appropriateness, and consent for unsolicited action, not just unsolicited information.
- Evaluation is moving into real workflows. Deployment simulation, post-market monitoring, PerceptUI, UXBench. Synthetic UX evaluation is useful but dangerous if over-trusted.

---

## Part 2 — Paradigms Being Explored

The corpus surfaces a coherent set of conceptual moves the field is making to address those trends.

### Interaction and product paradigms

- **Coordination zones.** Done-for-me, done-under-me, done-with-me, done-without-me. Replaces "human-in-the-loop" as a slogan.
- **Progressive or earned autonomy.** Replaces the binary autonomy switch.
- **Responsive salience.** AI presence rises and falls with risk, stakes, expertise, and uncertainty. Replaces static UI prominence.
- **Workplan gating.** Designed pause, ask, approve, escalate points. Replaces one-shot approvals.
- **Schema-driven interaction.** App Intents, MCP. Replaces free-form prompting.
- **Refinement loops.** Iterative co-shaping. Replaces one-shot generation.
- **Cognitive forcing functions.** Deliberate reflective friction. Replaces frictionless flow as a default goal.

### Trust, governance, and evaluation paradigms

- **Graduated transparency.** Depth of explanation matches task risk and user expertise. Replaces one-size explainability.
- **Interaction-centered evaluation.** Trajectory, drift, repair, participation balance. Replaces model-centric benchmarks.
- **Release-authority evidence packages.** Risk reports, system cards, capability thresholds, escalation pathways. Replaces vague safety claims.
- **Context manifests and memory controls.** Live, user-facing inventory of access and memory. Replaces implicit context capture.
- **Scoped mandates.** Especially for agentic commerce. Replaces open-ended agent authority.
- **Synthetic user evaluation paired with human validation.** Replaces either-or research methods.
- **Adoption as workflow redesign.** Replaces tool rollout and generic training.

### The unifying structure: a five-layer trust stack

1. **Release authority and evidence** — who decides what can ship, run, or pause.
2. **Context and permission model** — what the AI can access, infer, remember, and do.
3. **Judgment-preserving interaction** — how the experience keeps humans capable, skeptical, and responsible.
4. **Post-launch governance** — how teams monitor, learn, correct, roll back, and remain accountable.
5. **Adoption system** — how leaders redesign work, incentives, skills, and culture so trust is earned through evidence.

Almost every paradigm above is a tool for one of these five layers.

---

## Part 3 — Top Design Leadership Problems

Filtered for what the corpus repeatedly returns to, what is under-owned by the major platforms, and what is defensible as Tam-specific territory.

### Problem 1. Designing the AI authority model

**The question.** How do people — users, admins, customers, auditors — know what an AI system is allowed to see, infer, remember, decide, and do, and how do they revoke it?

**Why it matters.** This is the single recurring spine across the corpus. It connects Apple App Intents and View Annotations, EU AI Act Articles 13 and 14, agentic commerce mandates, computer-use agents, and enterprise role and permission context. Current permission dialogs are too blunt for AI behavior. No platform publicly owns this fully.

### Problem 2. Making delegation legible and bounded

**The question.** How does a human delegate work to AI without losing situational awareness or accountability?

**Why it matters.** This is where Coordination Zones and the business-context UX paper meet. Delegation is the new core interaction loop: scopes, plans, checkpoints, approvals, status, review states, handoffs. The 37.8 percentage-point preference lift for high-transparency prototypes is empirical backing. Microsoft is closest publicly, but still implementation-bound.

### Problem 3. Designing for proportional oversight by risk

**The question.** When should AI act automatically, when should it ask, when should it require approval, and when should it hand off to a human?

**Why it matters.** This is the operational answer to Problem 2. It turns governance into product behavior: graduated control by risk, reversibility, user expertise, and stakes. It operationalizes progressive autonomy and responsive salience as concrete design levers. Without it, AI is either unusable or unsafe.

### Problem 4. Preserving human judgment while improving speed

**The question.** Do users become more capable over time, or more dependent?

**Why it matters.** Backed by the MIT misinformation study, the persuasion paper, the cognitive-forcing-functions paper, and Davis's interactional drift framework. The differentiated framing: AI productivity must be measured against long-term human capability, not short-term output. This is the lane platforms are least likely to own — it cuts against their engagement incentives — which is exactly why it is a strong leadership claim.

### Problem 5. Connecting builder experience to customer trust

**The question.** How do internal design, governance, eval, and monitoring practices show up in the customer experience?

**Why it matters.** This is the strongest Tam-specific problem. If builders cannot design, govern, test, and explain AI behavior, customers inherit that uncertainty as mistrust. None of Apple, Google, Meta, or Microsoft public guidance fully owns the internal-to-external trust chain. This is where the territory has the cleanest moat.

---

## Part 4 — What to Write Next

The corpus has been telling you what to publish.

1. A short piece on the delegation loop. Use Coordination Zones as scaffold, with the builder-to-customer extension.
2. A design-review heuristic kit. Proportional oversight by risk, with the "more capable, equally capable, or dependent" question as the centerpiece.
3. A piece on context as invisible authority. Use the EU AI Act, Apple App Intents, and "Local Is Not a Sufficient Privacy Boundary" as the evidence base.
4. A piece naming "interactional drift" for an enterprise audience. Translate Davis into product-review language. Almost nobody is doing this yet.

Items 1, 3, and 4 are the most defensible because the corpus shows nobody else is owning that exact framing publicly.

---

## One-Page Summary

**Trends.** Delegated actor. Context as invisible authority. HCI becoming supervision. Trust as architecture. Judgment erosion.

**Paradigms.** Coordination zones. Progressive autonomy. Responsive salience. Workplan gating. Schema-driven interaction. Graduated transparency. Interaction-centered evaluation. Release-evidence packages. Context manifests. Scoped mandates. Adoption as workflow redesign.

**Five-layer trust stack.** Release authority. Context and permission. Judgment-preserving interaction. Post-launch governance. Adoption system.

**Top five design leadership problems.**

1. Designing the AI authority model.
2. Making delegation legible and bounded.
3. Designing for proportional oversight by risk.
4. Preserving human judgment while improving speed.
5. Connecting builder experience to customer trust.

**Primary vocabulary spine.** Delegation. Authority. Judgment.

**Signature review question.** After using this system for a month, is the person more capable, equally capable, or dependent?

### Segments to serve

B2B is the standout gap — and it's often invisible to the company itself. Most B2B organizations believe they're doing UX right while stuck at lower maturity levels, confusing having UX with being mature in UX. The structural cause is a buyer/user mismatch: the user, customer, and buyer aren't the same person; enterprise deals close on features and integrations, not flow and delight, which lets usability debt accumulate silently until the renewal conversation. The symptom of this trap is that talented design teams end up buried inside a product org with no research budget, no seat at the roadmap table, and no shared language with sales, customer success, or executives.

The sectors that consistently sit at the bottom of the UX maturity curve share three traits: legacy operating models, regulation that rewards compliance over experience, and a buyer who isn't the user.

#### Specific laggard industries

**Insurance** — The clearest case: an industry managing trillions in risk on systems that often feel stuck in the '90s. ~74% of insurers name technology adoption as their top strategic priority, yet most policies are still completed over the phone rather than in-app. A textbook "we have digital, but it doesn't work" gap.

**Finance / banking and healthcare** — The canonical stage-3 plateau (on the NN/G six-stage model). Large enterprises hover here, where UX work happens but inconsistently, or is consistent but has no measurable impact and people don't see its value.

**Below stage 3 (genuinely low maturity)** — Mostly companies outside technology and software, in industries where UX is unknown or rarely practiced:

- Manufacturing / industrial
- Logistics and freight
- Utilities / energy
- Construction
- Agriculture
- Government / public sector
- Legal
- Field services

#### Priority targets

Insurance (carriers and insurtech), healthcare payers, financial services, and B2B industrial SaaS — because they combine four monetizable conditions:

1. Real money at stake
2. Regulatory accountability that *forces* explainability
3. Deep legacy UX debt
4. Live AI initiatives that are stalling on adoption

Their structural inability to hire senior design talent full-time — no design DNA, no roadmap seat for design — is precisely what makes a fractional/advisory engagement land.

#### Where not to play

Consumer tech and design-mature software, where you'd be selling premium help for capabilities they already have in-house.

### The positioning line

You're not advising them on *how their AI looks* — you're advising them on *whether anyone will trust it enough to use it*, and how to prove that with evaluation.

That reframes design from cost center to adoption insurance, which is the only framing that sells into a low-maturity org.

### Ideas

1. A user context / profile app that follows the user across all tools, companies, etc.; open-brain like concept

### Theses I've explored
