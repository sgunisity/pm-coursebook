---
id: A8.5
title: "Funnels, cohorts and retention curves"
last_reviewed: 2026-11-10
---

# A8.5 Funnels, cohorts and retention curves

## In one line

A **funnel** shows where users drop off on the way to a goal. A **cohort** groups users by when they started. A **retention curve** shows how many in each cohort keep coming back.

## Why this matters

Averages lie. "Monthly active users are up" can hide the fact that every new group of users leaves faster than the last. Funnels, cohorts and retention curves are the three tools that show you what's *really* happening. They're also the first thing an investor or senior PM will ask to see.

## Key terms

| Term | Plain-English meaning |
|---|---|
| **Funnel** | A set of steps toward a goal, showing how many users reach each step. |
| **Conversion rate** | % of users who move from one step to the next. |
| **Cohort** | A group of users who share a starting point (e.g. signed up in March). |
| **N-day retention** | % of a cohort active *on* day N (or in week/month N). |
| **Unbounded retention** | % of a cohort active on day N *or any time after*. |
| **Churn** | % of users or customers who stop using or paying in a period. |
| **Net revenue retention (NRR)** | Revenue this year from last year's customers ÷ their revenue last year; above 100% means existing customers grew. |
| **Mix effect** | An average changing because the *types* of users changed, not their behaviour. |

## The idea, simply

!!! tip "Analogy: a school's batches"
    A coaching centre wants to know if its teaching is getting better. Looking at "total students this year" doesn't help, because new admissions hide dropouts. Instead it tracks each **batch** (the 2024 batch, the 2025 batch) separately. How many from each batch were still attending after 1 month, 3 months, 6 months? If newer batches stay longer, teaching is improving. That batch-by-batch view is **cohort analysis**.

### Funnels

A funnel is a list of steps toward a goal, with the % who make it to each step.

*Example: ordering food*
Open app → search → open restaurant → add to cart → pay → order delivered

- Look at the **step-to-step conversion**, not just start-to-end. The step with the biggest drop is your first problem.
- **Segment** the funnel: new vs returning users, Android vs iOS, city by city. A problem in one segment is often hidden in the total.
- Set a **time window**, e.g. "within the same session" or "within 7 days".

### Cohorts

A cohort is a group of users who share a starting point, usually the week or month they signed up (or first ordered). You then follow each cohort over time.

*Example cohort table (% of users still ordering):*

| Sign-up month | Month 1 | Month 2 | Month 3 | Month 6 |
|---|---|---|---|---|
| Jan | 100% | 42% | 33% | 25% |
| Feb | 100% | 45% | 36% | 28% |
| Mar | 100% | 48% | 39% | — |
| Apr | 100% | 51% | — | — |

Read it **down the columns**. Month-2 retention has improved from 42% to 51% across four cohorts, so recent product changes are working. A single "overall retention" number would have hidden this.

### Retention curves

Plot one cohort's retention over time and you'll see one of three shapes (see diagram):

1. **Falls to zero.** Almost everyone leaves eventually, so the product hasn't found its fit yet.
2. **Flattens.** Retention drops at first, then levels off. You have a loyal core. This is the classic sign of product-market fit.
3. **Smiles.** It dips, then rises as some users come back and use the product more. That's rare and powerful.

