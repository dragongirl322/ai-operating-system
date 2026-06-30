# Positioning: Experience-Trust Evaluation for AI Products

  

### The human-in-the-loop white space

  

**Working thesis:** Two mature tooling markets bound a category that neither one fills. Engineering owns *"is the AI output correct?"* Research owns *"does this design work for users?"* Nobody owns *"does this AI experience earn enough trust to actually get used — and can a domain expert prove it?"* That question is becoming the gating factor for AI adoption in regulated, high-stakes workflows, and it has no incumbent.

  

---

  

## 1. The white space, stated plainly

  

The decision that determines whether an AI product succeeds is no longer whether the model is accurate. It's whether the human on the other side trusts the output enough to act on it, understands what the system did, and can recover when it's wrong. Today that judgment is made ad hoc — in pilots that stall, in "quiet sabotage" by skeptical experts, in adoption curves that flatline after launch.

  

There is no discipline, and no tool, that treats **experience-and-trust evaluation of AI products as a measurable, repeatable practice operated by domain experts.** That is the category this product defines.

  

---

  

## 2. Why the space is open: the two landscapes that bound it

  

### Landscape A — AI / LLM evaluation & observability tooling

  

Braintrust, LangSmith, Langfuse, Arize Phoenix, Confident AI, Latitude, Adaline, DeepEval, Ragas, Promptfoo, Fiddler, W&B Weave.

  

- **Measures:** output correctness — hallucination, faithfulness, RAG retrieval, regression, drift.

- **Operated by:** engineers and ML teams.

- **Human role:** an annotation queue bolted onto an engineering workflow.

- **Blind spot:** correctness is not the same as trust. A factually correct output that a user doesn't understand, doesn't believe, or can't override still fails in production. These tools cannot see that failure mode because they never leave the output layer.

  

### Landscape B — UX research & experience tooling *(your market map)*

  

Six adjacent sub-markets, none of which evaluate the AI experience itself:

  

| Sub-market | Representative tools | What it actually does |

|---|---|---|

| AI-native moderated research | Listen Labs, Strella, Outset | Interviews humans at scale |

| Usability-testing suites | Maze, UserTesting, Lyssna | Validates designs pre-build |

| Research synthesis & repositories | Dovetail, Looppanel | Organizes human-generated feedback |

| In-product analytics & replay | FullStory, Contentsquare, Sprig | Detects friction in live behavior |

| Predictive attention / design eval | Attention Insight, Neurons | Simulates where humans look |

| Enterprise XM | Qualtrics, Medallia | Measures experience sentiment at scale |

  

This market applies AI in four distinct ways — **analyst** (synthesizes human data), **moderator** (runs the interview), **predictor** (simulates attention), and **observer** (spots friction in behavior). Every one of them points the lens at *humans or human-facing designs.* None point the lens at *the AI's own behavior as the artifact under judgment.*

  

That missing fifth mode is the white space:

  

> **AI as subject, domain expert as judge** — the AI's decisions and outputs are the thing being evaluated for trust, comprehension, and recoverability, by the person qualified to know whether they're good.

  

### The gap, drawn

  

| | LLM-eval tooling | UX-research tooling | **This category** |

|---|---|---|---|

| **Measures** | AI output correctness | Whether a design works for users | **Whether an AI experience earns trust & adoption** |

| **Operated by** | Engineers / ML | Researchers (or "democratized" to all) | **Domain experts + product leaders** |

| **Lifecycle stage** | Dev + production monitoring | Pre-launch / live optimization | **Continuous, on real AI behavior in context** |

| **Human role** | Annotation queue (bolted on) | The subject being studied | **The evaluator — first-class** |

| **Incumbent** | Crowded, consolidating | Crowded, consolidating | **Open** |

  

---

  

## 3. Why human-in-the-loop is the moat, not a limitation

  

The obvious objection — "won't AI just evaluate the AI?" — is already answered by the evidence the research market itself produced:

  

- **NN/g**, testing the leading synthetic-users product against three prior real-participant studies, found synthetic users sycophantic — they praised concepts that real users questioned, and could not substitute for real people.

- **Loop11's own case study** of AI browser agents found **0–25% task success versus 62–95% for humans.**

  

The conclusion is durable: synthetic and predictive methods are supplements, never substitutes, for human judgment on consequential decisions. In regulated, high-stakes workflows — underwriting, claims, prior authorization, clinical intake — that ceiling is permanent, because the law increasingly *requires* a qualified human in the loop. The human-in-the-loop architecture isn't a constraint to engineer around. It's the defensible core.

  

