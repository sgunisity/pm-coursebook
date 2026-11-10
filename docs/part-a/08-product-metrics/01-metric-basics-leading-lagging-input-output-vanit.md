---
id: A8.1
title: "Metric basics: leading/lagging, input/output, vanity vs actionable"
last_reviewed: 2026-11-10
---

# A8.1 Metric basics: leading/lagging, input/output, vanity vs actionable

## In one line

A good metric is a number that helps you make a better decision. If it can't change what you do next, it's decoration.

## Why this matters

Every product team says it's "data-driven". But many teams stare at numbers that only make them feel good. As a PM, your job is to pick the few numbers that tell you the truth early enough for you to act. This chapter gives you the vocabulary to do that.

## Key terms

| Term | Plain-English meaning |
|---|---|
| **Metric** | Any number you track over time (orders per day, % of users who return). |
| **KPI** | Key performance indicator: a metric leadership has agreed matters most. |
| **Leading metric** | An early signal that predicts a later result. |
| **Lagging metric** | A result you only see after the fact (revenue, churn). |
| **Input metric** | Something a team can move directly, which drives a bigger result. |
| **Output metric** | A result of many things working together; no single team controls it. |
| **Vanity metric** | Looks impressive but doesn't change any decision. |
| **Counter (guardrail) metric** | A number you watch to make sure you're not breaking something while pushing your main number. |
| **Proxy metric** | A number you track because the thing you really care about (like "happiness") is hard to measure directly. |

## The idea, simply

!!! tip "Analogy: the cricket scoreboard"
    Imagine you are captaining a T20 side. The final score at the end of 20 overs is the **result**. But you can't change it once the match is over. During the match you watch the **run rate**, **wickets in hand** and **dot balls**. Those numbers tell you, ball by ball, whether you're on track. They let you change your plan *while it still matters*.

Product metrics work the same way. There are three simple pairs of ideas to learn.

**1. Leading vs lagging**

- A **lagging metric** tells you what already happened. Revenue, profit and yearly churn (how many customers left) are lagging. They are important, but they arrive late.
- A **leading metric** gives you an early signal of what is *likely* to happen. For example, how many new users complete their first order in week one is a good early sign of how many will still be ordering in month three.

**2. Input vs output**

- An **output metric** is a result of many things working together: total orders, revenue, monthly active users. No single team controls it.
- An **input metric** is something your team can push directly this week. Examples: how fast the search page loads, how many restaurants are listed in a new city, or what share of users finish sign-up.
- Teams set goals on inputs, and leaders watch outputs. When the inputs are chosen well, moving them moves the output.

**3. Vanity vs actionable**

- A **vanity metric** looks impressive but doesn't guide a decision. "Total downloads ever" only goes up. It never tells you if people are getting value.
- An **actionable metric** changes your next move. "Share of users who come back in week two" goes up or down based on what you build. That tells you whether your last change helped.

A simple test: *If this number doubled tomorrow, would I know what caused it? Would I do anything differently?* If both answers are no, it's probably vanity.

**Two more ideas you'll hear every day:**

- **Rate vs count.** Counts (like 10,000 sign-ups) grow just because you spent more on ads. Rates (like 40% of sign-ups placing an order) tell you about the *quality* of the experience. Track both, but make decisions with rates.
- **Counter metrics (guardrails).** Whenever you push one number, pick a second number to make sure you aren't breaking something. If you push "orders", also watch "cancellations" and "refunds".

## Framework: The Metric Definition Card + the 2×2

There's no single inventor of leading/lagging or input/output; these ideas come from management accounting and operations. Product teams popularised them through tools like Amazon's input-metric approach and Amplitude's [North Star Playbook](https://amplitude.com/books/north-star), which separates a North Star from the "inputs" that drive it.

**Step 1: Write a metric definition card for every important metric.** Use the [template in the appendix](../../appendix/templates.md). The most common analytics fight in any company is two teams defining "active user" two different ways.

**Step 2: Place the metric on the 2×2 below.** Decide whether it's leading or lagging, and whether it's an input or an output.

**Step 3: Run the vanity test.** If it doubled, would you know why, and would you act differently?

**Step 4: Add a counter metric** that would warn you if you were gaming the number.

