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
