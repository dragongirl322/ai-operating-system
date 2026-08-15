# Military Systems Thinking vs. Meadows: Notes Toward a Framework

## 1. What "soldiers are taught to think systemically" actually means

Codified in the **Army Design Methodology (ADM)** — ADP 5-0, ATP 5-0.1. Added on top of the older **Military Decision-Making Process (MDMP)**, a linear sequence (define problem → generate courses of action → pick one → execute) that kept failing against "ill-structured" problems: insurgencies, unstable governments, populations that adapt and react to your own moves rather than sitting still as a fixed target.

ADM's core moves:

- **Frame the operational environment** using **PMESII-PT** (Political, Military, Economic, Social, Information, Infrastructure, Physical environment, Time) — mapping how variables interact, not analyzing "the enemy" in isolation.
- **Frame the problem** as its own explicit step, before proposing solutions — because acting on the wrong frame is the most common failure mode.
- **Center of Gravity (CoG) analysis** — find the node holding the adversary's capability together, rather than attacking the most visible target.
- **Mission command / commander's intent** — push decision authority down to the lowest level, because on-the-ground feedback loops move faster than information can travel up and back down a command chain.

ADM is officially defined as applying critical and creative thinking to understand, visualize, and describe unfamiliar problems and approaches to solving them — built from _interconnected_ thinking activities rather than one linear procedure. It traces back to Israeli general Shimon Naveh's **Systemic Operational Design**, and cites Jamshid Gharajedaghi's _Systems Thinking_ as a foundational text.

## 2. Mapping to Donella Meadows

**Real overlap:**

|Meadows|Military equivalent|
|---|---|
|Stocks, flows, feedback loops|PMESII-PT environment framing|
|"All models are wrong, hold them loosely"|Continuous _reframing_ as the operation unfolds; OODA loop (Boyd) — Observe-Orient-Decide-Act as a repeating cycle, not a one-time plan|
|Distrust of centralized control in complex systems|Mission command / decentralized authority|
|Leverage points|Center of Gravity analysis|

**Where they genuinely diverge:**

- Meadows' _highest_-leverage points are upstream and abstract — paradigms, the goal of the system itself. Military CoG analysis stays lower on that hierarchy in practice: physical or organizational nodes, capabilities, chokepoints. It's leverage-hunting _within someone else's system to defeat it_, not leverage-hunting within your own system to steward it.
- Meadows' posture is diagnostic and humble about unintended consequences. Military systems thinking is adversarial and outcome-forcing by design — aimed at collapsing another system, not co-evolving with one.
- ADM was bolted onto MDMP, a hierarchical linear process, rather than replacing it. Even where the doctrine sounds like Meadows, the institution around it still wants a plan, a timeline, and an endstate in a way Meadows would call reductive.

## 3. A framework sketch for tech work

Keeping the compatible pieces, dropping the adversarial/command-and-control skeleton:

1. **Frame the environment before the problem.** Map actors, incentives, and feedback loops around the work — not just the stated ask. (PMESII-PT equivalent: users, incentives, adjacent systems, information flow, constraints.)
2. **Frame the problem explicitly, as its own step.** Write down what the problem actually _is_ before anyone proposes a solution.
3. **Find the actual leverage point** — not the most visible lever, but the one that changes the most downstream behavior with the least force.
4. **Set intent, then decentralize.** State the desired end-state in one sentence; let people closest to the fast-moving parts of the system act without waiting for it to travel up and back down.
5. **Run a fast OODA loop and reframe on purpose.** Build a short observe → reframe cycle into the actual cadence of the work, not just a retro at the end.

**Honest caveat:** the military version works because it accepts a hierarchical chain of command and a win/lose frame as given. Importing it into tech work means keeping the "map the system, decentralize decisions, reframe continuously" muscle while dropping the command structure it was built inside of — otherwise it's just MDMP with better vocabulary.