**When to use:** whenever you build a dashboard, set a quarterly goal or write a PRD success section.
**When not to:** don't over-engineer metrics for a quick, low-risk experiment. One clear success metric and one guardrail is enough there.

## Diagram

![A 2x2 grid with leading/lagging on top and input/output on the side, with example metrics in each box](../../assets/A8.1/metric-types-2x2.svg)
<p class="caption">The top-left box (leading + input) is where team goals should live: numbers you can move this week that predict next month.</p>

## Worked example

You are the PM for the "Groceries" tab of a food delivery app in Pune. Your manager says: "Our goal this quarter is more grocery orders."

1. **Output (lagging):** weekly grocery orders. Good to report, but it's influenced by ads, festivals and even rain.
2. **Ask "what drives this?"** Orders = (users who open Groceries) × (share who add to cart) × (share who check out) × (orders per user).
3. **Pick a leading input your team owns:** share of first-time grocery users who place a second order within 14 days. This predicts long-term orders, and your team can move it with better substitutes, faster delivery promises and reminders.
4. **Vanity check:** "Grocery tab impressions" would rise if the tab were simply made bigger. That's vanity. Drop it.
5. **Counter metric:** refund rate on grocery orders. If you push second orders by over-promising delivery times, refunds will warn you.
6. **Definition card:** *Second-order rate = first-time grocery buyers in week W who place another grocery order within 14 days ÷ all first-time grocery buyers in week W.*

Now your weekly team review has one steering number, one guardrail, and one scoreboard number for leadership.

## Going deeper: nuances and trade-offs

### 1. Goodhart's law: every target gets gamed

