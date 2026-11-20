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

## Opportunity solution tree (text version)

Keep this in a shared doc and update it weekly. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

```text
Desired outcome (metric, baseline -> target, by when):
Opportunities (customer's words; children are smaller parts of parents):
  - Opportunity A
      - Sub-opportunity A1
  - Opportunity B
Target opportunity (and why: size, market, company, customer factors):
Solutions (at least 3):
  1.
  2.
  3.
Riskiest assumptions per solution (desirability / viability / feasibility / usability / ethical):
Tests (method, sample, success criterion written BEFORE running, result, decision):
Last updated:
```

## AI opportunity fit check

Run this on any proposed AI feature. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

```text
User and task:
How it's done today, and what it costs (time, money, drop-off):
Volume per day/month:
Simpler answer (rules, better form, UI fix)? Would it cover most cases?:
Why AI (messy input? too many cases for rules?):
Cost of a wrong answer (low / medium / high) and who is harmed:
How easy is it to check the output, and who checks?:
Risk zone: sweet spot / monitor / augment / danger:
Automate or augment, and why:
Data and context the model needs at run time; permission to use it:
Value per task:
AI cost per task + checking cost + build and upkeep:
Break-even accuracy:
Prototype eval result (n = ___ real examples):
Guardrails (human approval, audits, fallback):
Go / no-go date and criteria:
```

## Problem statement card

Fill this in before any significant piece of work, and put it at the top of the PRD. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

```text
Request as received (if any):
Stakeholders' written definitions (one line each):
Who (specific segment):
Situation (when / where it happens):
Struggle (what goes wrong for them):
Cause (we believe... because...; what would prove it wrong):
Evidence and size (data + quotes; reach x frequency x severity):
Impact and measure (outcome metric: baseline -> target, by when):
Reframes tried (what's left out? when doesn't it happen? is the objective right?):
How might we... (3-5 questions; circle 1-2):
Out of scope (other causes or segments we're not tackling):
Agreed by (trio + stakeholders), date:
```

## AI pattern and autonomy plan

Use this when choosing how users will meet an AI feature. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

```text
User and task:
Who knows the work is needed (user / product can see it):
One step or many:
Cost of a mistake; reversible?:
How easy is checking, and who checks:
How often it happens:
Chosen pattern (chat / copilot / agent / ambient, or a mix) and why:
Autonomy per action (act silently / act then show / draft for review / ask every time):
  - Action 1:
  - Action 2:
  - Action 3:
Trust signals (sources, reasons, plan, log, undo):
Consent and data access (what is watched; default on/off; how to switch off):
Latency target:
Steering metric, outcome metric, guardrails (edit rate, opt-outs, wrong actions):
How users move up or down the autonomy ladder:
```

## Assumption test card

Use one card per risky assumption, filled in before the test runs. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

```text
Idea (one sentence):
Assumption (We believe that...):
Type (desirability / viability / feasibility / usability / ethical):
Why it's risky (importance; evidence so far):
Test (cheapest test that could prove it wrong):
Who (which users, how many, which channel):
Metric (behaviour or commitment, not opinion):
Success threshold (set now; go / iterate / stop zones):
Cost and time:
Ethics check (honest to users? no money taken for nothing?):
Result:
Learning (We observed... so we learned... so we will...):
Decision (persevere / pivot / stop) and next riskiest assumption:
```

## Trust and failure plan

Use this for any AI feature that can affect money, health, legal rights or customer trust. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

```text
Feature and users (experts or novices? languages?):
Failure inventory (top 5-10):
  - Failure | how often (evals) | harm | would the user notice?
Actions and oversight level (automate / preview / undo + audit / human approves):
  - Action 1:
  - Action 2:
Routing rule (stakes first, then confidence threshold):
Trust signals (AI label, sources, uncertainty wording, stated limits):
Recovery (undo, edit, preview; graceful-failure messages and next steps):
Human handoff (triggers incl. emotion; context passed; promised reply time):
Feedback capture and where it goes (eval set, weekly review):
Oversight health metrics (reviewer agreement, override rate, canary catch rate, audit error rate):
Regulatory checks (disclosure, right to challenge, incident reporting):
```

## Eval plan

Use this before launching or changing any AI feature. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

```text
Feature and quality owner:
Quality bar (3-5 sentences: what great looks like, what must never happen):
Traces reviewed (how many, from where, which languages/user types):
Failure modes (from error analysis):
  - Failure | count in sample | harm (high/med/low) | grader (code / AI judge / human)
AI judge check (labelled cases | failures caught % | passes correct %):
Eval set (real failures | typical | edge/adversarial) and trials per case:
Launch thresholds (set before running):
  - Check | bar
Run on: every prompt/model change | weekly trace review owner:
Online signals to watch after launch:
```

## Outcome statement card

Use this to turn a feature request into an outcome. See [A2.4](../part-a/02-problem-discovery/04-outcomes-over-outputs-escaping-the-build-trap.md).

```text
Request as received (the output):
Direction it serves (company strategy):
Who (which customers or users):
Does what (observable behaviour):
From ___ to ___ (current value and target):
By when:
Leading indicator we can check within 4 weeks:
Evidence the behaviour drives business results:
Cheapest ways to move it (at least one that isn't a feature):
Guardrail metric:
When we'll check results after launch:
```
