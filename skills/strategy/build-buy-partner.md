---
name: build-buy-partner
description: Help an executive think through whether to build AI capability internally, buy it from a vendor, or access it through a partnership. Use when an executive is facing a specific AI capability decision and needs a structured framework to evaluate the options — not a generic make-or-buy analysis, but one calibrated to the specific dynamics of AI: rapid depreciation, vendor lock-in risk, talent scarcity, and the difference between commodity and strategic capability. Triggers on phrases like "should we build this or buy it", "do we need our own AI team", "a vendor is pitching us their AI platform", "how do I decide whether to build AI in-house", "what's the right AI partnership model".
---

# Build / Buy / Partner

The build-vs-buy question looks familiar. In AI, it is not. The dynamics are different enough that applying standard make-or-buy reasoning produces systematically wrong answers.

The specific distortions in AI:

- **Capability depreciates faster than almost any prior technology.** What you build today may be commoditised by a foundation model update in 18 months. The case for building is weaker than it looks when the capability is moving toward commodity.
- **Vendor lock-in is structurally deeper.** AI systems embed in data pipelines, workflow design, and staff behaviour in ways that are hard to reverse. The switching cost of a bad vendor decision is higher than a bad software decision.
- **"Build" requires talent you probably can't hire or retain.** Genuine AI engineering talent is scarce and expensive. The talent required to build a real AI capability is not the same as the talent required to use one. Many "build" decisions are based on a misread of what building actually requires.
- **"Partner" is often the least examined option.** Partnerships — with startups, research institutions, industry consortia, or adjacent businesses — can provide access to capability without the commitment of a vendor contract or the cost of a build. They are underused because they require relationship-building rather than procurement.

---

## Step 1: Define the Capability Precisely

Before evaluating options, name the capability you're deciding about with operational specificity.

Answer:

- What specific task or workflow would this AI capability perform?
- Who would use it, in what volume, and with what frequency?
- What is the decision quality or efficiency improvement you're trying to achieve?
- What does success look like at 12 months — specifically, what would be measurably different?

A vague capability definition produces a vague build-buy-partner analysis. "AI for our customer service function" is not specific enough. "AI-assisted triage of inbound customer complaints, with human escalation for anything above a defined complexity threshold, targeting a 40% reduction in first-response time" is.

---

## Step 2: Assess the Capability Dimensions

For the specific capability you've defined, assess across four dimensions.

### Strategic Centrality

Is this capability core to your competitive differentiation, or is it operational infrastructure?

**Core / differentiating**: The capability embeds proprietary data, institutional knowledge, or customer relationships that competitors cannot replicate. The way you do this thing is part of why customers choose you.

**Operational / commodity**: The capability is table stakes — necessary but not differentiating. Competitors need it too, and the way you do it is not a competitive advantage.

*Build-buy-partner implication*: Commodity capabilities should almost never be built. The economics are wrong and the strategic return is zero. Core capabilities warrant a serious build conversation — but only if you have the talent and data to build something genuinely differentiated.

### Data Advantage

Do you have proprietary data that would make a built capability materially better than a bought one?

**High data advantage**: You have years of labelled, structured, domain-specific data that no vendor has access to. A model trained on your data would outperform a general model on your specific tasks.

**Low data advantage**: Your data is similar to what vendors have already trained on. A general model, fine-tuned or prompted appropriately, would perform comparably to a purpose-built one.

*Build-buy-partner implication*: If your data advantage is low, the build case collapses for most use cases. The marginal gain from a custom build rarely justifies the cost when a vendor model will perform at 85-90% of the ceiling.

### Talent Availability

Do you have — or can you realistically acquire and retain — the talent required to build and maintain this capability?

This is not about having engineers. It is about having the specific combination of ML engineering, domain expertise, data engineering, and product thinking required to build an AI capability that improves over time rather than decaying.

**Realistic**: You have identifiable people, a credible hiring path, and a retention environment that would keep them.

**Unrealistic**: You are competing for talent with organisations that can offer more money, more interesting problems, and better infrastructure. The people who could build this for you have better options.

