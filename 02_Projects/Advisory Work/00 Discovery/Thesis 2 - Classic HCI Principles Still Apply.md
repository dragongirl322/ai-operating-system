---
title: "Thesis 2 — Classic HCI Principles (Shneiderman, Nielsen) Still Apply, No New Principles Needed"
date: 2026-06-30
tags: [human-centricity, ai-ux, hci, usability-heuristics, shneiderman, nielsen]
conclusion: largely-confirmed-with-nuance
---

# Thesis 2: Classic HCI Principles Still Apply — We Just Need to Apply Them

> "The human centered design principles that have applied for years continue to apply today because they are great principles. I'm talking about Shneiderman's, Nielsen's, etc. They are simply being applied to new technologies and possibilities and to the fact agents can, in theory, use their super intelligence to do things that have traditionally been done by humans. I submit we don't need new principles we just need to figure out how and where to apply the ones that have worked across time, form factors, surfaces, and paradigms."

## Conclusion: **Largely Confirmed, with important nuance**

Substantially supported by the most authoritative HCI voices — including Jakob Nielsen himself and Nielsen Norman Group's current AI-agent content — but the picture is not unanimous. A meaningful contingent of practitioners and at least one major peer-reviewed academic stream (Microsoft Research's Amershi et al.) argue the classic principles need significant extension/reinterpretation, not pure reapplication. The strongest, most convergent finding: **the underlying heuristics hold, but their expression and implementation must change substantially for agentic systems** — a middle position closer to the thesis than to "we need entirely new principles," but not a pure restatement of it either.

## Summary

**Jakob Nielsen (NN/g co-founder) gives the single strongest, most direct piece of evidence** — he literally wrote the 10 heuristics being discussed. On his current blog, Nielsen states his heuristics "still apply — they are still solid" because they are broad heuristics about human cognition, not technology-specific standards, and "humans don't change." Crucially, he simultaneously argues current AI products are "fraught with basic usability errors, violating decades-old UX findings" and that AI firms "need more UX, not less" — while also calling AI "the first genuinely new UI paradigm in 60 years." This is a nuanced position: the principles don't change, but AI is framed as a genuinely novel UI paradigm requiring serious, fresh design investment to apply them correctly — not trivial reapplication.

**Nielsen Norman Group's institutional content reinforces this.** NN/g's "AI Agents as Users" article makes a near-verbatim version of the thesis: "None of these recommendations are new. They are the same principles that make interfaces more usable for humans with disabilities, more robust across devices and contexts, and more maintainable over time." This converges with Nielsen's personal statement — though note both originate from the same institutional lineage, so it's not fully independent corroboration on its own.

**Ben Shneiderman's position is consistent but less directly stated on this exact question.** His 2022 book *Human-Centered AI* doesn't reject classic HCI principles; it reframes the goal of design — arguing AI should be designed for comprehensibility, predictability, and controllability rather than mimicking human-like autonomy, offering 15 governance-level recommendations layered on top of, not replacing, established usability/UX values. No direct Shneiderman quote was found explicitly saying "we don't need new principles, just new application" — this is an inference from his framework, so it should be treated as **suggestive, not confirmed** for that specific framing.

**The most direct academic counterpoint is Amershi et al.'s "Guidelines for Human-AI Interaction"** (Microsoft Research, CHI 2019, ~1,360 citations — highly credible, widely cited). Their framing is explicitly hybrid: classic interaction guidelines "hold" with AI systems, but AI's accuracy/failure modes and adaptive behavior "raise new challenges" requiring "updated guidance," leading them to propose 18 new, AI-specific guidelines (not just relabeled old ones). This is a credible, peer-reviewed counterweight: it agrees the foundations hold but insists meaningfully new guidance was needed in practice. A related CHI 2020 paper ("Re-examining Whether, Why, and How Human-AI Interaction Is Uniquely Difficult to Design") was written specifically to interrogate — and partially push back on — claims that AI interaction is "uniquely difficult," landing on a nuanced middle position about uncertainty and output complexity as genuinely new design challenges.

**Industry/practitioner voices are more split, with a vocal minority explicitly arguing for new principles.** Several recent (2025) UX-industry essays argue agentic AI represents a "paradigm shift" because it inverts the basic UX assumption that users initiate and systems react — agents now hold and execute intent, sometimes autonomously. These explicitly call for "new heuristics," citing consistency-breaking behavior (same prompt, different output) and black-box decision-making. These are credible-but-lower-authority sources (independent essayists/consultants, not peer-reviewed or from a major lab), and they conflict directly with Nielsen/NN/g's position — a genuine, unresolved point of disagreement in the field.

**Academic synthesis work tends to extend rather than discard classic methodology.** For example, a paper on "Design Principles for Human-Agent Interaction" adapts Nielsen and Molich's (1990) heuristic evaluation method to validate new AI-specific design principles — suggesting the evaluation methodology and underlying values persist even where new content-level principles are added. This is more "extend" than "replace," lending modest support to the thesis's spirit if not its letter.

