# Workflow Fit — MVP PRD

Oct 9, 2026 · @Tammy Snow

## Summary

Workflow Fit is a web app where a consultant and a client team map how work actually gets done, then decide, and record, where AI belongs and in what form. One shared model drives two views: a **coordination map** (who works with whom, and what passes between them) and a **sequence map** (what happens in what order toward a purpose).

The core bet: generic diagram tools can draw a workflow, but none turn it into an agreed, documented AI decision record. That record is the product's reason to exist, and it plays to Tam's AI governance depth.

## Users and job to be done

The primary job: **decide where AI belongs in a workflow, what form it should take, and why, and get the team to agree.**

| User | Who | What they need |
| --- | --- | --- |
| Facilitator | Tam (Workflow Fit), the first and only paying user in v1 | Set up an engagement, run sessions, hand the team something durable |
| Practitioner | IC designers, researchers, PMs, engineers doing the work | Drive the map themselves, not watch someone else drive it |
| Observer | Managers or directors, occasionally in the room | Read the maps and the AI decisions; understand the why |

A successful first session ends with three things: living maps the team can keep editing, a list of where AI applies and in what form, and a documented, agreed rationale for each choice.

## Goals and non-goals

The MVP must carry one real client engagement end to end, and be credible enough to show the URI board.

**Goals**

- One model, two views: edits in either view update the same underlying data.
- Client practitioners can drive the map, one editor at a time.
- Every AI decision is captured with its outcome, problem, affected roles, oversight level, evidence basis, and who agreed.
- Teams can see how solid the map is: what was researched, what is anecdotal, what is assumed.
- Client data is isolated per engagement from the first commit.
- The data model can change cheaply under AI-assisted development.

**Non-goals for the MVP**

- Real-time simultaneous co-editing.
- Storing, uploading, or linking evidence. Teams describe evidence; the tool never holds it.
- Swimlane view, merging many maps, and AI that edits maps from notes.
- Self-serve signup, billing, and transferring a workspace to a client.
- SSO, SOC 2, data residency options.
- Templates library, integrations, mobile editing.
- Matching the drawing power of general whiteboard tools.

## Core model and terminology

