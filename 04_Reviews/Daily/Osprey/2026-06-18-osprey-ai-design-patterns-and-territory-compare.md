---
title: Osprey AI design patterns and territory comparison
aliases:
  - Osprey AI design patterns compare
  - Osprey Apple Google Meta Microsoft AI UX
tags:
  - osprey
  - ai
  - design
  - positioning
  - apple
  - google
  - meta
  - microsoft
created: 2026-06-18
---

# Osprey: AI design patterns and territory comparison

Prepared on June 18, 2026.

## Why this note exists

You asked for two things:

1. A design-pattern inventory focused on what is publicly visible from Apple, Google, Meta, and Microsoft about AI experience design and design-system or component evolution.
2. A comparison between those signals and your own territory.

The short version is that Apple, Google, Meta, and Microsoft are all moving beyond "chatbot as a box" and toward AI as a system behavior. They differ in emphasis, but the recurring themes are legibility, continuity across surfaces, refinement loops, and better human handoffs. Your territory still sits one layer above that: not only designing the interaction, but designing the conditions under which organizations and customers trust the interaction enough to adopt it.

## Part 1: Public design-pattern inventory

## Apple

### What Apple appears to believe

Apple's public guidance suggests a long-game view in which AI should become a native system capability rather than a separate power-user tool. The through-line is not "give engineers maximum model freedom." It is "make intelligence feel integrated, attributable, and controlled inside familiar product structures."

### Patterns Apple is making visible

