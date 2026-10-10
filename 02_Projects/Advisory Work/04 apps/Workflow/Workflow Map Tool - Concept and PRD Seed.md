# Workflow Map Tool: concept, data model, MVP, PRD seed

Captured 2026-10-09 by Idea catcher. Purpose: a tool for Workflow Fit consulting that may later be offered to customers at a price below competitors.

## IP guardrail
Assume Karen Holtzblatt / InContext holds copyright. Use only the general concept (separate "who coordinates with whom" from "what happens in what order"). Do not copy her shapes, symbols, names, or exact methodology. Use original terminology and visual language. Get a quick trademark/copyright check (ideally a short attorney review) before naming or selling.

## Working concept
- Coordination map: people, roles, and systems in a workflow, and what passes between them.
- Sequence map: ordered steps toward a purpose, with trigger, branches, and friction points.
- Both are views of one shared model. Swimlane (role x step) view later.
- Original vocabulary: actors, handoffs, friction points, phases.

## Data model (v1)
- Project: a client engagement or study.
- Source: interview, document, or observation, with notes and transcript link.
- Actor: person, role, team, or system (systems are first-class).
- Handoff: actor to actor, carrying a work item, with a label.
- Work item: document, message, request, or data.
- Sequence: purpose, trigger, owner.
- Step: order, actor, optional system, phase.
- Branch or loop: link between steps with a condition.
- Friction point: attaches to any step or handoff; description and severity.
- Evidence: quote or source link attached to any element.
- Merge group (v2): many individual maps combined with traceability.

## MVP scope (Workflow Fit first)
- Build actors, handoffs, steps, friction points; view as coordination map and sequence map.
- Fast drawing: keyboard shortcuts, templates, auto-layout.
- Every element links to evidence.
- Export PNG, PDF, JSON, plus CSV of friction points.
- One workspace with client viewer links.
- Defer: real-time multiplayer, AI, merging many maps, swimlane view, integrations, "update map from notes" AI.

## Economics notes (estimates, not verified)
- Stack idea: React Flow (MIT) + Supabase (Pro from $25/mo per supabase.com/pricing).
- Estimated fixed costs about $50-100/mo; estimated gross margin about 40% at 10 seats, about 80% at 50, about 89% at 200 at $15/seat. Excludes build time, support, marketing, AI costs.
- Competitor price points seen: Miro $8-20, Lucid ~$10-15 (unconfirmed), Eraser $15-45, UXPressia/Smaply $36-96 per seat.
- White space: structured people x systems x sequence model; maps that stay current; AI that edits maps; one model with several views; mid-price tier with free viewers.

## Seed prompt for Claude or ChatGPT
Act as a senior product manager. Interview me one question at a time to produce a PRD for a web app that lets consultants and teams create workflow maps showing people, roles, and systems, how work and information pass between them, and the ordered sequence of steps toward a purpose, including triggers, branches, and friction points.

Context: I'm a consultant (my practice is "Workflow Fit") and I'll be the first user. Later, customers may use it. I want pricing below competitors (Miro $8-20, Lucid ~$10-15, Eraser $15-45, journey-map tools $36-96 per seat) with strong margins. I'll supervise AI-assisted development, so favor a lean stack (React Flow, Supabase) and a data model that's easy to change.

Constraints: the product must be inspired by the general idea of separating "who coordinates with whom" from "what happens in what order." It must not copy any existing methodology's shapes, symbols, names, or procedure. Use original terminology and visual language. Flag any place where you think a requirement might copy someone's protected work.

Core model: Project, Source, Actor (person, role, team, or system), Handoff, Work item, Sequence (purpose, trigger), Step, Branch/loop, Friction point, Evidence. Two views of one model: a coordination map and a sequence map. Later: swimlane view, merging many maps, AI that edits maps from notes.

Start by asking about my users, the job to be done, and what a successful first client session looks like. After the interview, write the PRD with goals, non-goals, user stories, functional requirements, success metrics, open questions, and risks. Keep it to what an MVP needs.

## Next steps
1. Run the interview with Claude or ChatGPT.
2. Bring the PRD back to Idea catcher for a gap and similarity check.
3. Trademark/copyright check on terminology before naming or selling.