Every object lives once in the model; views only store layout. Three changes from the original list: **Source** folds into a plain-text field on Evidence notes (nothing is stored or linked), and **AI Fit decision** is new, as is Outcome (the job the team's customer is trying to get done), which anchors sequences and AI decisions.

| Object | What it is | Key fields | Appears in |
| --- | --- | --- | --- |
| Workspace | One client engagement; the security boundary | name, client name, members (owner, editor, viewer) | — |
| Project | A body of mapping work within a workspace | name, description | — |
| Outcome | What the team's customer is trying to get done, e.g. an enterprise customer's "manage employee performance" | statement, customer (who is trying to get it done), success signal (how we'd know it's done), evidence notes | Outcome list; end of each sequence; groups the AI Fit register |
| Actor | A person, role, team, or system | name, kind, description | Coordination (node); Sequence (step owner) |
| Work item | Something that moves: information, artifact, request, decision | name, kind | Handoff label; step input/output |
| Handoff | Work items passing from one actor to another | from actor, to actor, work items, channel | Coordination (edge) |
| Sequence | An ordered path that serves one or more outcomes | name, outcomes served, trigger | Sequence (start and end) |
| Step | One action by one actor | sequence, order, actor, description, inputs, outputs | Sequence (node) |
| Branch | A conditional split or a loop back | from step, condition, to step | Sequence (edge) |
| Friction point | Where work slows, breaks, or costs too much | description, severity (low, medium, high), attached to step or handoff | Both (marker) |
| Evidence note | A team's statement of what supports a claim | statement, source name (text only), confidence: Researched, Anecdotal, Assumed | Both (outline style) |
| AI Fit decision | Where AI goes, in what form, and why | outcome served (one, required), problem, linked steps, handoffs and friction, affected roles, AI form, oversight level, evidence notes, agreed by (names), agreed on (date) | Both (badge); AI Fit register |

**AI form** (editable list): Suggest, Draft, Check, Route, Act.

**Oversight level** (editable list, original wording): Person does the work, AI helps → AI proposes, person decides → AI acts, person reviews → AI acts, person is told.

These lists live in a config table, not code, so renaming them is a data change.

## User stories

**Facilitator**

1. As the facilitator, I create a workspace per client and invite their team by email, so client data never mixes.
2. As the facilitator, I set up a project with the customer outcomes the team serves, and one or more sequences, each serving an outcome and starting from a trigger, so the session starts with a clear frame.
3. As the facilitator, I hand the editor role to a participant mid-session, so the team drives.
4. As the facilitator, I export maps and the AI Fit register at the end, so the team has a leave-behind outside the tool.

**Practitioner**

5. As a practitioner, I add actors and draw handoffs between them, labeling what passes, so we see who depends on whom.
6. As a practitioner, I build a sequence step by step, assign each step to an actor, and add branches and loops.
7. As a practitioner, I mark friction on a step or handoff and say how bad it is.
8. As a practitioner, I tag any element with an evidence note and a confidence level, so we know what we actually know.
9. As a practitioner, I propose an AI Fit decision tied to an outcome and to specific steps or friction, and the team records who agreed.
10. As a practitioner, I return weeks later, update the map, and see what changed and who changed it.

**Observer**

11. As a director, I open the AI Fit register and read each decision's outcome, problem, oversight level, and evidence basis without learning the canvas.
12. As a director, I see at a glance which parts of the map rest on assumption.

## Functional requirements

Priority: **P0** = required for the first client engagement; **P1** = needed before showing the URI board.

| ID | Requirement | Priority |
| --- | --- | --- |
| FR-1 | Email sign-in; workspace owner invites members as editor or viewer | P0 |
| FR-2 | One active editor per project, shown to all; editor can hand off or release; others see the latest saved state on refresh | P0 |
| FR-3 | Coordination map: create, edit, delete actors (by kind) and handoffs; label handoffs with work items | P0 |
| FR-4 | Sequence map: trigger start, ordered steps owned by actors, outcome end; branches with a condition; loops back to earlier steps | P0 |
| FR-5 | Shared model: renaming or deleting an actor updates both views; deleting warns about dependent steps and handoffs | P0 |
| FR-6 | Cross-view highlight: select an actor to see its steps; select a step to see its handoffs | P1 |
| FR-7 | Friction points on steps and handoffs with three severities; visible in both views | P0 |
| FR-8 | Evidence notes on any element or AI Fit decision; confidence shown as outline style (solid, dashed, dotted) | P0 |
| FR-9 | Filter or overlay: show only Assumed elements | P1 |
| FR-10 | AI Fit decision form with all model fields; links to steps, handoffs, friction, actors | P0 |
| FR-11 | AI Fit register: one table per project, grouped by outcome, sortable by form and oversight level | P0 |
| FR-12 | Edit history per element: who, when, what changed | P1 |
| FR-13 | Auto-layout for the sequence map; manual positioning saved per view | P0 |
| FR-14 | Export: PNG or PDF of each view; PDF of the AI Fit register; full JSON of the project | P0 |
| FR-15 | Duplicate a project, to try an alternative or a future-state version | P1 |
| FR-16 | Outcomes: create and edit per project; link each sequence to one or more; every AI Fit decision links to exactly one | P0 |

## Security, stack, and pricing hypothesis

**Security built in from the first commit**

- Row-level security on every table, scoped to workspace membership. No query path bypasses it.
- No public or anonymous share links.
- No client content sent to third-party AI services. When AI editing arrives, it is opt-in per workspace.
- The tool holds no evidence, files, or raw logs, which keeps personal data out by design.
- Edit history doubles as an audit trail.
- Post-MVP, soon after: a security one-pager, data processing terms, SSO, then SOC 2 if enterprise demand requires it.

**Stack**

- Frontend: React with React Flow for both canvases; an auto-layout library (dagre or ELK) for sequences.
- Backend: Supabase (Postgres, Auth, row-level security). No custom server in v1.
- Data model: normalized core tables plus a JSONB attributes column per object, so new fields need no migration while the model is still moving.
- Layout stored separately from the model, one row per element per view. This is what makes swimlanes cheap to add later.

**Access and pricing**

- MVP: Tam owns each client workspace and folds its cost into the engagement fee. Clients buy nothing.
- Later: handover to a client-owned workspace on subscription.
- Pricing hypothesis to test: charge per editor, viewers free, or a flat price per workspace. Either undercuts per-seat competitors for an 8-person team, while hosting cost scales with stored data, not headcount.

## Originality and IP flags

Ideas are not protected; specific names, symbol sets, diagrams, and written procedures can be. These are the places this PRD comes closest to existing work. This is a design-risk review, not legal advice.

| Area | Risk | Mitigation |
| --- | --- | --- |
| Separating coordination from sequence | Low. A general idea found across process and systems thinking. | Keep our own names and visuals; don't adopt any one method's vocabulary or steps |
| Sequence shapes | Medium. Diamonds for decisions and circles for events echo standard flowchart and process-modeling notation. | Design an original visual language: condition labels on edges, not diamond nodes |
| Oversight levels | Medium. Published levels-of-automation scales exist. | Keep our own four levels and wording; don't match any published scale's count or labels |
| Friction points | Low. Generic term. Avoid journey-mapping names like "pain points" or service-design terms like "line of visibility." | Use "friction" and our own markers |
| Swimlane view (later) | Low. Swimlanes are a generic convention. | Avoid copying a specific tool's lane styling |
| Session method | Medium. A facilitation script for the AI Fit session could drift toward Tam's own AI Outcome Walkthrough, or toward published workshop methods. | Keep the facilitation method outside the product; the tool supports the session, it doesn't prescribe it |
| Product name | Unknown. "Workflow Fit" needs a trademark search before public use. | Search before showing anyone outside the engagement |

## Success metrics

The MVP succeeds if, within 6 months of launch, it is used in at least one client engagement and the URI board expresses interest in selling it.

| Metric | Target | Why it matters |
| --- | --- | --- |
| Client engagements using the tool | 1 or more | Tam's primary bar |
| URI board interest in selling | Expressed interest | Tam's second bar; depends on resolving ownership first |
| Edits made by client participants | 50% or more of edits | Proves the team drives, not just watches |
| AI Fit decisions agreed in the first session | 3 or more, all fields filled | Proves the core output works |
| Return visits after the engagement | Client edits the map at least once, 30+ days later | Proves the map is "living" |
| Share of elements marked Assumed | Tracked, no target | Shows where research is needed; a sales hook for URI's services |

## Open questions

- [x] **Ownership (resolve before showing the URI board).** Who owns the product: Workflow Fit, Steel Thread, or URI? And what does "URI sells it" mean: URI resells it to clients, licenses it from you, or it is included in the PE sale of AI offerings? Resolved: Tam is comfortable assigning URI the IP rights, paid for what URI takes on. Remaining: put the terms in writing before the board demo.
- [x] How does Workflow Fit relate to Steel Thread? Resolved: separate. Steel Thread stays entirely Tam's and is not used at URI.
- [x] Outcome statements: free text or a fixed pattern? Resolved: free text.
- [ ] Are the AI form and oversight level lists right? They should come from your governance practice, not from me.
- [ ] Pricing model to test: per editor with free viewers, or flat per workspace? At what price?
- [ ] Branded names for the two views, or keep the plain "coordination" and "sequence" maps?
- [ ] Typical map size per session (actors, steps)? This sets performance and layout needs.
- [ ] Hosting region and the first client's data-handling expectations.

## Risks

| Risk | Likelihood | Impact | Mitigation |
| --- | --- | --- | --- |
| IP terms still unwritten when the URI board shows interest | High | High | Write the IP assignment, price, and equity terms before any board demo; a buyer's diligence will check that URI clearly owns what it is selling |
| Enterprise security review blocks client participation | High | High | Security built in from day one; prepare a security one-pager and data terms right after the MVP |
| AI-assisted build breaks on two synced canvases | Medium | High | One model, layout stored separately; build the coordination map first, the sequence map second; test sync explicitly |
| Scope creep toward a general whiteboard | Medium | Medium | Hold the non-goals; every feature must serve the AI Fit decision |
| Validated by one user (n = 1) | High | Medium | Run the first engagement as a study: observe participants, log where they stall |
| Timeline misses the 18-month URI sale window | Medium | High | MVP aimed at one engagement in about 3 months, leaving room for a second engagement and a board demo |
| Oversight and AI form lists feel generic | Medium | Medium | Ground them in your governance practice; validate with the first client |