Economist Charles Goodhart made the original point in 1975 about monetary policy. Anthropologist Marilyn Strathern later turned it into the popular saying "when a measure becomes a target, it ceases to be a good measure" ([background](https://en.wikipedia.org/wiki/Goodhart%27s_law)). In product terms: the moment you reward a team for a number, people find the easiest way to move *the number*, which isn't always the thing the number was meant to show.

- Reward support agents for "tickets closed per hour", and tickets get closed before problems are solved.
- Reward a growth team for "sign-ups", and sign-up forms get shorter while user quality drops.

**How experienced PMs defend against it:**

- Always pair the target with a counter metric.
- Prefer metrics close to real customer value.
- Read a sample of real user sessions or tickets every week.
- Treat a sudden, too-easy win as a warning sign.

### 2. Proxy metrics: check that the proxy actually tracks the real thing

Most product metrics are proxies. "Week-1 orders" stands in for "this customer will be valuable for years". A proxy is only useful while it really moves with the outcome you care about. Check it in two ways:

- **Historically:** do users with a high proxy value later show a high outcome?
- **Experimentally:** when an A/B test moves the proxy, does the outcome follow weeks later? See [A9.1](../09-experimentation/01-a-b-testing-basics.md).

Amazon is famous for this discipline. *Working Backwards* by Colin Bryar and Bill Carr describes how Amazon focuses its weekly business reviews on **controllable input metrics** and refines them by trial and error until moving them reliably moves the outputs ([summary by Holistics](https://www.holistics.io/blog/how-amazon-measures); [book site](https://www.workingbackwards.com/)).

### 3. Definitions and time windows change the answer

"Active user" sounds simple until you ask:

- Active doing *what*? Opening the app, or completing a value action?
- Over *what window*?
    - **DAU:** active on a given day
    - **WAU:** active in the last 7 days
    - **MAU:** active in the last 28 or 30 days

Pick the window that matches how often the product is *naturally* used. A bill-payment app used once a month will look "dead" on a daily metric. When you change a definition, keep the old one running for a while and label the switch on every chart. Otherwise trend lines break silently.

### 4. Ratios have two moving parts

**DAU/MAU** (often called *stickiness*) is popular because it shows how often monthly users come back. But a ratio can rise for the wrong reason. If a marketing campaign ends and casual users stop arriving, MAU falls faster than DAU, and stickiness "improves" while the business shrinks. Whenever you report a ratio, show its top and bottom numbers next to it.

### 5. Signal vs noise

Daily numbers bounce around. Before reacting:

- **Compare like with like:** this Tuesday vs the last 4–6 Tuesdays.
- **Know your normal range.** If orders usually swing ±4% week to week, a 3% dip is noise.
- **Remember that small numbers are jumpy.** 20 orders vs 25 orders is a 25% change, but tells you almost nothing.
- **Use the median when outliers distort the average.** Delivery time is a classic example: a few 3-hour deliveries can drag up the mean while most customers had a great experience.

### 6. How metrics differ by business type

- **B2C transactional** (food, travel, payments): orders, frequency, order value, repeat rate.
- **B2C attention** (social, media, OTT): time spent, sessions, content consumed, creator activity.
- **Subscription / SaaS:** paid conversion, churn, revenue retention, seats used.
- **B2B:** measure **accounts and teams**, not just individual users. Signals arrive slowly because there are fewer customers, so lean more on qualitative feedback.
- **India-specific rhythms:** festival seasons (Diwali, Durga Puja), salary-day spikes at the start of the month, exam seasons, monsoon and IPL evenings all shift behaviour. Build them into your "normal range".

## Real-world examples (2023 onwards)

!!! example "Threads (Meta), July 2023: a record sign-up number vs. the real signal"
    Meta launched Threads on 6 July 2023, and it passed 100 million sign-ups within days. The sign-up count was a vanity metric. Within about a week, [Similarweb estimated](https://www.similarweb.com/blog/insights/social-media-news/threads-week/) that daily active users on Android had roughly halved, from about 49 million to 23.6 million. By the end of July, [Sensor Tower data reported by CNN](https://edition.cnn.com/2023/08/03/tech/threads-user-count-falls) put daily users down about 82% from the launch peak, with time spent per user also falling sharply.

    **PM lesson:** sign-ups told you about curiosity. Daily actives and time spent told you about value. Instagram's team kept improving the product after this. The early, honest reading of the *actionable* numbers is what made those fixes possible.

!!! example "Swiggy, 2024–2026: reporting inputs, not just outputs"
    In its shareholder letters, Swiggy reports a small set of operating metrics every quarter. These include average **monthly transacting users (MTU)**, **platform frequency** (orders per user), **average order value** and **gross order value (GOV)**. In the [Q1 FY27 letter (July 2026)](https://nsearchives.nseindia.com/corporate/SWIGGY_30072026154100_Covering_Letter_Letter_to_Shareholders_-_signed.pdf), platform MTU rose to 27.5 million while platform frequency slipped to 3.87 from 4.13 a year earlier.

    **PM lesson:** GOV is the output. MTU and frequency are the inputs that multiply into it. Showing both lets you see *why* the output moved. Here, more users were joining, but the average user was ordering a little less often (see [A8.5](05-funnels-cohorts-and-retention-curves.md) for why that often happens when you grow fast).

## Common mistakes

!!! warning "Watch out for"
    - **Celebrating cumulative totals** ("1 crore downloads!"). They can only go up, so they hide problems.
    - **Setting team goals on outputs the team can't control.** It leads to frustration or gaming.
    - **No written definition.** Two dashboards, two numbers, one wasted meeting.
    - **No counter metric.** You will eventually "win" the number and hurt the business.
    - **Too many metrics.** If everything is important, nothing is. Aim for 1 steering metric and 2–3 guardrails per team.
    - **Silently changing a definition.** The chart now compares apples with oranges.
    - **Reporting only averages.** Show medians or percentiles (p50, p90) when a few outliers distort the picture.

## In the interview

!!! question "In the interview"
    **How it's tested:** "How would you measure the success of *[feature/product]*?" is one of the most common PM interview questions, and it often comes up inside product design questions too.

    **Sample question:** *"How would you measure the success of WhatsApp's 'Status' feature?"*

    **Outline of a strong answer:**

    1. **Clarify the goal:** Is Status meant to raise daily engagement, help people share updates without group-chat noise, or drive ad revenue?
    2. **Name the users and their value:** posters (self-expression) and viewers (staying in touch).
    3. **Pick one primary metric that reflects value:** for example, the % of daily users who view or post at least one Status.
    4. **Add 2–3 input metrics:** posting rate among weekly users, views per Status, replies sent from Status.
    5. **Add guardrails:** the effect on chat messages sent (is Status cannibalising chats?), reported or blocked Statuses, and app performance.
    6. **Say how you'd know it's working:** an A/B test or a before/after comparison with a holdout, and the time frame you'd judge it over.

    Interviewers listen for a clear goal, one main metric, a short list of inputs, and at least one guardrail.

## Research happening now

!!! info "Research happening now"
    - **Acquisition and retention aren't linked (Amplitude, 2025).** Amplitude's [2025 Product Benchmark Report](https://amplitude.com/blog/leaky-bucket-problem) analysed over 2,600 companies. It found no meaningful correlation between how well a product *acquires* users and how well it *keeps* them. This is strong evidence that top-of-funnel counts are a poor proxy for product health. *Status: industry report based on Amplitude customers, not peer-reviewed.*
    - **Metric trees as a discipline.** Data leaders such as Abhi Sivasailam (Levers Labs) have been pushing "metric trees" as a standard way to connect inputs to outputs; see the [Levers Labs introduction](https://www.leverslabs.com/article/introducing-metric-trees). Analytics tools like [Mixpanel](https://mixpanel.com/blog/metric-tree/) now ship metric-tree features. *Status: fast-growing practice; standards still forming.* Covered in depth in [A8.2](02-north-star-metric-and-metric-trees.md).

## Try it yourself (20 minutes)

Open any app you use daily (UPI, food delivery, a news app). Write down:

1. One **vanity** metric the company might brag about
2. One **lagging output** metric
3. One **leading input** metric a single team could own
4. One **counter metric** for that input

Then write a one-line definition card for the input metric.

??? success "Check your answer"
    For a UPI payments app, a good answer might look like this:

    - **Vanity:** total app downloads, or "10 crore registered users".
    - **Lagging output:** monthly transaction value, or revenue from merchant services.
    - **Leading input:** the % of new users who complete their *second* payment within 7 days, owned by the onboarding team.
    - **Counter metric:** failed-payment rate, or fraud complaints per 10,000 transactions.
    - **Definition card:** *Second-payment rate = new users in week W who complete a 2nd successful payment within 7 days of their first ÷ all new users who made a first payment in week W.*

    Check that your input is something one team can move *this month*, and that your counter metric would warn you if the team cut corners.

## How this connects

- [A8.2 North Star metric and metric trees](02-north-star-metric-and-metric-trees.md): organises input and output metrics into one tree.
- [A8.5 Funnels, cohorts and retention](05-funnels-cohorts-and-retention-curves.md): the most important leading metric for most products.
- [A8.6 Diagnosing a metric drop](06-diagnosing-a-metric-drop.md): what to do when a metric moves unexpectedly.
- [A4.3 OKRs and goal setting](../04-strategy-and-vision/03-okrs-and-goal-setting.md): good key results are usually leading input metrics.
- [A9.1 A/B testing basics](../09-experimentation/01-a-b-testing-basics.md): how to prove an input actually moves an output.

## Go deeper

- **Book:** [*Lean Analytics*](https://www.oreilly.com/library/view/lean-analytics/9781098168179/) by Alistair Croll and Benjamin Yoskovitz. The classic on vanity vs actionable metrics. (Teresa Torres has a short [review on Product Talk](https://www.producttalk.org/read-lean-analytics/).)
- **Guide:** [Amplitude North Star Playbook](https://amplitude.com/books/north-star). Free; it explains how output and input metrics fit together.
- **Article:** [Amplitude: The leaky bucket problem](https://amplitude.com/blog/leaky-bucket-problem). Benchmark data on why more users doesn't mean more growth.
- **Watch:** [Lenny's Podcast on YouTube](https://www.youtube.com/@lennyspodcast). Search the channel for the Sean Ellis episode on North Star metrics.

## Key takeaways

- A metric is only useful if it can change your next decision.
- **Leading** metrics warn early; **lagging** metrics confirm late. You need both.
- Set team goals on **inputs** they control; report **outputs** to leadership.
- Prefer **rates** over **counts** when you make decisions.
- Always pair a target metric with a **counter metric**.
- **Goodhart's law:** any number you reward will be gamed. Pair targets with guardrails and read real user behaviour.
- Write down **definitions and time windows**, and match the window to how often the product is naturally used.

## Updates

*No updates yet.*
