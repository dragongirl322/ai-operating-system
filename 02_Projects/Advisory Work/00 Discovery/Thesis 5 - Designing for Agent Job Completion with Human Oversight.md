---
title: "Thesis 5 — Designing for Agent Job Completion with Human Oversight and End-User Engineering"
date: 2026-06-30
tags: [human-centricity, ai-ux, hci, human-in-the-loop, agentic-ux, end-user-development]
conclusion: partially-confirmed
---

# Thesis 5: Designing for Agent Job Completion with Human Oversight

> "We have to design for the paradigm of helping agents successfully complete the job to be done while allowing the human to monitor and optimize for success and to be able to fix problems when they are encountered. So essentially we want every human who uses AI to be able to 'design and engineer' solutions that make it easier for the agent to do its job."

## Conclusion: **Partially Confirmed**

The thesis splits into two claims with different evidentiary strength.

- **Claim A** — agentic AI design must let humans monitor, oversee, and correct/fix agent behavior — is **confirmed** by strong, convergent evidence across multiple independent, credible sources (academic HCI, major industry guidelines, and practitioner consensus).
- **Claim B** — the goal is to make *every* (non-technical) human user able to "design and engineer" agent behavior — is **unclear/aspirational**. It's discussed in real but smaller, more emergent literatures, and at least one rigorous recent usability study found this aspiration largely unmet in practice.
- The "Jobs to Be Done" framing applied specifically to AI agents is real but is **early-stage practitioner/blog discourse, not yet established consensus** — it appears mostly within one small, overlapping cluster of authors, so it should be treated cautiously.

## Summary

**Human oversight as a design paradigm is well-supported.** Three independent, high-credibility lineages converge: (a) Microsoft's HAX Toolkit, built on Amershi et al.'s peer-reviewed "Guidelines for Human-AI Interaction" (CHI 2019, 1,300+ citations), explicitly structures guidelines around stages including "when the system is wrong" and "over time" — designing for correction and ongoing monitoring; (b) Google PAIR's People + AI Guidebook organizes its framework around "Feedback + Control" and "Errors + Graceful Failure" as core pillars; (c) Nielsen Norman Group's recent agentic-UX research and related practitioner writing converge on patterns like "Intent Preview" (show what the agent plans to do before it acts) and keeping humans "in the loop with review, feedback, and rollback options." Apple's Generative AI Human Interface Guidelines independently echo the same principle — user agency, transparency, and the ability to override AI suggestions. This is real convergence across four organizationally independent sources, not a single-source claim.

**The "human-in-the-loop" framing itself is contested, not uncritically endorsed.** Multiple 2025–2026 sources independently argue that naive human-in-the-loop (HITL) designs often fail in practice: they create bottlenecks at agent speed, induce "automation bias" (over-trusting the AI), and can produce "HITL theater" — the appearance of oversight without the contextual visibility needed for it to be meaningful. The emerging alternative framing is "human-on-the-loop" — continuous monitoring with intervention on exceptions, rather than approval-per-step. This doesn't refute the thesis's core point, but complicates "monitor and fix problems when encountered" — the literature converges on the need for genuine visibility/context (e.g., intent preview, confidence/data lineage display), not just a checkpoint. The thesis is directionally right but underspecified relative to current critical discourse.

**Empowering non-technical/everyday users to "design and engineer" agent behavior is unclear, with mixed evidence.** There is a genuine academic literature here: "end-user development" (EUD) for AI, discussed in a peer-reviewed *Behaviour & Information Technology* article, describes component-based, rule-based, and template-based paradigms letting non-engineers shape AI/agent behavior. This is independently corroborated by a wave of industry "no-code AI agent builder" products and by mainstream agent platforms (custom GPTs, Claude Projects, Vertex AI Agents) that let ordinary users write persistent instructions. However, a more rigorous and very recent study — "Why Johnny Can't Use Agents: Industry Aspirations vs. User Realities with AI Agent Software" (a 31-participant usability study of commercial agents like Operator and Manus) — found a significant gap between the industry's aspirational framing (agents as easy, autonomous, user-configurable) and what non-technical users actually experience: misaligned mental models and agents lacking the transparency needed for users to meaningfully direct or correct them. This is a direct, fairly rigorous counterpoint to the thesis's optimistic framing — the aspiration is real in industry rhetoric, but empirical usability research suggests current systems don't yet deliver on it.