*Build-buy-partner implication*: Most large organisations overestimate their ability to hire and retain genuine AI talent. The honest assessment of talent availability is the most common place where build decisions go wrong.

### Lock-in Tolerance

How exposed are you if the vendor relationship sours, the product is deprecated, or the pricing changes materially in 24 months?

**Low tolerance**: This capability will be embedded in core operations, your data will be processed by the vendor's systems, and switching would require significant re-engineering. You are making a multi-year commitment.

**High tolerance**: The capability is peripheral, the data exposure is limited, and switching would be disruptive but survivable. You retain genuine optionality.

*Build-buy-partner implication*: Low lock-in tolerance raises the threshold for a buy decision significantly. It also shapes the contract terms you should insist on: data portability, exit provisions, price caps.

---

## Step 3: Map to the Decision

Based on the four dimensions, the decision matrix looks like this:

| Strategic Centrality | Data Advantage | Talent Available | Lock-in Tolerance | Default Recommendation |
|---|---|---|---|---|
| Core | High | Yes | Any | **Build** — with clear scope and exit criteria |
| Core | High | No | Any | **Partner** — with a specialist who has the talent, using your data |
| Core | Low | Any | High | **Buy** — with careful vendor selection and contract terms |
| Core | Low | Any | Low | **Partner or selective build** — vendor risk too high for core capability |
| Commodity | Any | Any | High | **Buy** — fastest path to capability, no strategic return on building |
| Commodity | Any | Any | Low | **Buy with strong exit provisions**, or **Partner** for lower commitment |

This matrix is a starting point, not a verdict. The dimensions interact and the specific numbers matter.

---

## Step 4: Evaluate the Partner Option Properly

Partnership is the most underexamined option and often the most appropriate one for the current moment — when AI capability is moving fast, vendor lock-in is high, and genuine build capability is scarce.

Partnership models worth evaluating:

**Startup partnership**: Access to cutting-edge capability in exchange for a reference customer relationship, early access pricing, or co-development input. Works when the startup has the specific capability you need and you have the market credibility they need. Risk: startup failure or acquisition.

**Research institution partnership**: Access to academic AI capability and talent pipelines in exchange for funding, data access, or deployment context. Works for longer-horizon capability development. Risk: slower timelines, IP complexity.

**Industry consortium**: Shared development of pre-competitive AI infrastructure with peers in the same sector. Works when the capability is needed by multiple organisations but not differentiating for any of them. Risk: governance complexity, slowest path to capability.

**Systems integrator partnership**: A large consultancy or technology services firm builds and maintains the capability on your behalf, using vendor tools. Works when you lack internal talent but need a managed outcome rather than a product. Risk: dependency, cost, and the integrator's incentives may not align with yours.

For each option, assess: who has leverage in the relationship, what happens when it ends, and what you own at the conclusion.

---

## Step 5: Produce the Recommendation

Produce a structured recommendation:

**The capability** (one sentence, operational)

**The assessment** (one paragraph): Where the capability sits on the four dimensions, and what that implies.

**The recommended path** (build / buy / partner / hybrid): With specific reasoning tied to the dimension assessment — not generic principles.

**The conditions**: What would have to be true for this recommendation to be wrong? What signal would cause you to revise it in 12 months?

**The immediate next step**: One specific action — a vendor shortlist, a conversation with a potential partner, a talent audit, a data assessment — that moves the decision forward.

---

## Principles

**The build case is almost always weaker than it looks.** The talent required, the time to value, and the pace of capability commoditisation all conspire against it. Build when you have genuine data advantage and genuine talent. Otherwise, the pride of ownership is not worth the cost.

**The buy case is almost always riskier than it looks.** Lock-in in AI is deeper than in conventional software. The contract you sign today governs a relationship that will shape your operations for years. Negotiate it accordingly.

**Partnership is not a compromise.** It is often the option with the best risk-adjusted return — especially in the current moment, when the capability frontier is moving too fast for most organisations to track internally, and vendor lock-in is too costly for most operations to absorb comfortably.

**Revisit in 12 months.** A build-buy-partner decision made today is not permanent. The capability landscape, your talent situation, and the vendor market will all change. The decision should have an explicit review trigger.
