---
title: AI Coordination Zones and Interaction-Centered Intelligence
date: 2026-06-29
tags:
  - osprey
  - ai
  - ai-experience
  - design-leadership
  - hci
---

# AI Coordination Zones and Interaction-Centered Intelligence

Created June 29, 2026 as a follow-up to items 4 and 5 in the Osprey AI Overnight Brief.

## Executive Read

The two papers point in the same direction from different levels of abstraction.

The Human-AI Coordination Zones paper gives design teams a practical vocabulary for deciding how a user and an AI system should coordinate in a product experience. It is useful because it sits between broad principles like "keep humans in control" and narrow UI patterns like "show a confidence score."

The Interaction-Centered Intelligence paper gives HCI and AI leaders a broader paradigm: evaluate human-AI systems by the quality of the interaction over time, not only by the final output. It is useful because agentic and co-creative AI systems can succeed or fail through pacing, repair, drift, dependency, handoff quality, and participation balance.

Together, they support Tammy's strongest current territory: designing the trust layer around AI-mediated action.

## Item 4: Human-AI Coordination Zones

Source: James Pierce, Vaiva Kalnikaite, Siddharth Gupta, and Brian Granger, "Human-AI Coordination Zones: A Framework for Designing Human-in-the-Loop Experiences with Agentic AI," arXiv, published May 1, 2026. https://arxiv.org/abs/2606.09848

### What The Paper Is Trying To Solve

The paper starts from a practical design gap. AI UX teams have many high-level principles, such as transparency, appropriate trust, and user control. They also have low-level UI patterns, such as chat boxes, loading states, attribution labels, and confidence indicators. What is missing is mid-level design knowledge: a way to reason about what kind of human-AI relationship a product is creating before jumping into components.

The authors frame agentic AI as a coordination problem rather than a simple interaction problem. In conventional software, the user acts and the system responds. In agentic AI, the AI may infer, initiate, adapt, or act while the user is not directly operating it. That means the experience has to mediate an ongoing relationship between the user, interface, agent, and surrounding systems.

### The Three Design Dimensions

The paper defines human-AI coordination through three dimensions:

- Human involvement: what the user can or must do, such as direct, request, approve, pause, override, monitor, correct, or review.
- AI salience: how visible, prominent, proactive, transparent, vocal, or attention-demanding the AI is in the interface.
- AI activity: what the AI is actually doing in the system, whether or not the user can see it.

The important design insight is the possible mismatch between those dimensions. A system can have low salience but high activity: the AI is doing a lot, but the user barely sees it. Or it can have high salience but low meaningful involvement: the user sees lots of AI activity but has little real control. Those mismatches are where trust, consent, and agency problems often hide.

### The Four Coordination Zones

The paper names four zones:

- Done-for-me: the AI completes work with minimal user input. The user is barely in the loop. This can be useful for low-risk automation, but it needs clear scope, permission, review, and rollback when stakes rise.
- Done-under-me: the user appears to be doing the work while AI quietly assists in the background. This is common in recommendations, ranking, autocomplete, prioritization, and invisible personalization. The risk is hidden steering: the user may not realize how strongly the AI shaped the field of options.
- Done-with-me: the user and AI collaborate across several phases. The AI is salient, and the user has meaningful involvement through plans, updates, edits, interruptions, approvals, and extensions. This is the most obvious fit for complex agentic work.
- Done-without-me: the AI acts without user awareness or involvement. The paper treats this as largely outside its design scope, but from a leadership perspective it is the danger zone: covert agency, poor consent, unclear accountability, and weak auditability.

The value of these zones is not taxonomy for its own sake. They let design, product, engineering, legal, and operations teams talk about autonomy as an experience choice. A team can ask: should this moment be done-for-me, done-with-me, done-under-me, or not done at all?

### Input And Initiation Patterns

The paper also separates types of user input:

- Conventional input: normal UI interaction where the system responds predictably.
- Prompted input: the user deliberately asks the AI to act or generate.
- Sparked input: a normal interaction unexpectedly creates a generative or AI-mediated response.
- Inferred input: the system derives intent, preference, or context from user activity.
- Layered input: multiple modes combine, such as a conventional click plus inferred context plus an AI-prepared suggestion.

For initiation, the paper gives a useful ladder:

- Do-this: the user gives detailed instructions.
- Do-that: the user selects from AI-generated options.
- Do-it: the user approves or rejects an AI-prepared plan.
- Already-doing or already-done: the AI acts proactively under prior permission or assumed mandate.

