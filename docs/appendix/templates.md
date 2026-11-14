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
