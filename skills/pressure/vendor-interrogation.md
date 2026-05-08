---
name: vendor-interrogation
description: Generate the questions that cut through an AI vendor's demo or proposal. Use before or after a vendor meeting to surface what the vendor didn't answer — and what you should have asked. Triggers on phrases like "we have a vendor meeting about AI", "they're demoing their AI product", "I need to evaluate an AI vendor", "what should I ask them", "how do I know if their AI is real".
---

# Vendor Interrogation

AI vendor meetings are structured to answer questions you didn't ask. The demo is designed to produce confidence in conditions that favour the vendor. The ROI case is built on assumptions you haven't examined. The timeline is optimistic about your organisation's readiness.

This skill generates the questions that rebalance the meeting — the ones that are rarely asked, and whose answers most reliably separate genuine capability from performance.

---

## Step 1: Brief Claude on the Vendor

Before generating the questions, provide:

- What does this vendor claim their AI system does?
- What problem in your organisation are you considering it for?
- What stage are you at — pre-demo, post-demo, or evaluating a proposal?
- What have they already told you, if anything?
- What is the rough scale of the potential engagement — pilot, department, enterprise?

---

## Step 2: Interrogation Questions

Claude will tailor these to your context. The base questions are organised by the moment in which they're most powerful.

### Questions to Ask Before They Start the Demo

These frame the conversation on your terms rather than theirs.

1. "Before you show us anything — can you describe a customer deployment that failed, or didn't deliver its projected value? What happened?"
   *Why*: A vendor who can describe failure credibly is more trustworthy than one who cannot. Watch for specificity vs vagueness.

2. "What is the most common reason organisations buy your product and don't get the value they expected?"
   *Why*: This question is harder to deflect than "what are your risks?" It asks for their knowledge of their own failure patterns.

3. "We'll be running this on [describe your data environment]. What would you need to know about our data before telling us whether this would work?"
   *Why*: Forces them to engage with your specific context. A vendor who doesn't ask follow-up questions here is not thinking about your deployment — they're thinking about the demo.

---

### Questions During the Demo

4. "Can you show us what happens when the input is ambiguous or low quality?"
   *Why*: Demos are curated for clean inputs. The behaviour on messy inputs is what you'll live with.

5. "What does the system output when it doesn't know the answer? Can you show us that?"
   *Why*: Hallucination behaviour is critical. If they can't demonstrate it, they haven't stress-tested it.

6. "Who on your team is responsible for this deployment if we go ahead — and are they in this room?"
   *Why*: Separates sales capability from delivery capability. If the answer is "our implementation team," ask to meet them.

---

### Questions After the Demo

7. "The ROI figure you've shared — which customer is it based on, and can you connect us with their operations lead?"
   *Why*: Reference calls with procurement or IT are structured. Operations leads tell you what actually happened.

8. "What is the data preparation effort on our side, realistically? In person-weeks, not a range."
   *Why*: Data preparation is the most consistently underestimated part of AI deployments. Forcing a number reveals whether they've thought about your context.

9. "If we sign and the deployment isn't delivering value at six months, what does the contract say?"
   *Why*: The answer reveals where they think the risk lives. "We'll work with you" is a theatre answer. A substance answer describes specific exit or remediation provisions.

10. "What is our data portability situation — if we leave, what do we take with us and in what format?"
    *Why*: This tells you how locked-in they expect you to be, and whether they've thought about it from your perspective.

11. "Can you describe the integration with [your current system] concretely — not at the API level, but at the workflow level? Who changes what behaviour?"
    *Why*: Integration depth is almost always understated. The answer surfaces the adoption surface they haven't accounted for.

12. "What does your customer's team look like a year after deployment — what skills did they need to develop, and did you help them develop them?"
    *Why*: Reveals whether they treat the deployment as a technology event or an organisational change.

---

### Questions to Save for the End

13. "If we don't buy this — what's the strongest reason we'd regret it in 18 months?"
    *Why*: You want to hear their genuine conviction, unmediated by sales structure. Listen for specificity.

14. "What's the one thing about your product that you'd want to improve most, that you're actively working on?"
    *Why*: A vendor who can answer this is engaged with the reality of their product. One who cannot is in performance mode.

---

## Step 3: After the Meeting

Run the [ai-theatre-detector](../ai-theatre-detector/SKILL.md) skill on what you heard.

Specifically note:
- Which questions produced specific, grounded answers
- Which questions produced pivots, generalities, or deferred commitments
- Which questions they answered before you finished asking them (rehearsed answers signal which questions they expect — and which they've structured the pitch to pre-empt)

---

## Principle

*The vendor is a professional at this conversation. You are not. The questions that make the meeting uncomfortable for them are the ones that produce the most useful information for you.*

Ask the uncomfortable questions. The relationship can survive it. A failed deployment cannot.
