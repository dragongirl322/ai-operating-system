# Human-Centered AI: My Foundations Reference

*A working reference for the advisory practice. The stance, the borrowed stack, and the one thing I build myself.*

---

## The Stance

Most design leaders are chasing the algorithm. They treat the technology as the fixed point and ask how humans adapt to it. That is backwards. The human is the fixed point. The technology is what we tweak.

The line that keeps the room, and the line that loses it, are close together. Get it right:

**Humans don't change much. Task allocation does.**

Working memory, the need for feedback, error tendencies, the drive for mastery: stable for decades, stable now. What moves is the division of labor. When the cost of a first draft drops to zero, the human's job shifts from producing to judging. That is not humans bending to the algorithm. That is the work being reallocated while the human stays exactly the same.

Say "AI changes everything" and you concede the argument. Say "nothing changes" and the keyholder answers with "my team ships three times the output now," and I'm on my heels. The precise claim wins: the human is constant, the allocation moves. Shneiderman's own framework concedes this. That is the whole point of separating the two axes.

One flag I plant on purpose: human-centered means **capable**, not **comfortable**. They diverge constantly. Designing for what people say they want in the moment is the soft version everyone claims. Designing so people leave more capable and more free is the harder stance, and it is mine.

---

## Ask 1: Core Design Guidelines

I am not reinventing this. I am stacking tested work by altitude and committing to it in public.

| Layer | Source | What it covers |
|---|---|---|
| **Substrate** | Nielsen's 10 Usability Heuristics (1994) | The most-validated general set. Timeless. |
| **Substrate** | Shneiderman's 8 Golden Rules of Interface Design | Overlaps Nielsen, sharper on user control and memory load. The direct through-line into HCAI. |
| **AI overlay** | Amershi et al., 18 Guidelines for Human-AI Interaction (Microsoft, CHI 2019) | AI-specific, empirically tested, organized by *when* they apply: up front, during use, on failure, over time. |
| **GenAI top coat** | Weisz et al., Design Principles for Generative AI Applications (CHI 2024) | The generative-era extension. Trust calibration, source citation, friction against overreliance. |

Nielsen and Shneiderman are the timeless base. Amershi is the AI layer. Weisz is the generative coat. That is a defensible spine I can hold to.

---

## Ask 2: Training — Where, What, How Much, How

The decision architecture already exists. I assemble it. I don't author it.

1. **Where to apply AI at all** — comparative advantage. Start at Fitts's List (1951): what humans do better versus what machines do better. Dated as static allocation, but the question is right. Modernize with complementarity thinking.
2. **How much autonomy** — Shneiderman's 2D grid (below). Place the task by consequence and reversibility.
3. **What type** — sort by task nature (predict, classify, generate, retrieve, optimize) against cost of error.
4. **How to build it** — design the control and feedback affordances with Amershi's 18.

Five sessions, built entirely on tested work. None of it mine to invent. All of it mine to teach well.

### The engine: Shneiderman's Two-Dimensional HCAI Framework

Pull apart the two things everyone collapses into one slider. Automation and human control are **independent axes**, not a tradeoff.

- **Low automation / low control** — dead zone. Primitive, no leverage.
- **High automation / low control** — excessive computer control. Runaway, opaque, unaccountable.
- **Low automation / high control** — excessive human control. Manual, error-prone the moment the human is overloaded.
- **High automation / high control** — the target. Reliable, safe, trustworthy. The machine does the work; the human holds intent and can intervene.

The discipline is *not* "always aim top-right." It is: decide on purpose which tasks need full human control, which need full computer control, and which belong in high/high. A pacemaker needs full automation because humans are too slow. A high-consequence, low-reversibility judgment needs the human. The framework forces that to be a decision, not an accident.

---

## Ask 3: Designing New Patterns for New Paradigms

This is the one place I build, because it is the differentiation. The rule:

**New paradigms don't need new principles. They need new patterns that express old principles under new constraints.**

Three moves:

1. Name the invariant principle (from the stack).
2. Name what is genuinely new about the medium.
3. Derive the pattern as the bridge between them.

**Worked example.** "Visibility of system status" is invariant. What's new with generative AI: outputs are probabilistic and the system can't tell when it's wrong. So the pattern becomes uncertainty surfacing, confidence signaling, source citation. The principle held. The pattern is new because the failure mode is new.

That derivation method is mine. It stands on foundations no one can argue with.

---

## Where the Value Actually Sits

"I apply Nielsen, Shneiderman, and Amershi" is table stakes. A bootcamp teaches that. The borrowed stack earns me the room. It is not the moat.

The moat is two things: the derivation method in Ask 3, and my judgment about which quadrant a task belongs in and whether the keyholder will accept the allocation. That last part is the A-to-B bridge. The frameworks get me in the door. The conversion is what I sell. I will not let the modesty of "I didn't reinvent it" hide where my value lives.

---

## References

- Nielsen, J. (1994). *10 Usability Heuristics for User Interface Design.* Nielsen Norman Group.
- Shneiderman, B. *Eight Golden Rules of Interface Design.* In *Designing the User Interface* (Addison-Wesley; multiple editions).
- Fitts, P. M. (1951). *Human Engineering for an Effective Air Navigation and Traffic Control System.* National Research Council. (The "Fitts's List" / MABA-MABA allocation.)
- Amershi, S. et al. (2019). Guidelines for Human-AI Interaction. *CHI '19.* DOI: 10.1145/3290605.3300233
- Shneiderman, B. (2020). Human-Centered Artificial Intelligence: Reliable, Safe & Trustworthy. *Int'l Journal of Human–Computer Interaction*, 36(6), 495–504. DOI: 10.1080/10447318.2020.1741118
- Shneiderman, B. (2020). Human-Centered AI: Three Fresh Ideas. *AIS Transactions on HCI*, 12(3), 109–124. DOI: 10.17705/1thci.00131
- Shneiderman, B. (2022). *Human-Centered AI.* Oxford University Press.
- HCIL project hub (book, four papers, videos, tutorial): hcil.umd.edu/human-centered-ai
- Weisz, J. et al. (2024). Design Principles for Generative AI Applications. *CHI '24.* DOI: 10.1145/3613904.3642466

---

*Humans don't change all that much. We shouldn't force them to bend to the will of the algo.*