This ladder is a practical way to discuss consent and agency. The more a product moves toward "already-done," the more it needs explicit mandate design, reviewability, interruption, audit trail, and recovery.

### Design Patterns Worth Stealing

The paper gives four patterns that map cleanly to AI experience leadership:

- Responsive salience: increase or decrease how prominent the AI is based on risk, user expertise, confidence, task complexity, emotional state, or system uncertainty. Routine low-risk work can be quieter; high-stakes or ambiguous work should become more visible and controllable.
- Workplan gating: define the points in a workflow where the AI must pause, notify, ask, escalate, or get approval. This is especially useful for long-running agents where the user wants the efficiency of automation without losing control.
- Attribution markers: make AI contributions visible through labels, annotations, provenance, or generated-by indicators. The right level of visibility depends on risk and policy; a subtle marker may be enough for routine summaries, while high-stakes content needs stronger disclosure.
- Progressive autonomy: let AI earn greater independence over time as reliability, user trust, and permission increase. This reframes autonomy as staged and revocable, not binary.

### Why It Matters For Tammy

This paper is useful because it translates "AI trust" into concrete design levers. A design leader can use it to review an AI product and ask:

- What is the AI actually doing?
- How visible is that activity to the user?
- What can the user meaningfully do at each phase?
- Where is the user approving a plan versus merely reacting to an output?
- Where is the AI steering options without being noticed?
- Where does salience need to rise because stakes, ambiguity, or emotional risk are higher?
- Where does the system need a gate, checkpoint, override, or recovery path?

The strongest Tammy-relevant insight: human-in-the-loop is not enough as a phrase. The design question is what kind of loop, at which moment, with what visibility, what authority, what reversibility, and what evidence.

## Item 5: Interaction-Centered Intelligence

Source: Nicholas Davis, "Interaction-Centered Intelligence: Toward an Interaction-Based Theory of Human-AI Co-Creation," arXiv, published May 30, 2026. https://arxiv.org/abs/2606.00807

### What The Paper Is Trying To Solve

The paper argues that AI is still too often evaluated as isolated computation: benchmark score, output quality, prediction accuracy, task completion, or generated artifact quality. That framing misses something important in co-creative and collaborative AI systems: the intelligence may emerge through the interaction itself.

This is a theoretical paper, not a field study. Its usefulness is that it gives language for a shift Tammy has been tracking: the design object is no longer just the model response or final output. It is the evolving relationship among human, AI, interface, task, environment, and social context.

### Core Argument

The paper proposes interaction as the primary unit of analysis for co-creative AI. It argues that intelligence, creativity, and meaning can emerge through:

- Participation.
- Coordination.
- Timing.
- Adaptation.
- Divergence.
- Repair.
- Regulation.
- Sustained trajectories of interaction.

This changes the way teams should evaluate AI systems. Instead of asking only "Was the answer good?" or "Did the task finish?", teams should also ask "Did the interaction preserve agency, sustain coordination, recover from breakdowns, and improve the human-AI relationship over time?"

### Interactional Drift

One of the most useful concepts is interactional drift: the way collaboration quality changes over time. A system may start helpful but gradually become imbalanced, rigid, dominating, confusing, overly divergent, or dependency-forming.

The paper names several drift patterns:

- Participatory imbalance: one participant increasingly dominates while the other becomes passive or disengaged.
- Temporal drift: pacing, responsiveness, or interaction rhythm degrades.
- Conceptual drift: human and AI diverge in goals, meaning, or creative direction.
- Interactional rigidity: the collaboration becomes repetitive or insufficiently adaptive.
- Excessive divergence: exploration becomes so unstable that shared coordination breaks down.

This is highly relevant to real AI products. A chatbot can appear successful in a single turn while slowly training the user into passivity. A design copilot can produce strong artifacts while weakening the designer's own judgment. A research agent can complete a report while drifting away from the user's real question. A customer-service bot can reduce handle time while degrading the emotional handoff.

### Evaluation Shift

The paper contrasts traditional AI evaluation with interaction-centered evaluation. The practical shift is:

- From accuracy to coordination quality.
- From task completion to participation balance.
- From output quality to trajectory quality.
- From benchmark score to coherence maintenance.
- From user satisfaction to adaptive co-regulation.
- From model explainability to interaction explainability.
- From static outcomes to temporal evolution.
- From single-agent performance to human-AI system performance.

