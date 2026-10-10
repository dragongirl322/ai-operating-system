# Working rules

- Source of truth: /docs/Workflow-Fit-MVP-PRD.md and /docs/Workflow-Fit-Tech-Spec-Blueprint.md.
- Work is tracked in Linear: team "Workflow Fit" (key WF), project "Workflow Fit MVP".
  Issue IDs WF-1 to WF-31 match the spec's work orders.
- Work one issue at a time, in dependency order. Don't start an issue whose blockers aren't done.
- Move the issue to In Progress when you start. Comment progress and decisions on the issue.
- Name branches with the issue ID (e.g. wf-1-scaffold-repo).
- Open a pull request when acceptance criteria pass, and move the issue to In Review.
- Never merge, and never move an issue to Done. Tam does both.
- Schema changes only through Supabase migrations; regenerate types after each one.
- No map code until every isolation test in WF-5 passes.
- If a decision isn't covered by the spec, ask on the Linear issue instead of guessing.
