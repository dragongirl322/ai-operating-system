# Systems Thinking Chapter Outline




## 1. Open

- Hook: February 2024, the British Columbia Civil Resolution Tribunal (CRT) rules against Air Canada. A grieving customer, Jake Moffatt, asked the airline's website chatbot about bereavement fares after his grandmother died. The chatbot told him he could apply for the discount retroactively, within 90 days. That was not the real policy. The real policy required the request before travel, and it lived on a different page of the same website. Air Canada's defense: the chatbot was "a separate legal entity, responsible for its own actions." The tribunal rejected it and asked the obvious question back: why should a customer have to double-check one part of a company's own website against another part of it.
- Land the tension in one line: the chatbot was not lying. It was fragmented. Nobody had connected the part of the system that talks to a grieving customer to the part of the system that knows the actual policy. That is not new. What is new is that it is now impossible to hide.

## 2. Reframe

- Systems thinking has always been the actual job of design and research leadership. Every "unrelated" one-off fix, every feature shipped without asking what it displaces elsewhere, was already a systems failure. AI did not invent this problem. Fragmented systems, teams that update a policy on one page and never touch the interaction layer three clicks over, are as old as multi-team organizations.
- What changed is not the presence of fragmentation. It is the danger of it, and the reason is specific: a human working inside a fragmented system carries tacit knowledge and intuition the system itself does not have. A phone rep unsure about a bereavement policy hesitates, hedges, says "let me check." That hesitation is systems awareness, even when nobody would call it that. It is a safeguard built from experience, not documentation.
- An agent has none of that instinct. It answers with total confidence regardless of whether the part of the system it drew from was the accurate part. It does not know what it does not know, and nothing in it pauses to check. The fragmentation a human would have quietly absorbed and corrected for, an agent will confidently act on, and hand the consequences straight to the customer with no human judgment in between to catch it.
- That is the exponent worth naming plainly: the same underlying fragmentation as always, but the buffer that used to catch it is gone.

## 3. The Core Model: Steel Thread and One Click Out

- Two paired ideas, not one. Steel Thread is the perceptual habit. One Click Out is the test you run once you've used it. Neither works alone: One Click Out without Steel Thread is a checklist run against whatever's directly in front of you, no wider than the ticket. Steel Thread without One Click Out is awareness with nothing done about it.
- **Steel Thread** (extending your existing concept, applied here at the level of individual craft rather than organizational influence): before working on any single part of a system, trace the thread of the human's actual journey through it. Not just the screen or workflow you were handed. What happens immediately before this moment for the person, what happens immediately after, and what else is adjacent to and dependent on this piece being right. It is a recognition skill: can you see the thread the person is walking, not just the node you were asked to fix.
- **One Click Out**: once the thread is visible, run three questions against it.
    - Is this the right problem?
    - Does a solution already exist elsewhere along that thread?
    - Could the solution I'm building here apply elsewhere along it?
- Position this pairing as the compressed, practical answer. Everything else in the chapter explains why it works, not how to do something different.
- Worked example, using the opening scene: the chatbot team was answering "can I get a bereavement discount." Steel Thread means asking what comes immediately before that question (a death in the family) and immediately after it (the actual refund process, living on a different page, owned by a different team, governed by a different, non-retroactive rule). Run One Click Out against what the thread reveals: is answering the question the right problem, or is making sure any answer matches the one true policy, wherever it lives, the real one? Does an answer already exist elsewhere in the system? Yes, the bereavement travel page. Could this response apply elsewhere? Yes: the chatbot and that page should be drawing from the same single source, so two conflicting truths can't exist in the first place. This should be the most memorable page in the chapter, and it now has a real, public, costly failure behind it instead of a hypothetical.

## 4. Where It Comes From

Treat each of the following as a paragraph, not a subsection. One sentence each on what it is, one sentence on what it hands the "One Click Out" model.

- **Meadows** — the shared vocabulary underneath all of it: stocks, flows, feedback loops. Why "the system fights back" is the starting assumption, not the exception.
- **The military precedent** — Army Design Methodology exists because a linear planning process failed against problems too interconnected for it. Mission command decentralizes decisions when feedback moves faster than the chain of command. Name it, don't unpack the full doctrine.
- **Cynefin** — sorts a problem before you try to solve it. Answers your first click-out question: is this the right problem, or is it even a problem you can solve the way you're trying to.
- **CATWOE** — root definitions expose when a "disagreement about the solution" is actually a disagreement about the problem itself.
- **Ackoff** — resolve, solve, dissolve, absolve. The dissolve option is the one nobody proposes, and it's often where your second click-out question lives.
- **Pattern Language** — coherence lives in how patterns connect across scale, not in any one component being well-made. Answers your third click-out question: could this apply elsewhere.
- One line of external validation: Elizabeth Stone (Netflix CPTO) naming systems thinking as a top-tier priority independently.

## 5. In Practice

- Two exercises maximum, chosen for zero facilitation overhead:
    - The domain-sort question, before any team proposes a solution: do we already know the cause and effect here, or will we only find out by trying it?
    - Run "One Click Out" live on whatever the team is currently building.
- One pointer, not a full curriculum embedded in the book: readers who want the full workshop sequence (root-definition worksheets, the dissolve cost/benefit tool, the pattern/playbook qualification test) go to the companion practitioner guide.

## 6. Close

- Return to the tribunal ruling. The line that matters most: why should a customer have to double-check one part of a company's own website against another part of it. Reframe it as the chapter's whole thesis in a single question: whether it's a customer or an agent doing the double-checking, that question is the entire test for whether you've traced the steel thread through your own systems.
- Ask the reader to hold that ruling in mind the next time they ship anything that touches more than one part of a system, human-facing or agent-facing.
- One-line bridge to the next skill in the book.



## Sources to Cite Directly

- Donella Meadows, _Thinking in Systems_
- Peter Checkland, Soft Systems Methodology (CATWOE)
- Russell Ackoff, problem typology and idealized design
- Christopher Alexander, _A Pattern Language_
- Dave Snowden, Cynefin
- Army Design Methodology (ADP 5-0, ATP 5-0.1)

## Sources for a Single Line, Not a Citation

- Jamshid Gharajedaghi, Peter Senge, Stafford Beer/Ashby, Meg Wheatley — useful lineage, not chapter-length material for a nine-skill book