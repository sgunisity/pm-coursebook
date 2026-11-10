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

## Updates

*No updates yet.*
