---
name: ai-theatre-detector
description: After a vendor pitch, internal proposal, or board presentation on AI — run this skill to distinguish genuine capability from performance. Use when an executive has just seen an AI demo, received an AI proposal, or is evaluating an AI initiative and wants to know whether what they saw was real. Triggers on phrases like "we just had a vendor in", "our team presented an AI pilot", "the board wants us to do X with AI", "I'm not sure if this is real".
---

# AI Theatre Detector

Your job is to help the executive run a structured diagnostic on an AI claim they've just encountered — a vendor pitch, an internal proposal, or a board-level initiative. The goal is a calibrated verdict: genuine capability, probable theatre, or insufficient information to judge.

This is not skepticism for its own sake. Many AI capabilities are real. The discipline is in distinguishing which ones, and on what evidence.

---

## Step 1: Get the Claim

Ask the executive to describe, in their own words, what they were shown or told. Specifically:

- What did the AI system do in the demo or proposal?
- What problem was it claimed to solve?
- What numbers were attached to it — speed, accuracy, ROI, cost savings?
- Who presented it, and in what context?

Do not editorialize yet. Just capture the claim precisely.

---

## Step 2: Run the Theatre Diagnostic

For each dimension below, ask the executive what they know. Where they don't know, flag it — absence of information is itself diagnostic.

### Data Provenance
- Was the demo run on real production data, or on a curated dataset?
- If it was real data, whose data was it — the vendor's reference customer, or yours?
- Was the data volume representative of your actual operating scale?

*Theatre signal*: Demo data was clean, pre-formatted, or belonged to a reference customer in a different industry or scale.
*Substance signal*: Demo was run on a sample of your actual data, or vendor clearly described the data preparation required for your context.

### Failure Mode Disclosure
- Did the presenter describe conditions under which the system produces wrong output?
- Did they describe what happens when it fails — who notices, and what the recovery process is?
- Was there any discussion of edge cases, exceptions, or known limitations?

*Theatre signal*: Accuracy figures given without a denominator. No discussion of failure. "It's continuously improving" offered as the failure mode response.
*Substance signal*: Specific failure modes named. A human-in-the-loop described for high-stakes outputs. Error rate discussed alongside accuracy rate.

### Process Ownership
- Is there a named individual on their side who owns the integration?
- Is there a named individual on your side who would own the workflow once deployed?
- Was there a discussion of what your operations team would need to do differently?

*Theatre signal*: Integration described as a handoff — "your IT team implements it." No discussion of change management.
*Substance signal*: A specific implementation owner named. Change management scoped, even roughly.

### ROI Attribution
- Where did the ROI figure come from?
- Is it based on a deployment in your sector, at your scale, with comparable data quality?
- Does it assume a before/after comparison with a named baseline?

*Theatre signal*: ROI figure from a press release, a different industry, or "industry average." No baseline described.
*Substance signal*: ROI tied to a specific customer deployment with a named metric and a measurement period.

### Timeline Realism
- What is the proposed time from contract to value?
- Does this timeline include data preparation, integration, training, and change management?
- Who bears the timeline risk — the vendor or your organisation?

*Theatre signal*: Timeline assumes smooth data availability and internal cooperation. Risk sits entirely with the client.
*Substance signal*: Timeline accounts for your data readiness. Pilot phase with clear go/no-go criteria described.

### Exit Clarity
- What happens if you want to stop using the system in 12 months?
- Is your data portable?
- What is the contractual exit path?

*Theatre signal*: No exit discussion. Data portability not mentioned.
*Substance signal*: Data portability confirmed. Exit terms discussed proactively.

---

## Step 3: Produce the Verdict

Based on the executive's answers, produce a structured verdict:

**Theatre Score**: High / Medium / Low / Insufficient information

**Evidence for the score**: Two or three specific observations from the diagnostic — what was present, what was absent.

**The one question to ask before any further engagement**: Based on the most significant gap in the diagnostic, identify the single question that would most change your assessment if answered well.

**Recommended next step**: One of:
- *Proceed to detailed scoping* — the capability appears genuine; the next step is a proper technical and operational assessment
- *Request a production pilot* — the claim has potential but needs validation against your actual environment
- *Pause and request evidence* — specific evidence needed before any further time investment
- *Decline* — the signals are sufficiently negative that the opportunity cost of continued engagement is not justified

---

## Principles for This Diagnostic

**Absence of information is diagnostic.** A vendor who hasn't addressed failure modes hasn't addressed them — that's a data point, not a gap to fill charitably.

**Optimism is not dishonesty.** Most AI theatre comes from genuine belief in capability that hasn't yet been stress-tested operationally. Treat it as a calibration problem, not a character problem.

**The demo is not the product.** The relevant question is never "did this work in the demo?" It is always "what would have to be true about my organisation for this to work here?"

**Your seniority is a liability in this room.** Presenters optimise for the most senior person. The questions nobody asks in front of you are the ones your team asks afterward. Build in a separate channel for that.
