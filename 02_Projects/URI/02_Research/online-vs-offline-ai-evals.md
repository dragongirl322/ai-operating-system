# Online vs. Offline Evals for AI

## Definitions

**Offline evals** — Pre-deployment assessments run against static datasets with known expected outputs, in a controlled environment disconnected from live users. They answer: *"Is this good enough to ship?"*

**Online evals** — Production assessments run on real user traffic, measuring how the system performs with live, unpredictable inputs. They answer: *"Is this actually working for users?"*

## Examples

### Offline
- Running a golden dataset of 500 customer-support questions through a RAG pipeline and scoring answer accuracy
- Benchmarking against public (MMLU) or internal test sets
- LLM-as-judge grading on a curated prompt set before release
- Regression testing after a prompt or model change

### Online
- A/B testing two prompt versions; comparing thumbs-up rates or task completion
- Sampling 1% of production conversations and scoring with an automated judge
- Tracking deflection rate, escalation rate, or user retention
- Canary deployments monitoring quality on a small traffic slice

## Best Practices

### Offline
1. Build golden datasets from real (anonymized) production traffic; refresh regularly to avoid drift
2. Cover edge cases and adversarial inputs, not just happy paths
3. Validate LLM-as-judge against human judgment; check inter-rater agreement
4. Version eval sets and run them as regression gates in CI
5. Avoid contamination — don't eval on training data

### Online
1. Define quality metrics before launch; pair with guardrail metrics (latency, cost, safety)
2. Sample intelligently — representative slices, oversampling high-risk segments
3. Use implicit signals (retries, rephrases, abandonment) alongside sparse explicit feedback
4. Feed production failures back into the offline golden set
5. Roll out gradually (canary → % ramp) with automated rollback triggers

## The Flywheel

Offline gates what ships → online reveals what offline missed → production failures become new offline test cases. Human-in-the-loop review adds the most value adjudicating ambiguous online cases that automated judges get wrong; those adjudications become the highest-value additions to the offline set.