This is a strong design-leadership move because it makes evaluation less model-centric and more experience-centric. It also gives research and product teams a reason to instrument agentic workflows differently: not just success/failure, but interruption, repair, escalation, user correction, reliance, confidence, pacing, and abandonment.

### Ethical And Governance Implications

The paper argues that if intelligence emerges through interaction, then ethical evaluation cannot stop at model behavior. Teams need to ask how participation, coordination, influence, and authority are distributed across the human-AI system.

That matters for design leadership because harms can emerge in the interaction even when each individual output looks acceptable. Examples:

- Over-reliance emerges through repeated deference.
- Loss of agency emerges through low-friction automation.
- Automation bias emerges through confident AI presentation.
- Unequal participation emerges when the system privileges one role, language, expertise level, or workflow.
- Accountability gaps emerge when the final outcome is co-produced but responsibility is not.

The design implication is that ethical AI needs interaction design, not just model policy. Contestability, reversibility, intervention, and meaningful human control must exist throughout the process, not only at the beginning or the end.

### Why It Matters For Tammy

This paper supports a more mature AI experience thesis:

AI value is not just whether the model can produce a good answer. It is whether the human-AI system sustains useful, agency-preserving, accountable collaboration over time.

For Tammy, this creates a concrete leadership agenda:

- Define what healthy human-AI collaboration looks like in a given workflow.
- Instrument interaction trajectories, not just outputs.
- Watch for drift: passivity, over-reliance, conceptual divergence, repetitive loops, and failed repair.
- Treat handoffs, checkpoints, interruptions, and corrections as core product moments.
- Make "interaction explainability" visible: not just why the model answered, but how the human and AI got here together.
- Design governance around evolving participation and authority, not static permission screens.

## Combined Takeaway

The Coordination Zones paper is the practical product-design vocabulary. It helps a team decide the shape of AI involvement at each moment.

The Interaction-Centered Intelligence paper is the evaluation and governance vocabulary. It helps a team decide whether the relationship is getting healthier, more legible, more balanced, and more accountable over time.

Together, they suggest a design-leadership problem worth owning:

Design the conditions under which people can safely delegate to AI without becoming passive, confused, over-persuaded, or unaccountable.

That is the trust layer in more operational language. It includes:

- Autonomy levels.
- Salience controls.
- Workplan gates.
- Human approval and override.
- Evidence and attribution.
- Interaction trajectory monitoring.
- Escalation and repair.
- Progressive autonomy.
- Drift detection.
- Accountability across human and AI actors.

## Product Review Questions

Use these questions when evaluating an AI feature or agentic workflow:

1. What zone is this moment in: done-for-me, done-under-me, done-with-me, or done-without-me?
2. Is that zone appropriate for the task risk, user expertise, reversibility, and emotional stakes?
3. What is the AI actually doing that the user cannot see?
4. Where does the user have real control versus decorative control?
5. What should become more salient when confidence drops, stakes rise, or the user appears confused?
6. Where should the agent pause for approval before continuing?
7. What would the audit trail need to show after something goes wrong?
8. What signs would indicate interactional drift: passivity, over-reliance, confusion, repetitive loops, or divergence from the user's goal?
9. How does the user recover, correct, contest, interrupt, or take over?
10. What human judgment should the system preserve or strengthen rather than replace?

## Cautions

Both sources are useful, but they should not be over-claimed.

The Coordination Zones paper is based on artifact analysis of 60 commercial applications, expert judgment, and internal validation through AWS design work. It is a strong framework for practice, but it is not yet a broadly validated empirical standard.

The Interaction-Centered Intelligence paper is a theoretical synthesis and research agenda. It offers strong language for evaluating long-running human-AI collaboration, but the metrics and methods still need operational development.

The practical move is to treat both as design-leadership scaffolding: strong enough to guide critique, strategy, and product framing, but not as settled doctrine.

## Sources

- arXiv, "Human-AI Coordination Zones: A Framework for Designing Human-in-the-Loop Experiences with Agentic AI" (published May 1, 2026): https://arxiv.org/abs/2606.09848
- arXiv, "Interaction-Centered Intelligence: Toward an Interaction-Based Theory of Human-AI Co-Creation" (published May 30, 2026): https://arxiv.org/abs/2606.00807
- Osprey AI Overnight Brief, June 29, 2026: `/Users/tammysnow/tamknowledge/04_Reviews/Daily/Osprey/2026-06-29.md`