**"Jobs to Be Done" applied to AI agents is thin, single-cluster evidence.** A cluster of related essays explicitly proposes "Jobs-to-Be-Done + Intention Mapping" for agentic design, plus generic JTBD-for-AI commentary from a couple of consulting/marketing blogs. These are practitioner/consultant essays, not peer-reviewed research, and substantially overlap in authorship/network rather than being truly independent. No major lab (Microsoft, Google, Apple, NN/g) was found explicitly adopting "JTBD" terminology for agent design — they use adjacent but distinct vocabulary (user goals, intent, outcomes). This part of the thesis should be characterized as an emerging framing in industry UX discourse, not an established research consensus.

## References

1. **"Guidelines for Human-AI Interaction"** — Amershi, Weld, Vorvoreanu, Fourney, Nushi, Collisson et al., Microsoft Research / CHI 2019 (ACM). https://dl.acm.org/doi/10.1145/3290605.3300233 — Peer-reviewed, heavily cited (1,300+) foundational paper; validated via a 49-practitioner study against 20 products. Primary source for the HAX Toolkit.

2. **Microsoft HAX Toolkit (Guidelines for Human-AI Interaction)** — Microsoft Research. https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/ — Industry-standard practitioner toolkit derived from the Amershi paper.

3. **People + AI Guidebook** — Google PAIR. https://medium.com/google-design/people-ai-guidebook-41ec2ee5ec3f ; https://research.google/blog/responsible-ai-at-google-research-pair/ — Major lab's applied design guidance; organized around Feedback+Control and Errors+Graceful Failure; independent of Microsoft.

4. **"Design Considerations for Human Oversight of AI: Insights from Co-Design Workshops and Work Design Theory"** — Faas et al., arXiv 2510.19512 (2025). https://arxiv.org/pdf/2510.19512 — Recent academic preprint using co-design and work design theory; supports the need for human intervention/correction mechanisms.

5. **Nielsen Norman Group, agentic AI / "Intent Preview" coverage** — Nielsen Norman Group, nngroup.com — Leading reputable UX research outlet (note: a specific source URL returned a 404 during research and should be re-verified directly before being cited as load-bearing).

6. **Apple Generative AI / Human Interface Guidelines (Responsible AI)** — Apple, developer.apple.com — Industry-leading design authority; independently converges with Microsoft/Google on user control, transparency, and override capability.

7. **"Why Johnny Can't Use Agents: Industry Aspirations vs. User Realities with AI Agent Software"** — arXiv 2509.14528 (2025). https://arxiv.org/abs/2509.14528 — Rigorous 31-participant usability study of commercial AI agents (Operator, Manus); the key counter-evidence to the "everyday users can design/engineer agents" claim.

8. **"End-user development for democratising artificial intelligence"** — *Behaviour & Information Technology* (Taylor & Francis), 2022. https://www.tandfonline.com/doi/full/10.1080/0144929X.2022.2100974 — Peer-reviewed journal article establishing end-user development for AI as a real, if nascent, academic subfield.

9. **"Jobs-to-Be-Done and Intention Mapping: Translating Human Needs into Agent Actions"** — Itamar Medeiros, designative.info, 2025. https://www.designative.info/2025/09/24/jobs-to-be-done-and-intention-mapping-translating-human-needs-into-agent-actions/ — Practitioner/consultant essay, not peer-reviewed; part of a small, possibly non-independent cluster of similar essays. Use with caution — single-cluster evidence only.

10. **"From Human-in-the-Loop to Human-with-Agency: Why AI Oversight Fails When Humans Are Present but Powerless"** — Institute for Systems Integrity. https://www.systemsintegrity.org/from-human-in-the-loop-to-human-with-agency-why-ai-oversight-fails-when-humans-are-present-but-powerless/ — Industry/think-tank essay critiquing naive HITL design, independently corroborated below.

11. **"Why having 'humans in the loop' in an AI war is an illusion"** — MIT Technology Review, 2026. https://www.technologyreview.com/2026/04/16/1136029/humans-in-the-loop-ai-war-illusion/ — Reputable major tech publication; independently corroborates HITL critique in a different domain (military) with the same structural argument.

12. **"Human-in-the-loop has hit the wall. It's time for AI to oversee AI"** — SiliconANGLE, 2026. https://siliconangle.com/2026/01/18/human-loop-hit-wall-time-ai-oversee-ai/ — Third independent source corroborating the HITL bottleneck/automation-bias critique.

*Methodology note: several secondary summaries (the Amershi PDF guideline list, the NN/g article, and the JTBD essay) were partly generated from search snippets or incomplete fetches during research — flagged here so they can be spot-checked against primary text before being treated as load-bearing.*
