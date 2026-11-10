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