---

  

## 4. Why now

  

Three forces converge in 2026 to make this category necessary rather than nice-to-have:

  

1. **Agentic deployment outran governance.** Adoption is mainstream in name and uneven in practice — only a small minority of insurers have scaled AI, and roughly 70% of scaling failures are organizational, not technical (Microsoft, 2026). Pilots stall at exactly the trust/adoption layer this category measures.

  

2. **Regulation is mandating explainability.** The EU AI Act classifies insurance underwriting and claims AI as high-risk, with documentation, human-oversight, and explainability obligations phasing in through August 2026; NAIC model bulletins and 25+ U.S. state guidances now require auditable, human-reviewed adverse decisions. "AI that cannot be explained is AI that cannot be adopted" has moved from slogan to compliance requirement.

  

3. **The trust gap is now measured and public.** HealthEdge's 2026 payer survey found 94% of payers have adopted AI while only 21% of members use AI tools — and explicitly tied that gap to transparency, explainability, and the perception that a human is still involved. That is a perception-and-trust gap, not a technology gap, and it is currently nobody's product.

  

---

  

## 5. Ideal customer profile

  

The buyer is a team that is **shipping a high-stakes AI experience into a regulated, expert-operated workflow** and discovering that accuracy didn't produce adoption.

  

- **Tier 1 — AI-native decision-surface vendors** (insurtech/health-tech building underwriter-, adjuster-, or clinician-facing AI): the experience *is* the product, they're engineering-led, and they lack the discipline to prove trust.

- **Tier 2 — Carriers, payers, and TPAs** rolling agentic AI to veteran staff who can stall it.

- **Common thread:** money at stake, regulatory accountability forcing explainability, and no existing function that owns the trust-and-adoption question.

  

---

  

## 6. Positioning statement

  

> **For** product and AI leaders deploying high-stakes AI into expert workflows,

> **who** find that model accuracy isn't translating into trust or adoption,

> **[Product]** is an experience-and-trust evaluation practice that lets domain experts judge real AI behavior — comprehension, trust, and recoverability — as a measurable, auditable discipline.

> **Unlike** LLM-eval tools that stop at output correctness, or UX-research tools that study users rather than the AI itself,

> **it** evaluates whether the AI experience earns the trust required to be used — with a qualified human in the loop, which both the stakes and the regulation now demand.

  

---

  

## 7. Objections & responses

  

| Objection | Response |

|---|---|

| "Our eval platform already covers this." | Output-correctness eval can't detect a correct answer that a user distrusts or can't override. Different layer, different failure mode. |

| "We'll democratize it like the research tools do." | Democratization is the right *motion*, wrong *object* — those tools democratize researching users; this democratizes evaluating the AI's trustworthiness. The framing transfers; the category doesn't exist there. |

| "Synthetic users will make this cheap." | The evidence (NN/g, Loop11) says synthetic methods fail on consequential judgment, and regulation mandates a human anyway. The human-in-the-loop requirement is the moat. |

| "Isn't this just compliance?" | Compliance is the floor. The product turns a regulatory burden (explainability, human oversight) into an adoption advantage (a trust signal users and regulators both reward). |

  

---

  

## 8. Defensibility

  

- **Regulatory tailwind** makes human-in-the-loop evaluation a requirement, not a preference — locking out fully-synthetic competitors in the highest-value segments.

- **Domain-expert workflow** is a different buyer and a different practice than engineering eval; incumbents in Landscape A would have to rebuild their product and their go-to-market to reach it.

- **Category-definition advantage:** the space is currently unnamed. Naming it, and owning the language of "experience-trust evaluation," is available now and won't be in 18 months.

  

---

  

## Appendix — Notes on the bounding markets

  

- Both bounding landscapes are **consolidating fast** (OpenAI/Promptfoo, ClickHouse/Langfuse on the eval side; UserTesting/UserZoom + User Interviews, Contentsquare/Heap+Hotjar on the research side), which compresses the field of potential fast-followers and raises the value of defining the open category before the consolidators notice it.

- The research market's **"make everyone a researcher" pitch** (Maze, Strella, Sprig) is the strongest available template for this category's go-to-market — borrow the democratization narrative, point it at AI-trust evaluation.

- Vendor accuracy claims in both markets are largely self-reported; an evaluation practice built on **independent, human-validated** judgment is itself a differentiator in a space full of unverifiable ">95% accurate" claims.