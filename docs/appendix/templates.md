# Templates

Copy-paste templates for everyday PM work. More are added as chapters are written.

## Metric definition card

Use this whenever you add a metric to a dashboard. It stops two teams from measuring "active user" in two different ways. See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

```text
Metric name:
One-line meaning (plain English):
Exact formula:
Counted when (event/trigger):
Time window (daily / weekly / 28-day):
Who is included / excluded:
Type: leading or lagging · input or output
Owner (team/person):
Counter metric to watch alongside it:
Where it lives (dashboard link):
```

## Metric drop investigation

A checklist for when a key number suddenly falls. See [A8.6](../part-a/08-product-metrics/06-diagnosing-a-metric-drop.md).

```text
1. What exactly dropped? (metric, by how much, since when)
2. Is it real? (tracking change, data pipeline, dashboard bug, definition change)
3. Internal or external? (our releases, experiments, pricing vs. season, holidays, competitors, outages, news)
4. Where is it concentrated? (platform, app version, country/city, new vs. old users, channel)
5. Which step of the funnel moved?
6. Best hypothesis + evidence for and against
7. Next action + owner + when we'll check again
```

## User session debrief note

Fill this in within 24 hours of any interview or observation. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

```text
Who (segment, not name):           Date / place / format:
Context (where, when, with whom, under what pressure):
What they did (observed, step by step):
Quotes (their exact words):
Surprises (what didn't match our assumptions):
Candidate insight (a non-obvious truth that points to a decision):
How common might this be? How will we check?
Open questions for next session:
```

## System prompt spec

A one-page spec for any AI feature's system prompt. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

```text
Job (one sentence):
Users and their context:
Success criteria (3-5, measurable):
Role and goal:
Rules, each with a reason:
Examples (2-5, varied in topic, length, language, mood):
Input data and how it's tagged:
Output format (and how code validates it):
When unsure / out of scope, the model should:
Hard limits enforced in code, not the prompt:
Eval set (link, size, last score):
Model + version, token count, est. cost per 1,000 calls:
Owner, version, change log:
```

## Interview discussion guide

A one-page plan for a 30–45 minute story-based interview. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

```text
Decision this research informs:
Research question:
Who (segment, defined by behaviour):        Interviewer / note-taker:
Consent and recording script:

1. Warm-up (3-5 min)
   - Tell me a bit about yourself and your day-to-day ...
2. The story (15-20 min)
   - Tell me about the last time you ...  (walk through it step by step)
3. Dig deeper (10-15 min)
   - What happened next? / What was hardest about that?
   - What did you try instead? / Can you show me?
4. Wrap-up (3-5 min)
   - Is there anything I should have asked but didn't?
   - Who else should we talk to?

Neutral probes: "Tell me more about that." "Why was that?" "What did you do then?"
Assumptions we are testing (write before sessions):
Stop rule (e.g. two sessions in a row with nothing new):
```

## RAG knowledge-base checklist

Decisions to settle before building an AI assistant over your documents. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

```text
Job and top 30-50 real user questions (source):
Size of knowledge (tokens) — under ~200k? consider no retrieval:
Sources in / out, owner of each, review date:
Which source wins when two disagree:
Freshness needed (minutes / daily / weekly) and re-index trigger:
Access rules: who may see which documents (filtered before retrieval):
Live data that needs a tool call instead (orders, balances):
Golden set: size, owner, last run date:
Targets: recall@k, faithfulness, correct-answer rate, "I don't know" rate:
Citations shown to users (link, quoted passage):
Fallback when nothing is found (human handoff):
Counter metrics (repeat contacts, thumbs-down, uncited answers):
Cost per answer and latency budget:
```

## Persona and job story card

A one-page summary of a user type and their top jobs. Every line should trace back to research, or be marked "assumption". See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

```text
Persona name and one-line summary:
Research behind it (interviews, data, date):
Context (device, place, time, who else is involved):
Goals:
Current behaviours and workarounds:
Frustrations (in their words):
One real quote:

Top jobs (2-3), each as:
  When [situation], I want to [motivation], so I can [outcome].
  Functional / emotional / social layers:
  Push:            Pull:
  Anxiety:         Habit:
  Real alternatives they "fire" to hire us:
  Desired outcomes (how they judge "done well"):

Not this persona (anti-persona notes):
Last reviewed:
```

## Agent design canvas

Decisions to settle before building an AI agent. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

```text
Job and definition of done:
Could a fixed workflow do it? (if yes, build that):
Tools (name, purpose, read/write, what it returns):
Autonomy per write action (suggest / draft / approve / act-and-report / autonomous):
Approval thresholds (e.g. refunds over Rs 1,000):
Rule of Two: untrusted input? private data? external actions? Mitigation if all three:
Limits: max steps, max cost per task, time limit:
Hand-off to human: when, and what summary they see:
Reversibility: undo, backups, staging for destructive actions:
Credentials and permissions (whose identity, what scope):
Eval set: size, source, runs per case, last run date:
Metrics: end-to-end success, wrong-action rate, cost and time per task:
Guardrails: complaints, repeat contacts, reversals:
Rollout plan (narrow start, criteria to widen):
Audit log location and owner:
```

## Journey map canvas

Use this for a current-state journey map of one actor in one scenario. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

```text
Actor (one user type):
Scenario and goal (one sentence):
Expectations (what they expect to happen):
Evidence used (interviews, funnel data, tickets, reviews, dates):

For each phase (5-7 phases, include offline and assisted steps):
  Phase:
  Touchpoints (screen, SMS, call, person, paper):
  Does:
  Thinks (real quotes where possible):
  Feels (-2 to +2, with evidence):
  Data (users reaching this step, drop-off %, tickets):
  Evidence or assumption?:
  Backstage (staff, processes, systems behind this step):

Moments that matter (2-3 biggest lows, plus the ending):
Opportunities (one per low):
  Opportunity:
  Owner:
  Metric that shows it improved:
  Estimated value and effort:
Riskiest assumptions to check next:
Next review date:
```

## Fine-tuning decision checklist

Run this before approving a fine-tuning project. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

```text
Task (narrow, stable, one sentence):
Eval set: size, source, who checked the answers:
Prompt baseline score (best prompt, strong model):
Break-even accuracy (value of right answer vs cost of wrong one):
Failure labels (count of 50-100 failures):
  Knowledge (missing, old or private facts) -> RAG or tools:
  Behaviour (format, tone, category mix-ups) -> prompt fixes, then fine-tune:
  Cost or speed -> caching, cheaper model, then fine-tune or distil:
All four true? behaviour problem / prompt gains stalled / task stable / enough good examples:
Volume per month:
Cost per call now (with caching) vs expected after fine-tuning:
Upfront cost (labelling, training, engineering):
Upkeep (retraining per year, hosting):
Payback period:
Data: consent, personal data removed, deletion plan:
Platform: can we export weights? base-model retirement date?:
Fallback (prompt-only version) ready?:
General-skills eval slice and A/B rollout plan:
```