- **Refinement over one-shot generation.** Apple explicitly updated its Generative AI guidance on **June 8, 2026** to add recommendations for letting people refine results and provide feedback during content generation. That is a strong signal that Apple sees AI as iterative and co-shaped, not just prompt-and-return.  
  Source: [Apple HIG: What's New](https://developer.apple.com/design/whats-new/), [Apple HIG: Generative AI](https://developer.apple.com/design/human-interface-guidelines/generative-ai)

- **System intelligence over isolated chat surfaces.** Apple Intelligence is framed around **personal context understanding, app actions, and on-screen awareness** across devices. The key interaction move is that people should be able to discover and act through Siri, Shortcuts, Spotlight, visual intelligence, and app surfaces without learning a separate AI UI every time.  
  Source: [Apple Intelligence overview](https://developer.apple.com/apple-intelligence/)

- **Schema-driven interaction.** Apple is pushing **App Intents schemas** and updated **App Shortcuts** guidance so apps can expose structured content and actions to Apple Intelligence and Siri. That implies a design pattern where AI works best when apps declare semantics the system can understand.  
  Source: [Apple HIG: App Shortcuts](https://developer.apple.com/design/human-interface-guidelines/app-shortcuts), [What's new in Apple Intelligence](https://developer.apple.com/apple-intelligence/whats-new/)

- **On-screen reference as a first-class pattern.** The **View Annotations API** introduces a conversational pattern where the user can refer to what is currently visible, and the system can understand it as an entity. That is a meaningful step toward context-aware HCI instead of command-style invocation.  
  Source: [Apple Intelligence overview](https://developer.apple.com/apple-intelligence/), [What's new in Apple Intelligence](https://developer.apple.com/apple-intelligence/whats-new/)

- **Testing AI behavior as behavior, not just code.** Apple's public emphasis on the **Evaluations framework** and **App Intents Testing** suggests a belief that AI quality has to be verified through system pathways and dynamic conditions.  
  Source: [What's new in Apple Intelligence](https://developer.apple.com/apple-intelligence/whats-new/)

### Design-system and component signals

- On **June 8, 2026**, Apple publicly updated or added guidance for `Siri`, `Snippets`, `App Shortcuts`, `Generative AI`, `Search fields`, `Searching`, `Tab bars`, `Menus`, `Sidebars`, `Scroll views`, and `App icons`.  
- Apple also shipped updated design resources including **iOS 27 / iPadOS 27 UI kits**, **Icon Composer 2**, and **SF Symbols 8 beta**.  
- The broader design language still carries the **Liquid Glass** direction introduced in 2025, but 2026 shows Apple extending that system into AI-aware patterns rather than treating AI as a separate layer.  
  Source: [Apple Design: What's New](https://developer.apple.com/design/whats-new/), [Apple Design Resources](https://developer.apple.com/design/resources/), [SF Symbols 8](https://developer.apple.com/sf-symbols/)

### Practical read

Apple's public pattern language points to AI that:

- lives inside existing app and OS anatomy
- reveals capability through structure instead of novelty
- favors guided refinement and contextual invocation
- keeps intelligence attributable to the app or system surface

This is the strongest public evidence for your read that Apple is optimizing for the end-user experience and long-term system coherence rather than just raw developer power.

## Google

### What Google appears to believe

Google is public about the fact that AI design needs new visual and interaction language. Compared with Apple, Google is more willing to foreground the design challenge itself: how do you make an evolving AI system feel trustworthy, discoverable, and expressive without making it chaotic?

### Patterns Google is making visible

- **Dynamic cues for discovery and trust.** Google's design write-up on Gemini says the assistant is "constantly learning and adapting," which means traditional linear design methods no longer fit. The design response is a system of **gradients, responsive containers, and intentional motion** that help users discover, learn, and master evolving features.  
  Source: [Google Design: Illustrating the Gemini App](https://design.google/library/gemini-ai-visual-design)

- **Guidance through motion, not just static UI.** Google describes motion in Gemini as a guiding element that shows the system is working with the user. Motion is being used to make system activity feel more transparent and to help users understand AI state.  
  Source: [Google Design: Illustrating the Gemini App](https://design.google/library/gemini-ai-visual-design)

- **Softness as an adoption strategy.** One of the clearest lines in Google's Gemini design story is that when the system is hard to approach, the design must be soft. That maps directly to lowering uncertainty at the edges of capability.  
  Source: [Google Design: Illustrating the Gemini App](https://design.google/library/gemini-ai-visual-design)

- **Human-centered AI patterns as a formal toolkit.** Google's **People + AI Guidebook** remains one of the strongest public AI UX artifacts from any company. It explicitly positions itself as methods, best practices, and patterns for designing with AI, grounded in research and broad expert input.  
  Source: [People + AI Guidebook](https://pair.withgoogle.com/guidebook-v2/)

- **Ambient, glanceable AI for new hardware.** Google's new **Jetpack Compose Glimmer** system for AI glasses rethinks the basics around focus, transparency, halation, typography, color, and motion. The important pattern is that ambient AI should appear when needed and disappear when not needed, earning attention instead of demanding it.  
  Source: [Google Design: Designing for Transparent Screens](https://design.google/library/transparent-screens), [Android Developers: AI glasses](https://developer.android.com/design/ui/ai-glasses)

### Design-system and component signals

- Google is extending **Material** into AI-adjacent form factors and behaviors rather than replacing it wholesale.
- Publicly visible updates include:
  - Gemini-specific visual language using gradients, motion, and responsive containers
  - **Jetpack Compose Glimmer**, described as a new design system for display AI glasses
  - formal AI design guidance through **PAIR / People + AI**
- The overall pattern is not a single AI component library, but a layered stack:
  - Material for system coherence
  - PAIR for human-centered AI patterns
  - Glimmer for ambient XR / glasses-specific interaction

### Practical read

Google appears strongest where AI is:

- visually expressive
- adaptive across contexts
- explicitly research-informed
- willing to invent new interaction language for emerging hardware

Compared with Apple, Google is more comfortable showing the scaffolding and experimentation behind the system.

## Meta

### What Meta appears to believe

Meta's public AI design stance is less formalized in a design system sense, but a few clear beliefs show up in official materials: AI should be **voice-forward**, **personal**, **social**, and **continuous across devices**, especially glasses, app, and web.

### Patterns Meta is making visible

- **Voice as the most natural entry point.** In the official Meta AI app announcement, Meta says voice is the most intuitive way to interact with Meta AI, and it built the app to let people start conversations quickly, including while multitasking.  
  Source: [Meta: Introducing the Meta AI App](https://about.fb.com/news/2025/04/introducing-meta-ai-app-new-way-access-ai-assistant/)

- **Persistent continuity across surfaces.** Meta emphasizes that you can start a conversation on glasses and continue it in the app or web, and that the Meta AI app becomes the companion layer for AI glasses. This is a continuity pattern more than a component pattern.  
  Source: [Meta: Introducing the Meta AI App](https://about.fb.com/news/2025/04/introducing-meta-ai-app-new-way-access-ai-assistant/)

- **Social discovery as product behavior.** The **Discover feed** is a distinctive Meta move: AI use is made socially legible by letting people see, remix, and share prompts.  
  Source: [Meta: Introducing the Meta AI App](https://about.fb.com/news/2025/04/introducing-meta-ai-app-new-way-access-ai-assistant/)

- **Personalization from platform context.** Meta says the assistant can remember preferences and use information people have already chosen to share across Meta properties. That suggests a design pattern where personalization is not just session memory but ecosystem memory.  
  Source: [Meta: Introducing the Meta AI App](https://about.fb.com/news/2025/04/introducing-meta-ai-app-new-way-access-ai-assistant/)

- **Future-facing but familiar.** Meta's public design blog has described four principles for AI products including creating familiarity and amplifying human capability. I could verify the existence of that official article, but the full page content did not render cleanly during this pass.  
  Source: [Meta Design: Designing AI products that are future-facing and familiar](https://design.facebook.com/blog/4-principles-for-designing-AI-products/)

### Design-system and component signals

Meta shows fewer public, formal, component-level AI design-system updates than Apple, Google, or Microsoft. The strongest public signals are product-pattern signals:

- app + glasses + web continuity
- voice-first interaction
- social prompt discovery
- memory/personalization
- richer document and image editing flows on the web

This means Meta currently looks more like a company designing **AI behavior across a product ecosystem** than a company publishing a mature public AI component system.

### Practical read

Meta seems strongest where AI is:

- socially mediated
- always available
- voice-led
- tied to wearables and everyday context

The weakness, from a public design leadership standpoint, is that the company exposes less formal public guidance about trustworthy AI interaction patterns than the others.

## Microsoft

### What Microsoft appears to believe

Microsoft is the most explicit of the four about turning AI experience design into a documented operating discipline. Publicly, it is treating AI not just as a product feature but as a design-system concern, an organizational design concern, and a governance concern.

### Patterns Microsoft is making visible

- **Trust as a design objective.** Fluent's **Responsible AI** guidance is direct: the goal is to build appropriate trust by being transparent, setting expectations, preventing overreliance, keeping users in control, and collecting feedback on outputs.  
  Source: [Fluent 2: Responsible AI](https://fluent2.microsoft.design/responsible-AI)

- **Conversation should extract capabilities, not clone apps.** Microsoft's Copilot guidance for MCP apps says agents should not recreate full applications inside Copilot. They should expose focused, native, task-oriented capabilities that work inside the conversational flow.  
  Source: [Microsoft Learn: UX guidelines for MCP apps in Copilot](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-mcp-apps-ui-guidelines)

- **Handoffs are a first-class pattern.** Fluent's **Handoffs** pattern treats cross-app movement as part of the AI experience itself. Copilot should infer intent, suggest next steps, preview transformations, and keep users in control as work moves across surfaces.  
  Source: [Fluent 2: Handoffs](https://fluent2.microsoft.design/handoffs)

- **Generative UI with progressive disclosure.** Microsoft's design write-up on the **Dynamic Action Button** in the Microsoft 365 Copilot mobile experience describes a floating, context-aware entry point that adapts in real time while trying to reduce cognitive load.  
  Source: [Microsoft Design: The new Microsoft 365 Copilot mobile experience](https://microsoft.design/articles/the-new-microsoft-365-copilot-mobile-experience/)

- **Agent design as structured planning.** Microsoft Copilot Studio's public **agent design framework** includes triggers, tools, channels, governance, evaluation, and success criteria. That is a notable signal: Microsoft is making agent design look like service design plus product design plus risk design.  
  Source: [Microsoft Learn: Use the agent design framework](https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/agent-design-canvas-framework)

### Design-system and component signals

- Fluent 2 publicly distinguishes:
  - **Fluent 2 design language**
  - **Fluent 2 Core UI Kits**
  - **Copilot UI Kits**
  - **Labs UI Kits**
- Fluent says the Copilot kits are **AI-focused components and patterns** across web, iOS, and Android.  
  Source: [Fluent 2: Start designing](https://fluent2.microsoft.design/get-started/design)

This is the clearest public evidence among the four that AI interaction patterns are being absorbed into a formal design-system structure.

### Practical read

Microsoft appears strongest where AI is:

- embedded in work
- operationalized through governance
- documented as reusable design practice
- explicit about trust, handoff, and control

Compared with Apple, Microsoft is much more public about the mechanics of designing AI work systems.

## Cross-company pattern map

### Shared patterns across Apple, Google, Meta, and Microsoft

These four companies are converging on several things:

- **AI is moving from destination UI to embedded system behavior.**
- **Refinement loops matter more than one-shot output.**
- **Continuity across surfaces is becoming core.**
- **Trust is now an interaction-design problem, not only a policy problem.**
- **Context is the new primitive.** Whether it is Apple's on-screen awareness, Google's adaptive cues, Meta's personal/social context, or Microsoft's work context, each company is trying to reduce the gap between user state and system response.

### Where they differ

- **Apple** emphasizes system coherence, semantic structure, and user-legible integration.
- **Google** emphasizes dynamic cues, expressive AI visual language, and new human factors for ambient computing.
- **Meta** emphasizes personal voice interaction, social discovery, and wearable continuity.
- **Microsoft** emphasizes work orchestration, structured handoffs, governance, and enterprise trust patterns.

## Part 2: Comparison to your territory

## Where your territory already aligns strongly

Your territory is highly consistent with the strongest public signals across all four companies:

- You focus on **trust as designed behavior**, not abstract sentiment.
- You focus on the **relationship between builder experience and user experience**, which is increasingly visible in how system patterns, agent frameworks, and evaluation models are being discussed.
- You focus on **human judgment, override, and adoption**, which maps directly to what Microsoft documents openly and what Apple implies through evaluation, schemas, and controlled system integration.
- You focus on **human-computer paradigm shifts**, and the clearest evidence here is that all four companies are moving away from screen-bound commands toward context-aware, persistent, multi-surface intelligence.

## Where your territory is stronger than what these companies publicly say

This is the most important comparison.

These companies are mostly publishing:

- interaction patterns
- platform capabilities
- design-system updates
- developer guidance
- product behaviors

Your positioning is stronger when it moves one level up and says:

- the real design problem is not only the AI interaction
- it is the **system of trust around the interaction**
- that system includes the internal team building it, the organization deploying it, the safeguards surrounding it, and the customer deciding whether to rely on it

That distinction matters because none of these companies, in their public design guidance, fully owns the whole internal-to-external trust chain the way you do.

### Apple vs your territory

Apple is closest to your instincts on restraint, integration, and user impact. But Apple's public posture is still platform-centric. It tells developers how to make AI feel coherent inside Apple systems. Your territory can go further by naming the organizational and behavioral conditions required for that coherence to translate into actual enterprise trust and adoption.

### Google vs your territory

Google contributes some of the richest public thinking on AI interaction and human-centered patterns. But much of it still lives at the level of interface language, design method, or new form factors. Your territory is stronger when it connects those patterns to leadership, capability-building, and enterprise operating conditions.

### Meta vs your territory

Meta is making interesting moves around continuity, voice, personalization, and glasses. But its public design language is still lighter on governance and trust architecture. Your point of view can be sharper here by articulating what happens when personal, persistent, socially shaped AI enters environments where trust calibration and human boundaries are weak.

### Microsoft vs your territory

Microsoft overlaps with you the most in explicit terms: trust, handoffs, control, governance, and adoption. The difference is that Microsoft's public language is still largely implementation- and platform-oriented. Your territory can stay differentiated by holding together both sides of the wall:

- what internal teams need in order to build trustworthy AI well
- what end users need in order to adopt and rely on what gets shipped

## Positioning implications for you

### Core claim that keeps getting stronger

The barrier to building agents is dropping. The barrier to building **trusted, adoptable, coherent AI experiences** is not.

That means your value is not "I understand AI UX." It is closer to:

**I design the trust layer that turns AI capability into human adoption and organizational value.**

### Sharper framing options

You could increasingly frame your territory around a few distinctions:

- **From interface design to relationship design.**  
  The system is no longer static; the human is learning the machine while the machine learns the human.

- **From feature delivery to trust architecture.**  
  The key problem is not whether the model can act, but whether the surrounding conditions make its action legible, governable, and worth relying on.

- **From AI rollout to organizational experience redesign.**  
  Agentic capability changes work rhythms, authority boundaries, skill requirements, and escalation paths. That is an organizational design problem, not just a product problem.

- **From intelligence to adoption.**  
  As the technology gets easier to deploy, the competitive edge shifts toward the teams that can create sustainable trust, better handoffs, and less judgment erosion.

## Design leadership problems this creates

These companies are all implicitly pointing at problems a design leader could help solve:

- How should AI show its work enough to support trust without creating noise?
- When should systems guide, ask, hand off, or act autonomously?
- How do you make refinement feel natural instead of like error recovery?
- How do you preserve human judgment when systems get more capable and more ambient?
- How do you design continuity across surfaces without making the system feel invasive?
- How do you align builder tooling, governance, and customer experience so trust is not broken upstream?

That last question is the one your territory owns best.

## Bottom line

If you keep writing into this territory, the strongest synthesis is:

The major platforms are converging on AI as a contextual, persistent, multi-surface system that needs better handoffs, better refinement loops, and better trust signals. But their public guidance is still mostly about product behavior and platform enablement. Your territory becomes more valuable when you name the missing layer: the organizational, experiential, and trust conditions that determine whether AI creates real human value or just more technically impressive instability.

## Sources

### Apple

- [Apple Design: What's New](https://developer.apple.com/design/whats-new/)
- [Apple Intelligence overview](https://developer.apple.com/apple-intelligence/)
- [What's new in Apple Intelligence](https://developer.apple.com/apple-intelligence/whats-new/)
- [Apple HIG: App Shortcuts](https://developer.apple.com/design/human-interface-guidelines/app-shortcuts)
- [Apple HIG: Generative AI](https://developer.apple.com/design/human-interface-guidelines/generative-ai)
- [Apple Design Resources](https://developer.apple.com/design/resources/)
- [SF Symbols 8](https://developer.apple.com/sf-symbols/)

### Google

- [Google Design: Illustrating the Gemini App](https://design.google/library/gemini-ai-visual-design)
- [Google Design: Designing for Transparent Screens](https://design.google/library/transparent-screens)
- [People + AI Guidebook](https://pair.withgoogle.com/guidebook-v2/)
- [Android Developers: AI glasses](https://developer.android.com/design/ui/ai-glasses)

### Meta

- [Meta: Introducing the Meta AI App](https://about.fb.com/news/2025/04/introducing-meta-ai-app-new-way-access-ai-assistant/)
- [Meta Design: Designing AI products that are future-facing and familiar](https://design.facebook.com/blog/4-principles-for-designing-AI-products/)

### Microsoft

- [Fluent 2: Responsible AI](https://fluent2.microsoft.design/responsible-AI)
- [Fluent 2: Handoffs](https://fluent2.microsoft.design/handoffs)
- [Fluent 2: Start designing](https://fluent2.microsoft.design/get-started/design)
- [Microsoft Learn: UX guidelines for MCP apps in Copilot](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/plugin-mcp-apps-ui-guidelines)
- [Microsoft Learn: Use the agent design framework](https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/agent-design-canvas-framework)
- [Microsoft Design: The new Microsoft 365 Copilot mobile experience](https://microsoft.design/articles/the-new-microsoft-365-copilot-mobile-experience/)