**Overall:** The claim is best characterized as confirmed for the foundational/psychological layer (consistency, feedback, user control, error prevention, reversibility — these survive essentially unchanged in name and intent across every source reviewed) but unclear/contested for the operational layer (concrete guidelines, evaluation heuristics, interaction patterns), where credible sources — including Microsoft Research's peer-reviewed CHI work — argue genuinely new guidance was necessary. No source argued the classic principles were wrong or irrelevant; disagreement centers on whether reinterpretation amounts to "the same principles" or constitutes something new in practice.

## References

1. **"Classic Usability Important for AI"** — Jakob Nielsen, Jakob Nielsen on UX (Substack). https://jakobnielsenphd.substack.com/p/classic-usability-ai — Highest-credibility source: author of the original 10 heuristics, directly addressing whether they still apply to AI. Confirms thesis with nuance.

2. **"AI Agents as Users"** — Nielsen Norman Group. https://www.nngroup.com/articles/ai-agents-as-users/ — Institutional NN/g position explicitly stating recommendations for AI agent design "are not new." High credibility, though not fully independent of Nielsen personally.

3. **"How I Developed the 10 Usability Heuristics"** — Jakob Nielsen / UX Tigers. https://www.uxtigers.com/post/usability-heuristics-history — Background on the heuristics' design intent as broad, technology-agnostic rules of thumb.

4. ***Human-Centered AI*** — Ben Shneiderman, Oxford University Press, 2022; overview via Institute for Systems Research (UMD) and HCIL UMD. https://isr.umd.edu/news/story/new-book-by-ben-shneiderman-focuses-on-humancentered-ai-opportunities · https://hcil.umd.edu/human-centered-ai/ — Authoritative author source; argues for reorienting (not replacing) classic HCI values; treat as suggestive support only.

5. **"Bridging the Gap Between Ethics and Practice: Guidelines for Reliable, Safe, and Trustworthy Human-centered AI Systems"** — Ben Shneiderman, ACM Transactions on Interactive Intelligent Systems, 2020. https://dl.acm.org/doi/10.1145/3419764 — Peer-reviewed ACM paper; 15 governance-level recommendations layered atop existing HCI foundations.

6. **"Guidelines for Human-AI Interaction"** — Saleema Amershi et al., Microsoft Research, CHI 2019. https://www.microsoft.com/en-us/research/blog/guidelines-for-human-ai-interaction-design/ (paper: https://dl.acm.org/doi/10.1145/3290605.3300233) — Highly credible, heavily cited peer-reviewed CHI paper. Key counter-nuance: classic guidelines "hold," but new AI-specific guidance is needed due to accuracy/failure-mode/adaptivity issues.

7. **"Re-examining Whether, Why, and How Human-AI Interaction Is Uniquely Difficult to Design"** — Yang, Steinfeld, Rosé, Zimmerman, CHI 2020. https://dl.acm.org/doi/10.1145/3313831.3376301 — Peer-reviewed CHI paper directly interrogating the "AI is uniquely hard to design for" claim.

8. **"Design Principles for Generative AI Applications"** — CHI 2024. https://arxiv.org/pdf/2401.14484 / https://dl.acm.org/doi/10.1145/3613904.3642466 — Peer-reviewed; proposes a two-tier principle/strategy framework for GenAI UX. Flagged as a lower-confidence read due to PDF parsing limits during research — worth a follow-up manual read.

9. **"Design Principles for Human-Agent Interaction"** — arXiv preprint. https://arxiv.org/html/2606.20630v1 — Synthesizes HCI literature into 14 principles and explicitly adapts Nielsen and Molich's (1990) heuristic evaluation methodology to validate them.

10. **"Designing for Autonomy: UX Principles for Agentic AI"** — UXmatters, Dec 2025. https://www.uxmatters.com/mt/archives/2025/12/designing-for-autonomy-ux-principles-for-agentic-ai.php — Credible industry trade publication; explicit counter-perspective arguing classic heuristics "break down" under agentic autonomy. Single-author essay, moderate credibility, useful for balance.

11. **"UX Evolution Through Agentic AI: A Paradigm Shift in Design Thinking"** and related Medium/Substack essays — Independent practitioner essays, 2025. Lower-authority but consistent counter-voice arguing for a paradigm shift requiring new mental models.

12. **"AI usability principles: 9 UX heuristics that actually work"** — Eleken. https://www.eleken.co/blog-posts/ai-usability-principles — Industry blog, moderate credibility; shows practitioners often present AI heuristics as adaptations of Nielsen's rather than fully new inventions.

*Methodology note: The Shneiderman "no new principles needed" framing relied on inference rather than a single quotable statement and is flagged as suggestive, not confirmed. The strongest convergence (Nielsen personally + NN/g institutionally + heuristic-evaluation-reuse pattern in CHI papers) supports the thesis. The strongest documented disagreement (Amershi/Microsoft CHI 2019, plus independent practitioner essays) is real, credible pushback and is represented here as genuine tension rather than resolved in the thesis's favor.*
