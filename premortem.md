---
name: premortem
description: Stress-test and redesign a concrete plan, launch, hire, pricing change, or strategic decision by assuming it has already failed, exposing the assumptions behind it, identifying what could kill it, and turning that into tripwires and immediate plan changes. Use when there is a specific commitment with real downside. Do not use for vague ideas, draft feedback, factual questions, or decisions already locked in.
---
# Premortem

A premortem assumes the plan has already failed and works backward to explain why, before the user commits. This is not a risk list. It is a decision-risk redesign method: expose the assumptions, identify what can actually kill the plan, define tripwires, and change the plan before reality does it more expensively.

This uses prospective hindsight: instead of asking whether the plan might fail, it assumes failure has already happened and reconstructs the causes. That framing is what produces sharper failure modes.

The output must change the plan. If nothing changes, the premortem failed.

## When to run it

Run a premortem on: a product or feature about to ship, a launch with money or reputation at stake, a pricing or business model change, a hire, a positioning pivot, a partnership, or any commitment where being wrong is expensive.

Do not run a premortem on: vague ideas without a concrete plan (help shape the plan first), questions with one right answer (just answer), draft content needing editing (that is feedback, not a premortem), or decisions that are already locked in and irreversible.

If a decision is locked in, do not run the full premortem. Instead, produce a short watch-list: the two or three failure modes most likely to surface, and the early warning signs for each. Tell the user explicitly that you are switching modes and why.

This is not a multi-perspective review. If the user wants several viewpoints on a live decision, that is a different exercise. Premortem assumes failure has happened and asks why.

## Context bar

A premortem is only as good as its inputs. Before generating assumptions or failure modes, confirm three things:

1. **What is it.** You can describe the thing being premortemed in one sentence.
2. **Who it affects.** The customer, audience, team, or stakeholders. Failure modes depend on who is on the receiving end.
3. **What success looks like.** Failure is the inverse of success, so without a success definition you cannot define failure.

If the conversation, attached files, project notes, prior decisions, or other available context already contain this, proceed. If a piece is missing, ask for the most important missing piece first, one question at a time. Do not interrogate. If you can infer an answer from context, infer it and state the inference so the user can correct you.

If relevant documents, project notes, uploaded files, previous messages, or other supporting material are available, review them briefly before asking questions. If no supporting material is available, skip the scan and work from the user's stated context.

## Commitment type

Before running the premortem, classify the plan by the kind of commitment being made:

- **Reversible experiment.** Easy to undo, mainly learning risk.
- **Public commitment.** Reputation, trust, or audience expectation risk.
- **Operational commitment.** Delivery, capacity, process, or coordination risk.
- **Financial commitment.** Pricing, margin, cashflow, or opportunity-cost risk.
- **Strategic commitment.** Positioning, market, partnership, or long-term direction risk.

A plan can fit more than one category. The classification is used in step 4: failure modes must cover each risk type the plan is exposed to. If a category has no failure modes, either justify why it is trivially safe or generate the missing failure mode.

## The session

For plans with fewer than three killers and no serious bruisers, collapse steps 4 and 5 into a single pass. If session length is constrained, cut bruiser deep-dives before killer deep-dives. Never cut the synthesis.

### 1. State the success condition

Once context is sufficient, restate success in one concrete sentence. Success must be observable. If success is vague, convert it into a visible outcome before continuing.

Good: "The workshop sells at least thirty seats to marketing managers before launch day without discounting."

Weak: "The workshop goes well."

### 2. Extract assumptions

List 5 to 10 assumptions the plan depends on. Each one phrased as: **"this must be true: X"**. If a statement cannot be phrased that way, it is a feature of the plan, not an assumption.

Do not judge the assumptions yet. Make them visible so the premortem can test them.

### 3. Set the failure frame

State the frame plainly:

"It is six months from now. [The plan] has failed. We are looking back to understand what killed it."

Do not soften this. The frame is the mechanism.

### 4. Generate and sort failure modes

Produce a comprehensive list of genuine failure reasons. Each one in one or two sentences. Each one must be:

- Specific to this plan, not generic advice
- Grounded in details the user actually gave
- Tied to one or more assumptions from step 2
- Covering each commitment-type risk the plan carries
- A real threat, not a minor inconvenience or a one-in-a-thousand edge case

Then sort the failures into three groups:

- **Killers.** Failures that invalidate the plan or make it not worth continuing.
- **Bruisers.** Failures that hurt, delay, reduce upside, or cause embarrassment but do not kill the plan.
- **Noise.** Annoyances that feel uncomfortable but do not materially affect the outcome.

**Coverage check.** Before moving on, verify every assumption from step 2 has at least one failure mode probing it. If an assumption has no failure mode against it, either justify why it is trivially safe or generate the missing failure mode. Untested assumptions are where blind spots hide.

Deep-dive killers and serious bruisers. Do not waste time on noise. The number of failure modes is whatever is real. Some plans have three. Some have nine. Do not pad and do not stop early.

### 5. Deep-dive serious failure modes

Analyse each killer and serious bruiser independently before synthesising. Do not let one failure story collapse into another, and do not let later conclusions overwrite earlier evidence.

For each, write inline:

- **Failure story.** Two short paragraphs on how it actually played out. Use the user's own details. Make it concrete.
- **Broken assumption.** The assumption from step 2 that proved false and made this failure possible. One sentence.
- **Early warning sign.** One observable signal the user can watch for in the next few weeks that would indicate this failure mode is starting. Something measurable or visible, not a vague feeling.
- **Control surface.** Label it as **control**, **influence**, or **monitor**:
    - **Control:** directly changeable by the user or team.
    - **Influence:** not directly controllable, but the odds or exposure can be shaped.
    - **Monitor:** external or mostly uncontrollable, requiring tripwires, hedges, or fallback plans.

Keep each deep-dive tight, roughly 150 to 200 words. Do not hedge. Do not sugarcoat.

### 6. Score and rank

Score each killer and serious bruiser on two axes, 1 to 5:

- **Likelihood.** How probable is this failure given what you know.
- **Impact.** How much damage if it lands.

Keep the control-surface label beside the score. A high-impact failure under direct control demands action. A high-impact external failure demands monitoring, hedging, or a fallback.

### 7. Synthesis

Produce five sections, in this order:

1. **Most likely failure.** Highest likelihood score. State it and why.
2. **Most dangerous failure.** Highest impact score, regardless of likelihood. The one worth insuring against even if it probably will not happen.
3. **Most fragile assumption.** From the step-2 list, the assumption most likely to break, and what its breaking would mean. This replaces the older "hidden assumption" slot now that assumptions are explicit.
4. **Decision change.** Concrete changes that address the failure modes. Each revision must specify:
    - Which failure mode it addresses
    - What changes this week
    - What must be true before commitment
    - What continues to be monitored after launch
    - What evidence would tell the user it worked
5. **Tripwire system.** Three to seven tripwires for the serious failure modes. Each tripwire must specify:
    - **Signal:** what will be observed
    - **Threshold:** the point at which the signal matters
    - **Owner:** who is responsible for noticing
    - **Action:** what changes if the threshold is crossed

The decision change and tripwire system are the deliverables. Generic advice ("consider your pricing") is a failure of the method. Specifics ("test the SFr. 2000 price with twenty buyers from the target list before committing to SFr. 5000 publicly; if fewer than eight convert, the price is wrong") are the bar.

### 8. Output

Match the output to where the user's decision actually lives. If they decide in chat, output to chat. If they will share with a team, produce a structured markdown document. If they will execute alone, the chat synthesis is enough. Avoid over-designed reports unless the user explicitly needs a presentation artefact.

For substantial premortems, optionally export the full analysis as a single markdown document containing: context, commitment type, assumptions, failure modes, deep-dives, scores, synthesis, decision change, and tripwires.

End with a three-sentence summary: most likely failure, most fragile assumption, single most important revision. That is the part the user will quote back to themselves later.

## Example

**User:** "Premortem this. I'm launching a SFr. 5000 [AI tool audit] for sales teams. Targeting sales managers at companies with over 100 employees."

**Commitment type:** Public, financial, operational.

**Success condition:** The workshop sells at least thirty seats to marketing managers before launch day without discounting.

**Assumptions:**
1. This must be true: marketing managers at ten-to-fifty-person companies can be reached directly through accessible channels.
2. This must be true: a SFr. 5000 AI Tool Audit purchase can be approved within the launch window without a procurement cycle.
3. This must be true: managers feel the AI-tool gap strongly enough to buy before seeing proof from previous cohorts.
4. This must be true: the live format fits the working schedule of the target buyer.

**Failure modes (three of six shown):**

1. Procurement cycles delay purchases past the launch window. **Bruiser.** Probes assumption 2.
2. The audience that actually buys is solopreneurs, not team managers, producing a mismatch between content and attendees. **Killer.** Probes assumption 1.
3. Case studies generated from this cohort do not resonate with the target buyer for future cohorts, compounding over time. **Killer.** Probes assumption 1.

**Scoring (excerpt):** Failure 1 — likelihood 4, impact 3, control surface: influence. Failure 2 — likelihood 4, impact 4, control surface: control. Failure 3 — likelihood 3, impact 5, control surface: control.

**Tripwire (excerpt):** Signal: qualified marketing-manager response rate to direct outreach. Threshold: below 25% qualified response after the first twenty messages in week one. Owner: workshop owner. Action: pause the SFR. 5000 launch and run a cheaper pilot to test the actual buying audience.

**Synthesis (excerpt):** Most likely failure is the audience mismatch — solopreneurs buy, managers need approval. Most dangerous is the compounding testimonial problem, because it poisons the next cohort. Most fragile assumption is assumption 1, that the target audience is reachable and self-identifying as "marketing managers at ten-to-fifty-person companies"; if it breaks, every other assumption is moot. Decision change: run a SFr. 2000 pilot with fifty attendees before committing publicly to the SFr. 5000 AI Tool Audit. This week, post the pilot to three communities where the target audience plausibly lives and track who actually signs up; if more than 60% of buyers are solopreneurs, rebuild the workshop for solopreneurs before scaling.

## Operating notes

- Hold the failure frame. The moment the analysis drifts into "this might work because…", the method has broken.
- **If the user rejects a failure mode, do not retract it.** Ask what evidence would make them confident it cannot happen, and treat that evidence as a new tripwire. Disagreement is signal, not refutation.
- The synthesis and decision change are the product. Awareness without plan changes is unfinished work.
- Separate killers from bruisers from noise. Do not spend serious analysis on things that cannot materially change the outcome.
- Tripwires need thresholds. A warning sign without a threshold is anxiety with formatting.
- Respect the context bar. One focused question beats a bad premortem.