**What is "good" retention?** It depends on the type of product. A widely used benchmark from Lenny Rachitsky and Casey Winters ([*What is good retention?*](https://www.lennysnewsletter.com/p/what-is-good-retention-issue-29), based on a survey of growth experts) suggests rough 6-month user retention:

| Product type | Good | Great |
|---|---|---|
| Consumer social | ~25% | ~45% |
| Consumer transactional (e.g. food, travel) | ~30% | ~50% |
| Consumer SaaS / subscription | ~40% | ~70% |
| SMB / mid-market SaaS | ~60% | ~80% |
| Enterprise SaaS | ~70% | ~90% |

Treat these as rough guides. Your own trend over time matters more.

### Building a cohort table, step by step

You don't need advanced tools to do this. A spreadsheet works.

1. **List users with their start date** (sign-up or first order) and assign each a cohort: the week or month they started.
2. **List every value action** (e.g. each delivered order) with its date.
3. **For each user, work out which periods after their start they were active:** week 0, week 1, week 2…
4. **Count active users per cohort per period,** then divide by the cohort size to get percentages.
5. **Lay it out** with cohorts as rows and periods as columns. Highlight with colour: darker means higher retention.

Most product analytics tools (Amplitude, Mixpanel, Google Analytics, CleverTap, MoEngage) build this automatically. Knowing the steps helps you check that the tool's settings match your definition.

### Four numbers to pull from every retention curve

| Number | What it tells you | What usually moves it |
|---|---|---|
| **Early drop** (period 0 → 1) | How many people never really got value | Activation and onboarding |
| **Slope** (how fast it falls after that) | Whether value lasts | The core experience and habit formation |
| **Plateau level** | Your loyal core as a % of each cohort | Product-market fit for that segment |
| **Plateau start** (when it flattens) | How long it takes users to "settle" | Learning curve, payday or usage cycles |

When you report retention, report these four numbers, not just one. "Our early drop improved from 55% to 48%, plateau unchanged at 22%" is far more useful than "retention went up".

### Funnel maths: where to fix first

Percentages can mislead you about where the biggest win is. Look at **users lost at each step**:

| Step | Users reaching it | Step conversion | Users lost here |
|---|---|---|---|
| Opened app | 100,000 | — | — |
| Searched | 70,000 | 70% | 30,000 |
| Opened a restaurant | 49,000 | 70% | 21,000 |
| Added to cart | 19,600 | 40% | 29,400 |
| Paid | 15,680 | 80% | 3,920 |

Payment conversion (80%) looks best, and add-to-cart (40%) looks worst. But ask what a **realistic improvement** at each step would add at the end:

- Lifting add-to-cart from 40% to 44% adds 1,960 carts. At 80% payment, that's **+1,568 orders**.
- Lifting payment from 80% to 84% adds **+784 orders**.

Both are worth doing. The add-to-cart fix is worth twice as much, *if* it's equally easy. Always convert step improvements into **final outcomes** before choosing what to work on.

## Framework: the weekly retention review

1. **Pick the action that means "retained".** This is a value action, not just "opened the app". Example: placed an order, or completed a lesson.
2. **Pick the right interval** for your product's natural frequency: daily for messaging, weekly for food delivery, monthly for bill payments.
3. **Build a cohort table** by sign-up week or month.
4. **Read down the columns** to see if newer cohorts do better.
5. **Look for the flattening point.** Where does the curve level off, and at what %?
6. **Find what retained users did early on** that churned users didn't. This is your activation clue. (It's a correlation; test it with an experiment, see [A9.1](../09-experimentation/01-a-b-testing-basics.md).)

## Diagram

![Three retention curves: one falling to zero, one flattening, and one smiling upward](../../assets/A8.5/retention-curves.svg)
<p class="caption">You want your curve to flatten (blue) or smile (black). A curve that keeps sliding to zero means fix the product before spending on growth.</p>

## Worked example

You're PM for a fitness app. Overall monthly active users are up 20% in 6 months, and leadership is happy. You build a cohort table:

- Cohorts from 6 months ago: month-3 retention 30%.
- Cohorts from 3 months ago (after a big ad campaign): month-3 retention 18%.

**Diagnosis:** the ad campaign brought in lots of users who don't stick. MAU is up only because acquisition is huge. That's the [leaky bucket](https://amplitude.com/blog/leaky-bucket-problem).

**Funnel check on the new cohorts:** 70% install → 40% finish the fitness quiz → only 15% complete their first workout. The big drop is between the quiz and the first workout.

**Action:** shorten the quiz, start a 5-minute "first workout" right after it, and measure month-1 retention of the next cohorts. Guardrail: workout injuries reported (don't push too hard too soon).

## Going deeper: nuances and trade-offs

### 1. Three ways to count retention, and why the number changes

Imagine 100 users who signed up on 1 March:

- **N-day (or N-week/month) retention:** how many were active *in* week 4? Say 30. This is the strictest and most common measure.
- **Unbounded (rolling) retention:** how many were active in week 4 *or any later week*? Say 40. It's higher because it counts people who skipped week 4 but came back later.
- **Bracket retention:** how many were active at least once *between* weeks 3 and 5? Useful for products used irregularly.

None is "right". Pick one, write it on your [definition card](../../appendix/templates.md), and never compare numbers measured different ways.

### 2. Which starting point should define a cohort?

- **Sign-up date:** the default. Good for judging onboarding.
- **First value action** (first order, first lesson): removes people who signed up but never really started. Good for judging the core product.
- **Acquisition channel or campaign:** reveals which channels bring users who stay. Often the most useful view for marketing spend.
- **Behavioural cohorts** ("users who used feature X in week 1"): good for finding activation moments. Remember that correlation isn't cause ([A8.3](03-aarrr-and-google-s-heart-framework.md)).

### 3. User retention vs revenue retention

In subscription and B2B products, track two kinds of retention:

- **User or logo retention:** are customers still here?
- **Revenue retention:**
    - **GRR** (gross revenue retention) counts only losses: cancellations and downgrades.
    - **NRR** (net revenue retention) also counts upgrades and expansion. **NRR above 100%** means your existing customers spend more over time, even after some leave. That's one of the strongest signals a SaaS business can have.

Lenny Rachitsky's [benchmarks](https://www.lennysnewsletter.com/p/what-is-good-retention-issue-29) include NRR ranges by business type too.

### 4. Funnel traps

- **Ordered vs any-order funnels:** must users do steps in sequence? Real users jump around.
- **Time window:** a 1-hour window and a 7-day window give very different conversion rates for the same funnel.
- **Multiple sessions:** many Indian users browse on one day and buy on payday. A same-session funnel will under-count them.
- **Denominator choice:** is step 1 "opened the app" or "opened the product page"? Always state it.

### 5. Survivorship bias in feedback

If you survey only active users, you hear from the people who stayed. Churned users, the ones with the most important feedback, are gone. Run short exit surveys or churned-user interviews regularly. Make sure the cohorts you analyse include everyone who started, not just the survivors.

### 6. Reading curves without fooling yourself

- **Small cohorts are noisy.** Don't conclude anything from a cohort of 80 users.
- **Festival and campaign cohorts behave differently.** A Diwali-sale cohort will look worse than an organic cohort. Compare like with like.
- **"Flattening" needs several periods.** One flat month isn't a plateau.
- **Look at curves by segment:** city, platform, channel. A good overall curve can hide one segment sliding to zero.

### 7. Resurrected users

Some users leave and come back weeks or months later, often thanks to a festival sale, a new feature, or a friend's referral. Track them as their own group:

- **Reactivated:** returned after a short break (e.g. 1–4 weeks).
- **Resurrected:** returned after a long break (e.g. 30+ days).

Duolingo's growth model counts these groups separately ([A8.2](02-north-star-metric-and-metric-trees.md)). They behave differently from both new and current users, so campaigns aimed at them should be measured on their own retention.

### 8. When averages hide the distribution

"Average orders per user = 4" can mean every user orders 4 times, or 10% of users order 30 times while most order once. Look at the **distribution** (how many users ordered 1, 2, 3 … times) before designing for "the average user", who may not exist. Power users often deserve their own features. Light users often need activation help.

## Real-world examples (2023 onwards)

!!! example "AI products and the 'AI tourist' problem (a16z, September 2025)"
    In [*Retention Is All You Need*](https://a16z.com/ai-retention-benchmarks/), a16z partners Santiago Rodriguez and Alex Immerman argue that many AI products attract curious "tourists" who try once and leave. That makes early retention curves look worse and less predictive than usual. They suggest measuring from **month 3**, once tourists have left, and using **M12 ÷ M3** to judge how the committed users behave over a year. The same article shows ChatGPT's monthly usage retention curve forming a "smile".

    **PM lesson:** choose the starting point of your curve carefully. For products with a lot of casual trial, the month-0 baseline can mislead you.

!!! example "Swiggy, FY26: when more users means lower average frequency"
    By Q4 FY26, Swiggy's platform monthly transacting users had grown about 27% year-on-year to 25.2 million, [MediaNama reported](https://www.medianama.com/2026/05/223-q4fy26-swiggy-adds-users-faster-retains-food-delivery-hits-15-quarter-high/). Over the same period, platform frequency (orders per user) dipped to 4.01, according to the company's shareholder letters.

    **PM lesson:** this is a classic **mix effect**. When lots of new users join, they usually order less often than long-time users at first. So the *average* falls even if no one's behaviour got worse. Cohort analysis is how you tell the difference: compare each cohort's frequency with older cohorts at the same age.

## Common mistakes

!!! warning "Watch out for"
    - **"Retained" = "opened the app".** Use a value action instead.
    - **Wrong interval.** Measuring daily retention for a monthly-use product makes it look broken.
    - **Reading cohort tables across rows only.** The real insight is in comparing columns.
    - **Mixing new and old users in one average.** This hides both problems and wins.
    - **Treating correlation as cause.** "Users who add 3 friends retain better" might be because engaged people add friends, not the other way round. Test it.
    - **Mixing retention definitions** (N-day vs unbounded) between reports.
    - **Learning only from survivors.** Talk to churned users too.

## Common questions

**Weekly or monthly cohorts?**
Use the product's natural frequency. Weekly suits food delivery and social apps. Monthly suits bill payments and subscriptions. When volumes are small, monthly cohorts are less noisy.

**What retention is "good enough" to start spending on growth?**
When curves flatten at a healthy level for your product type (see the benchmark table) across several cohorts, and the plateau holds for new cohorts too.

**Should I count retention by users or by revenue?**
Both, for subscription and B2B. Users tell you about engagement; revenue retention tells you about business health and expansion.

**How do I handle users who use the product on multiple devices?**
Count people, not devices: make sure analytics ties sessions to a logged-in user ID. Otherwise one person can show up as several "churned" users.

**My funnel shows a huge drop at sign-up. Should I remove sign-up?**
Maybe, but test it. Removing sign-up often lifts early steps while lowering later activation or retention (users who don't commit leave anyway). Measure the whole funnel through to retention, not just the next step.

## In the interview

!!! question "In the interview"
    **How it's tested:** "How would you improve retention for *[product]*?" or "New-user retention fell last month. What do you do?" Interviewers want to see cohort thinking, a funnel breakdown and a clear activation hypothesis.

    **Sample question:** *"How would you improve retention for a language-learning app?"*

    **Outline of a strong answer:**

    1. **Define retention:** completed at least one lesson in week N (a value action, not app opens), measured weekly.
    2. **Show the current shape:** cohort curves by sign-up week and by channel. Where's the biggest drop? Usually between day 1 and day 7.
    3. **Find the activation moment:** for example, users who finish 3 lessons in their first week retain much better. Treat it as a hypothesis.
    4. **Propose 2–3 ideas aimed at that moment:** a shorter first lesson, a goal set at sign-up, a well-timed reminder, a streak.
    5. **Explain how you'll measure:** A/B tests on new cohorts, a primary metric of week-4 retention, and a guardrail of notification opt-outs.
    6. **Mention segments:** check that the gains hold across platforms and channels.

## Research happening now

!!! info "Research happening now"
    - **The "7% rule" for week one (Amplitude, September 2025).** Amplitude's [2025 Product Benchmark analysis](https://amplitude.com/blog/7-percent-retention-rule) covers more than 2,600 companies. It proposes Day-7 retention of about 7% as a threshold that separates growing products from churning ones. It also found strong links between week-one activation and three-month retention. *Status: vendor benchmark; correlation-based.*
    - **AI subscription retention (RevenueCat, March 2026).** RevenueCat's [2026 report](https://www.revenuecat.com/state-of-subscription-apps/) found AI-powered apps keep fewer paying subscribers over monthly and annual periods than non-AI apps, despite stronger early conversion ([TechCrunch summary](https://techcrunch.com/2026/03/10/ai-powered-apps-struggle-with-long-term-retention-new-report-shows/)). *Status: industry dataset; researchers are still debating how much is "tourist" churn.*

## Try it yourself (30 minutes)

Use this toy data (users still active by month):

- Jan cohort: 1,000 → 400 → 300 → 280
- Feb cohort: 1,200 → 540 → 420 → —
- Mar cohort: 1,500 → 600 → — → —

1. Turn it into a % cohort table.
2. Is retention improving or getting worse?
3. Where is the curve flattening, and at roughly what %?
4. Write one sentence you'd say to your manager.

??? success "Check your answer"
    The % cohort table:

    | Cohort | M1 | M2 | M3 | M4 |
    |---|---|---|---|---|
    | Jan | 100% | 40% | 30% | 28% |
    | Feb | 100% | 45% | 35% | — |
    | Mar | 100% | 40% | — | — |

    - **Trend:** February improved on January (45% vs 40% in M2), but March fell back to 40%. **No clear improvement yet.** Find out what was different about February: a campaign, a feature, a festival?
    - **Flattening:** January drops from 30% to 28% between M3 and M4, so it's levelling off at roughly **28–30%**.
    - **One-liner to your manager:** "Retention is flattening at about 28–30%, which is healthy for a transactional product. February's better month-2 hasn't repeated in March, so we're checking what drove it before calling it a trend."

## How this connects

- [A8.3 AARRR and HEART](03-aarrr-and-google-s-heart-framework.md): activation and retention as stages of the customer journey.
- [A8.4 Lean Analytics](04-lean-analytics-one-metric-that-matters-and-stage.md): a flattening retention curve is the Stickiness gate.
- [A8.6 Diagnosing a metric drop](06-diagnosing-a-metric-drop.md): segment and mix-shift thinking applied to sudden changes.
- [A9.1 A/B testing basics](../09-experimentation/01-a-b-testing-basics.md): proving that a retention idea works.
- [A10.4 Retention and engagement](../10-growth-and-go-to-market/04-retention-and-engagement.md): tactics for improving the curves you measure here.

## Go deeper

- **Article:** [Lenny Rachitsky: What is good retention?](https://www.lennysnewsletter.com/p/what-is-good-retention-issue-29). The benchmark table above, with examples.
- **Article:** [a16z: Retention Is All You Need](https://a16z.com/ai-retention-benchmarks/). Retention curves for AI products.
- **Benchmarks:** [Amplitude: The 7% Retention Rule](https://amplitude.com/blog/7-percent-retention-rule).
- **Book:** [*Lean Analytics*](https://www.oreilly.com/library/view/lean-analytics/9781098168179/). The cohort analysis chapter is a great beginner's walkthrough.

## Key takeaways

- **Funnels** show where users drop; fix the biggest drop first.
- **Cohorts** group users by start date so averages can't hide the truth.
- A **flattening retention curve** is the clearest sign of product-market fit.
- Pick a **value action** and the **right interval** for your product.
- Fast growth lowers averages (the mix effect). Compare cohorts at the same age.
- Choose **one retention definition** (N-day, unbounded or bracket) and stick to it.
- For subscriptions and B2B, track **revenue retention (NRR)** as well as user retention.

## Updates

*No updates yet.*
