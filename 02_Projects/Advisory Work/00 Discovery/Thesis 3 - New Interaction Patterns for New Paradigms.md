---
title: "Thesis 3 — New Interaction Patterns for New Paradigms"
date: 2026-06-30
tags: [human-centricity, ai-ux, hci, interaction-design, agentic-ux, mixed-initiative]
conclusion: confirmed-directionally-not-yet-canonical
---

# Thesis 3: New Interaction Patterns for New Paradigms

> "While principles remain foundational and true, we do need to design new interaction patterns for new paradigms. The handoff between the human and the agent. The blend of voice, text input, images, etc. The mix of conversational AI with autonomous agentic output and GUI components. The continuity between devices and experiences."

## Conclusion: **Confirmed, directionally — but not yet a stable, settled canon**

Supported by convergent evidence from academic HCI research, major AI/tech company design teams, and respected industry voices. The field is young (most sources are 2024–2026) and terminology is still settling, so "confirmed" should be read as "directionally well-supported," not "established consensus" in the way decades-old GUI principles are.

| Sub-claim | Verdict |
|---|---|
| 1. Human-agent handoff needs new patterns | **Confirmed** — strongest evidence: academic lineage + corporate design org + editorial press |
| 2. Multimodal (voice/text/image) blending is a distinct pattern challenge | **Moderately confirmed** — real but weighted toward industry consensus over scholarly validation |
| 3. Blending conversational AI with GUI components (generative UI) | **Confirmed** — well documented and concretely shipping |
| 4. Cross-device continuity specific to AI agents | **Unclear** — relies on essentially one substantive source |

## Summary

**Human-agent handoff is the best-evidenced claim.** It connects directly to Eric Horvitz's 1999 "Principles of Mixed-Initiative User Interfaces" (Microsoft Research/CHI) — a genuinely foundational HCI concept about negotiated control between human and machine agents. Current research explicitly revives this lineage for LLM agents: the paper "Cocoa: Co-Planning and Co-Execution with AI Agents" frames itself as a new instantiation of mixed-initiative interaction and validates an interleaved-control pattern with a 16-person lab study and 7-person field deployment. Microsoft Design's official "UX design for agents" article independently states agent status must be "clearly visible at all times" and that users must remain in control of intervention — a design-pattern-level claim from a major company's design org. Industry sources (Smashing Magazine, agentic-UX pattern literature) converge on naming this "escalation pathway" / "handoff packet" patterns. This is convergence across academic, corporate, and editorial sources, not a single voice.

**Multimodal blending is real but less academically mature.** Microsoft Design's article explicitly requires agents to support "multimodal inputs and outputs... clearly visible to the user." Multiple independent practitioner sources converge on the claim that 2025–2026 voice products are "almost never voice-only," making seamless mode-switching the default. Most supporting sources here are practitioner guides rather than peer-reviewed HCI research, so this is weighted toward industry consensus rather than scholarly validation.

**Blending conversational AI with GUI components (generative UI) is the most concretely documented claim.** LangChain's "UX for Agents" series (founder Harrison Chase) argues chat-only interfaces are insufficient and documents three emerging patterns: spreadsheet UI, generative UI (agents composing UI components), and collaborative UI. This is corroborated independently by Vercel's AI SDK generative-UI feature, AWS Cloudscape Design System's "Generative AI chat" pattern guidance, and an arXiv survey paper on generative-AI interface design — three independent technical/design organizations converging on the same conclusion.

**Cross-device continuity specific to AI agents is the weakest sub-claim and should be treated as unclear.** The only source making an agent-specific (not generic responsive-design) claim is Microsoft Design's article, which is essentially one substantive source for this framing. It's plausible and consistent with the other findings, but not independently verified — per the stated methodology, a single-source claim cannot be called confirmed.

**A genuine counter-signal:** NN/g's "AI Agents as Users" article takes a more conservative position — for the case of agents *acting as users* of human-facing interfaces (browsing, form-filling), it argues existing accessibility patterns (semantic HTML, predictable labeling) already serve agents well, with no novel interaction pattern required. This doesn't contradict the thesis's framing (handoff, multimodal blending, generative UI), but is a real instance of an authoritative source pushing back on "new patterns are always needed," worth citing as nuance.

## References

1. **"UX design for agents"** — Microsoft Design. https://microsoft.design/articles/ux-design-for-agents/ — Primary source from a major AI company's design team; addresses multimodality, cross-device adaptation, and human control/handoff as explicit design requirements. High credibility, though promotional in tone.

2. **"Principles of Mixed-Initiative User Interfaces"** — Eric Horvitz, Microsoft Research, CHI 1999. http://erichorvitz.com/uiact.htm — Foundational peer-reviewed HCI paper establishing the academic lineage for handoff/negotiated control. Highest academic credibility; shows the concept is decades old and is now being explicitly re-applied to LLM agents.

3. **"Cocoa: Co-Planning and Co-Execution with AI Agents"** — arXiv 2412.10999. https://arxiv.org/pdf/2412.10999 — Peer-reviewed-track HCI research with a 16-person lab study and 7-person field deployment validating a new interleaved planning/execution pattern.

4. **"Designing Agentic AI: Practical UX Patterns for Control, Consent, and Accountability"** — Victor Yocco, Smashing Magazine. https://www.smashingmagazine.com/2026/02/designing-agentic-ai-practical-ux-patterns/ — Reputable, editorially-vetted design publication; author has relevant book credentials in this exact space.

5. **"UX for Agents, Part 3: Spreadsheet, Generative, and Collaborative UI/UX"** — Harrison Chase / LangChain. https://www.langchain.com/blog/ux-for-agents-part-3 — Primary source from a leading agent-infrastructure company; documents three distinct emerging patterns blending GUI and agentic output.

6. **"UX for Agents, Part 2: Ambient"** — LangChain. https://www.blog.langchain.com/ux-for-agents-part-2-ambient/ — Companion piece distinguishing "ambient" from "collaborative" agent UX patterns.

7. **"AI Agents as Users"** — Nielsen Norman Group. https://www.nngroup.com/articles/ai-agents-as-users/ — High-credibility counter-data-point: argues existing accessibility patterns largely suffice for agents-as-users scenarios.

8. **"Generative AI chat"** — AWS Cloudscape Design System. https://cloudscape.design/patterns/genai/generative-AI-chat/ — Official design-system pattern documentation from a major cloud/enterprise vendor; corroborates generative-UI patterns independently of LangChain.

9. **"Survey of User Interface Design and Interaction Techniques in Generative AI Applications"** — arXiv 2410.22370. https://arxiv.org/pdf/2410.22370 — Academic survey paper providing independent scholarly corroboration of generative-UI pattern emergence.

10. **"Terminal Is All You Need: Design Properties for Human-AI Agent Collaboration"** — arXiv 2603.10664. https://arxiv.org/pdf/2603.10664 — Academic paper on turn-taking/handoff design properties in CLI-based agent tools.

11. **"Secrets of Agentic UX: Emerging Design Patterns for Human Interaction with AI Agents"** — Greg Nudelman (author, *UX for AI*, Wiley 2025), UX Magazine. https://uxmag.com/articles/secrets-of-agentic-ux-emerging-design-patterns-for-human-interaction-with-ai-agents — Credentialed author, reputable trade publication; covers handoff and GUI/conversational blending with a concrete enterprise example.

*Lower-confidence supplementary sources used only as weak corroborating signals, not primary evidence: aiuxdesign.guide, agentic-design.ai, aiuxplayground.com (practitioner blogs without strong institutional/academic backing).*
