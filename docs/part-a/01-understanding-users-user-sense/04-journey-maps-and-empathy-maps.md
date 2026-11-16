---
id: A1.4
title: "Journey maps and empathy maps"
last_reviewed: 2026-11-16
---

# A1.4 Journey maps and empathy maps

## In one line

A journey map shows the steps a user goes through to reach a goal and how they feel at each one; an empathy map shows what a user says, does, thinks and feels. Together they show your team where the experience hurts, and why.

## Why this matters

Your team sees the product one screen at a time. Your user lives it as one long story, including the parts that happen outside your app. A journey map lets you see the whole story, find the moments that make or break it, and decide what to fix first.

An empathy map does the same for one user's inner world. It's the fastest way to get a room of engineers, designers and leaders to stop arguing about opinions and start talking about the same real person. Both turn research ([A1.2](02-user-research-methods-and-interviews.md)) into something a team can act on.

## Key terms

| Term | Plain-English meaning |
|---|---|
| **Journey map** | A picture of the steps a person takes to reach a goal, with what they do, think and feel at each step. |
| **Empathy map** | A one-page picture of what one type of user says, does, thinks and feels. |
| **Actor** | The person whose journey you're mapping (often a persona, see [A1.3](03-personas-and-jobs-to-be-done.md)). |
| **Phase (stage)** | A big chunk of the journey, like "find", "decide", "pay", "use". |
| **Touchpoint** | Any place the user meets your product or company: an app screen, an SMS, a call, a delivery person. |
| **Pain point** | A moment where the user is confused, slowed down, worried or annoyed. |
| **Moment that matters** | A step that strongly shapes how the user feels about the whole experience. |
| **Service blueprint** | A journey map extended to show the people, processes and systems behind each step. |

## The idea, simply

!!! tip "Analogy: the train trip home for Diwali"
    Think about a long train trip home for a festival. It isn't one event. It's a chain: booking a ticket (and waiting to see if your waitlisted seat confirms), getting to the station, finding the platform, boarding, the night on the train, food, and finally arriving.

    Ask someone about the trip a week later. They won't describe every step evenly. They'll remember the anxious hours checking whether the ticket confirmed, the platform change announced at the last minute, and the great chai at one station. The rest blurs.

    Now imagine the railway only looked at one piece, say, the booking website. It might make booking faster and still leave people miserable, because the real pain was the waitlist anxiety and the platform confusion. A **journey map** is a picture of the whole trip, with the highs and lows marked. An **empathy map** is what's going on inside the traveller's head.

Products work the same way. Let's build it up.

### 1. What a journey map is made of

Nielsen Norman Group (NN/g), the user-experience research firm, defines a journey map as a visualisation of the process a person goes through to accomplish a goal ([Journey Mapping 101](https://www.nngroup.com/articles/journey-mapping-101/)). Its core parts:

| Part | Question it answers | Example: a parent paying school fees online |
|---|---|---|
| **Actor** | Whose journey is this? | A working parent paying for one child, on a phone |
| **Scenario and expectations** | What are they trying to do, and what do they expect? | "Pay this term's fees before the due date; I expect it to take 5 minutes" |
| **Phases** | What are the big stages? | Get notice → find school → identify child → pay → get confirmation |
| **Actions** | What do they do at each step? | Searches for the school, types the student ID from a paper circular |
| **Thoughts** | What are they wondering? | "Where is that ID? Did the school actually get my money?" |
| **Emotions** | How do they feel, step by step? | Shown as a line that rises and falls |
| **Opportunities** | What could we improve? | "Let parents find their child by name and class" |
| **Ownership and metrics** | Who owns each fix, and how will we know it worked? | Onboarding pod; % of parents who reach the payment step |

NN/g advises **one actor and one scenario per map**. A map that tries to cover "all users" ends up describing nobody.

### 2. What an empathy map is made of

An empathy map is simpler. It's one page about one type of user, usually split into four boxes:

| Box | What goes in it | Example (the same parent) |
|---|---|---|
| **Says** | Things they said out loud, ideally exact quotes | "I just want a receipt the school will accept." |
| **Does** | What they were seen doing | Took a screenshot of the payment page "just in case" |
| **Thinks** | Beliefs and worries they may not say | Worries the payment will be "lost" and the child named in class |
| **Feels** | Emotions | Anxious near the due date; irritated by a surprise convenience fee |

The empathy map was created at the design firm XPLANE as part of the *Gamestorming* toolkit. Its creator, Dave Gray, later published an [updated empathy map canvas](https://medium.com/the-xplane-collection/46df22df3c8a). The update adds:

- **a goal section** at the top: who are we empathising with, and what do they need to do?
- **Sees** and **Hears** boxes for what's around them (ads, advice from friends, what the school says)
- **Pains and gains** inside the "think and feel" area

Gray also numbered the sections so teams fill in the *observable* things (sees, says, does, hears) before guessing at the *inner* things (thinks, feels). That order matters. It keeps the team anchored in evidence.

**Why the "says vs thinks" split is powerful.** People often say one thing and think another. "The app is fine" (says) can sit next to "I don't trust it with large amounts" (thinks). The gap between boxes is often where the insight is.

### 3. Which map for which question

Many map types exist and they're easy to mix up. Each answers a different question.

| Tool | Question it answers | Scope |
|---|---|---|
| **Empathy map** | What's going on inside this user? | One user type, one moment or theme |
| **Persona** ([A1.3](03-personas-and-jobs-to-be-done.md)) | Who is this user, and what do they want? | One user type, overall |
| **Journey map** | What happens, step by step, as they reach one goal with us? | One actor, one scenario, one product |
| **Experience map** | What does this kind of experience look like for people in general? | Broader than your product (e.g. "moving to a new city") |
| **Service blueprint** | What's happening behind the scenes at each step? | Customer steps plus staff, processes and systems |
| **User flow** | Which screens and taps does the user go through? | Screen-level, inside your product |
| **Story map** ([A6.2](../06-product-design-and-ux/02-user-story-mapping.md)) | What should we build, and in which release? | Planning the work, organised by the journey |

A useful rule: **empathy maps go deep on one person; journey maps go wide across time.** Teams often make an empathy map first, then use it to fill the "thinks" and "feels" rows of a journey map.

### 4. Current-state vs future-state maps

There are two kinds of journey map, and you should never mix them on one page.

- **Current-state map:** how the journey works *today*, based on research. It's for finding problems.
- **Future-state map:** how you *want* it to work. It's for aligning the team on a vision and planning changes.

| | Current state | Future state |
|---|---|---|
| **Built from** | Interviews, data, support tickets, observation | The current map, plus ideas and strategy |
| **Use it to** | Find and rank pain points | Agree a target experience; plan a roadmap |
| **Biggest risk** | Filling gaps with assumptions | Drawing a dream nobody can build |

Start with the current state. A future map drawn without one usually just shows what the team already wanted to build.

### 5. Moments that matter: not every step is equal

Most journeys have dozens of steps. Users judge the whole experience by a few of them. Two patterns help you find those few.

**Emotional lows.** Mark where the emotion line drops sharply. These are usually moments of *uncertainty* (did it work?), *effort* (where do I find this?), or *surprise* (why is the price higher now?).

**The peak–end rule.** Psychologist Daniel Kahneman and colleagues found that people judge a past experience largely by its most intense moment and by how it ended, not by the average of every moment ([background](https://en.wikipedia.org/wiki/Peak%E2%80%93end_rule)). For products, this means:

| If the journey… | …users tend to remember it as |
|---|---|
| Is smooth but ends with "payment pending" for an hour | Stressful |
| Has one annoying step but ends with an instant, clear confirmation | Fine |
| Has one delightful moment (an early delivery) | Better than its average step |

So a fix to the *end* of a journey, or to its worst moment, often does more for satisfaction than polishing a step in the middle.

### 6. Where the content of a map comes from

A journey map is only as honest as the evidence behind it. Use several sources, and mark what's evidence versus guesswork.

| Source | What it tells you | Which rows it fills |
|---|---|---|
| Interviews and observation ([A1.2](02-user-research-methods-and-interviews.md)) | Why people act, what they worry about | Thoughts, emotions, quotes |
| Funnel analytics ([A8.5](../08-product-metrics/05-funnels-cohorts-and-retention-curves.md)) | Where and how many people drop | Actions, size of each pain |
| Support tickets and call logs | What goes wrong after the fact | Pain points, often at the end of journeys |
| App-store reviews, social posts | Strong emotions in users' own words | Emotions, quotes |
| Frontline staff (support, delivery, sales) | Workarounds users invent | Actions, offline steps |

If you have no research yet, you can still sketch an **assumption-based map** in a workshop. Label it clearly as hypotheses, then go and check the riskiest ones with real users.

### 7. Front stage and backstage: the service blueprint

Users see the **front stage**: screens, messages, people. Pain often comes from the **backstage**: a slow bank reconciliation, a school that updates its records once a week, a warehouse that doesn't know an order changed.

A **service blueprint** adds the backstage to a journey map. It shows, under each customer step, what staff do and which systems are involved. G. Lynn Shostack introduced the idea in a 1984 *Harvard Business Review* article ([background](https://en.wikipedia.org/wiki/Service_blueprint)). NN/g has a clear [modern guide](https://www.nngroup.com/articles/service-blueprints-definition/).

As a PM, reach for a blueprint when the pain point you found can't be fixed with a screen change. For example, "the school can't see my payment" is a backstage problem: the data reaches the school only in a nightly batch.

## Framework: Journey mapping in seven steps (with an empathy map)

**Origin.** Journey mapping has no single inventor; it grew out of service design and customer-experience practice. Its closest ancestor is Shostack's 1984 service blueprint. The steps below follow NN/g's widely used approach ([Journey Mapping 101](https://www.nngroup.com/articles/journey-mapping-101/)). The empathy map step uses Dave Gray's [updated canvas](https://medium.com/the-xplane-collection/46df22df3c8a).

**Step 1: Pick the actor and the scenario.** One user type, one goal. Write it as a sentence: "A working parent pays one child's term fees on a phone, before the due date."

**Step 2: Gather evidence.** Pull together interviews, funnel data, support tickets and reviews. If you have none, plan 5–8 quick interviews before the workshop.

**Step 3: Make an empathy map first (30–45 minutes).** With the team, fill in sees, says, does, hears from real evidence, then thinks, feels, pains and gains. This warms the team up to the user's point of view.

**Step 4: Lay out the phases and steps.** Five to seven phases is usually right. Include steps outside your product (asking a friend, calling the school, checking SMS).

**Step 5: Fill in actions, thoughts and emotions for each step.** Draw the emotion line. Add real quotes wherever you have them. Mark which cells are evidence and which are assumptions.

**Step 6: Mark the moments that matter.** Circle the two or three biggest lows, and look hard at the ending. Size each one with data: how many users hit it, and how many drop off or complain.

**Step 7: Turn lows into owned opportunities.** For each big low, write an opportunity ("help parents identify their child without the ID"), an owner, and a metric that would show it improved. Rank them by value and effort ([A5.2](../05-roadmaps-and-prioritisation/02-prioritisation-frameworks-rice-ice-moscow-kano.md)).

**When to use:**

- when the problem spans several screens, channels or teams
- when the team disagrees about where users struggle
- when onboarding new team members to a product
- before a redesign of an end-to-end flow

**When not to:**

- for a single-screen bug or a small UI tweak (just fix it)
- when you have no evidence and no time to get any (an untested map can mislead with confidence)
- as a one-off poster. A map nobody owns or updates turns into wall decoration within a quarter.

## Diagram

![A journey map for a parent paying school fees online. Five phases run left to right: get notice, find school, identify child, pay, get confirmation. Rows show actions, thoughts and an emotion line that dips at identify child and at get confirmation. The bottom row lists opportunities.](../../assets/A1.4/journey-map.svg)
<p class="caption">Read the emotion line first. The two dips, finding the student ID and waiting to know if the school received the money, are where the opportunities are.</p>

## Worked example

You're the PM for school-fee payments at a fictional Indian payments app, "FeeEasy". Schools sign up; parents pay term fees in the app. Leadership says: "Fee payments feel stuck. Find out why." All numbers below are illustrative, to show the method.

**Step 1: Actor and scenario.** "A working parent pays one child's term fees on a phone, before the due date." You leave out schools' admin staff; they get their own map later.

**Step 2: Evidence.** You pull the monthly funnel, 600 recent support tickets, and run 8 parent interviews in Pune and Lucknow.

**Step 3: Empathy map (from the interviews).**

| Box | What you found |
|---|---|
| **Sees** | A paper circular with a long student ID; the school's WhatsApp group |
| **Says** | "Where do I even find this ID?" · "I need proof the school got it." |
| **Does** | Photographs the circular; screenshots the payment page; calls the school office |
| **Hears** | Other parents in the group: "My payment showed pending for two days" |
| **Thinks** | "If the school doesn't see it, my child gets a late-fee notice." |
| **Feels** | Rushed near the due date; anxious after paying; annoyed by a fee that appears only at the end |
| **Pains** | Finding the ID; not knowing if the school received the money; the surprise convenience fee |
| **Gains** | Paying in two minutes; a receipt the school accepts; never visiting the office |

**Step 4–5: The journey, with data.**

| Phase | Parents reaching this step (per month) | Drop at this step | Emotion | What interviews and tickets say |
|---|---|---|---|---|
| Get notice | 2,00,000 open the fee page | — | Neutral | "I pay every term; I just want it done" |
| Find school | 1,84,000 | 8% | Neutral | Mostly fine; some school names misspelt |
| Identify child | 1,50,000 | 18.5% | **Low** | Student ID is only on a paper circular |
| Pay | 1,30,000 pay | 13% | Dips | Convenience fee shown only on the last screen |
| Get confirmation | 28,600 contact support (22% of payers) | — | **Lowest** | "Payment done, but school says not received" |

**Step 6: Moments that matter.** Two big lows stand out: identifying the child, and the uncertain ending. The ending matters extra because of the peak–end rule: it's what parents remember next term. A third issue, the surprise fee at the pay step, is smaller, but it's also a legal risk under India's rules on "drip pricing" (see the real-world examples).

You check the backstage for the ending. The school dashboard updates once a night from the bank file, so for up to 24 hours the school sees "not paid". That's a service-blueprint problem, not a screen problem.

**Step 7: Turn lows into owned opportunities, and estimate what they're worth.** FeeEasy earns ₹12 per payment from schools. Each support contact costs ₹35 to handle.

| Opportunity | Owner | Estimate | Value per month | Effort |
|---|---|---|---|---|
| **A. Find your child by name, class and parent phone** (schools upload class lists) | Onboarding pod | ID-step drop falls from 18.5% to 9%: about 17,400 more parents reach payment; at today's 87% pay success, about 15,100 more payments | 15,100 × ₹12 ≈ **₹1.8 lakh** | Medium (6 weeks, needs schools' data) |
| **B. Show the full amount, fee included, from the first screen** | Payments pod | Interviews suggest a share of pay-step drop-outs are fee surprises; assume 2,500 more payments | 2,500 × ₹12 = **₹30,000**, plus removing a compliance risk | Small (1 week) |
| **C. Real-time "school has received it" confirmation**, on the school dashboard and on WhatsApp | Platform pod | Real-time updates to schools; "did school get it?" contacts fall by about 70%: about 20,000 fewer | 20,000 × ₹35 = **₹7 lakh** | Large (8 weeks, school ERP integration) |

**What is it worth over a year?**

| Opportunity | Value per year | Notes |
|---|---|---|
| A | ≈ ₹21.7 lakh | Plus fewer late fees for parents |
| B | ≈ ₹3.6 lakh | Do it now: cheap, and it removes legal risk |
| C | ≈ ₹84 lakh | Biggest value; fixes the moment parents remember most |

**Step 8: The plan you take to leadership.**

1. **This sprint:** B (show the full price upfront).
2. **This quarter:** C (real-time confirmation), since it's the largest value and fixes the ending.
3. **Next:** A, starting with the 50 largest schools that can share class lists.
4. **Metrics:** % of parents who reach the pay step; payment completion; support contacts per 1,000 payments. **Guardrail:** wrong-child payments (a risk with name search).

Notice what the map changed. Leadership's instinct was "make the pay screen faster". The map showed the biggest pain was *after* payment, and its cause was backstage.

## Going deeper: nuances and trade-offs

### 1. The "average user" journey hides the real ones

A map that blends first-time and repeat users, or confident and nervous users, shows a smooth average that nobody actually experiences. First-time payers may struggle at "identify child"; repeat payers may sail through but worry at "confirmation".

Make one map per actor. If two segments behave very differently at the same step, that's a finding in itself. Split the map, or add a separate row for each segment at that step.

### 2. In India, many journeys are assisted and happen partly offline

Many journeys don't happen on one phone by one person. A child pays the bill for a parent. A kirana owner books a ticket for a customer. A family shares one phone. People confirm things by calling the shop or messaging on WhatsApp, and cash on delivery adds offline steps.

Put these on the map. Add an "assisted by" note where someone helps, and include offline touchpoints like calls, visits and paper circulars. A map that stops at your app's edge will miss where much of the pain lives.

### 3. Assumption maps are useful, but label them

Workshop maps built from the team's memory are quick, and they're good for surfacing disagreements. They're also where confident fiction is born. Two simple habits help:

- Colour-code each sticky note: **evidence** (with its source) vs **assumption**.
- End the workshop with a list of the three riskiest assumptions, and a plan to check each one with users or data.

### 4. Emotions need evidence too

The emotion line is the most persuasive part of a map, and the easiest to invent. Base it on what users actually showed or said:

- direct quotes from interviews
- moments of hesitation you saw in usability sessions
- short in-app ratings at specific steps
- the tone of support tickets and reviews

Emotion isn't a soft extra. In Forrester's 2026 US CX Index, the emotional side of experience made the biggest gain of the three quality dimensions it tracks. Forrester calls emotion often the strongest predictor of loyalty, and the hardest to improve ([Forrester blog, August 2026](https://www.forrester.com/blogs/emotion-leads-cx-quality-rebound-in-the-us/)).

### 5. Maps die on walls unless someone owns them

The most common fate of a journey map is a beautiful poster nobody looks at after a month. NN/g's guidance is to give each opportunity an owner and a success metric. Teams that get lasting value from maps also:

- **review them on a rhythm**, for example quarterly, and update the current state after big launches
- **link steps to live metrics**, so each phase shows its current funnel number ([A8.5](../08-product-metrics/05-funnels-cohorts-and-retention-curves.md))
- **use them in planning**, so roadmap items point to the pain point they fix ([A5.1](../05-roadmaps-and-prioritisation/01-outcome-based-roadmaps-now-next-later.md))

### 6. B2B journeys have several actors and run for months

In B2B products, one "journey" may involve a buyer who signs the contract, an admin who sets things up, and end users who use it daily. They have different goals and pains, and a decision can take months.

Map each role separately, then show where their journeys hand off to each other. Hand-offs, like "admin invites the team", are frequent pain points. Nobody owns the gap between two people's journeys.

### 7. The same map can be used to help users or to exploit them

A journey map shows exactly where users are tired, rushed or confused. That knowledge can be used to remove friction. It can also be used to slip in extras, hide fees or make cancelling hard. Those tactics are called **dark patterns**.

In India, this isn't only an ethics question. The Central Consumer Protection Authority's 2023 guidelines name specific dark patterns, including false urgency, basket sneaking, subscription traps and drip pricing (see the case below). A good habit: for every opportunity on your map, ask "Would we be comfortable if the user saw exactly why we made this change?"

### 8. How experienced PMs actually use maps

Experienced PMs rarely make giant wall-sized maps. More often they:

- sketch a quick current-state map in the first week of a new product area, to learn the territory
- make a focused map of one painful phase (for example, "the first 10 minutes"), not the whole lifecycle
- use an empathy map to align a new team or a sceptical leader around real user evidence
- pull a service blueprint only when the pain is backstage
- reuse the map as a storytelling tool in reviews: "here's where users drop, here's why, here's our fix"

## Real-world examples (2023 onwards)

!!! example "India's consumer regulator, 2023–2025: the checkout journey becomes a legal matter"
    On 30 November 2023, India's Central Consumer Protection Authority (CCPA) notified the *Guidelines for Prevention and Regulation of Dark Patterns, 2023*. They apply to platforms offering goods or services in India, and to advertisers and sellers. The guidelines name specific tactics, including false urgency, basket sneaking, confirm shaming, subscription traps, interface interference, bait and switch, and drip pricing ([SCC Online summary](https://www.scconline.com/blog/post/2023/12/04/ccpa-notifies-guidelines-for-prevention-and-regulation-of-dark-patterns-2023-legal-news/)). In June 2025, the CCPA went further: it asked e-commerce platforms to self-audit for dark patterns within three months and to submit self-declarations that their platforms were free of them ([Storyboard18 report](https://www.storyboard18.com/amp/digital/ccpa-warns-e-comm-firms-over-dark-patterns-self-audit-within-3-months-69249.htm)).

    **PM lesson:** most of these patterns live at particular steps of a journey. Drip pricing sits at checkout, subscription traps at cancellation, basket sneaking just before payment. A current-state journey map, walked through with a "would the user feel tricked here?" lens, is a practical way to run that kind of self-audit.

!!! example "Airbnb, April 2025: fixing the moment of price surprise"
    From 21 April 2025, Airbnb began showing every guest the total price of a stay, including fees and taxes, from the start of their search, instead of a nightly rate that grew at checkout. The move came ahead of a US Federal Trade Commission rule on hidden fees taking effect in May. Airbnb said nearly 17 million guests had used an optional total-price toggle since 2022, and that in 2023 nearly 300,000 listings removed or reduced their fees after the tool launched ([ABC News report](https://abc13.com/post/airbnb-will-now-show-total-prices-default/16216095/)).

    **PM lesson:** a price that grows between search and checkout creates an emotional low right at the moment of decision. Fixing it changed behaviour on *both* sides of the marketplace: hosts cut fees once guests could compare total prices. Journey maps for marketplaces should include both the buyer's and the seller's journey.

## Common mistakes

!!! warning "Watch out for"
    - **Mapping "all users" on one map.** One actor, one scenario. Otherwise the map describes nobody.
    - **Stopping at the app's edge.** Calls, WhatsApp messages, paper circulars and visits are part of the journey.
    - **Inventing the emotion line.** Base it on quotes, observation and data, and mark assumptions.
    - **Mixing current and future state** on one map. You can't tell problems from plans.
    - **No numbers.** Size each pain point with funnel data or ticket counts, so you can rank them.
    - **No owners.** An opportunity without an owner and a metric won't get fixed.
    - **Polishing the middle, ignoring the end.** Endings shape memory; check the last step first.
    - **Treating the map as finished.** Update it after major launches, or it will mislead new team members.

## Common questions

**What's the difference between a journey map and a user flow?**
A user flow shows screens and taps inside your product. A journey map shows the person's whole experience towards a goal, including thoughts, feelings and steps outside your product. Use flows for designing screens and journey maps for finding problems.

**How long should making a journey map take?**
A focused current-state map can be drafted in a 2–3 hour workshop if research already exists. Gathering good evidence is the slow part, often one to three weeks. A map built in an afternoon without research is a hypothesis, not a finding.

**Do I need a designer or researcher to make one?**
It helps, but PMs make them often. What matters is mixing roles in the room, including engineering, design, support and sometimes sales. Different people know different parts of the journey.

**Should every product have a journey map?**
No. Make one when a problem spans several steps, channels or teams, or when the team disagrees about where users struggle. For a simple single-screen tool, a user flow and good analytics may be enough.

**Can AI tools make journey maps for me?**
They can draft structure and summarise interview notes quickly. But a map invented from a model's general knowledge describes a generic user, not yours. Early research suggests AI-simulated customers behave differently from real ones at exactly the moments that matter, such as walking away (see Research happening now).

## In the interview

!!! question "In the interview"
    **How it's tested:** journey thinking appears inside product sense and design questions ([A12.2](../12-career-and-interviews/02-product-sense-and-design-interviews-circles.md)). Interviewers ask you to "walk through the user's experience" before proposing features. They want to see that you pick one user, think end to end (including offline steps), and focus on the biggest pain.

    **Sample question:** *"How would you improve the experience of booking a cab from an Indian airport?"*

    **Outline of a strong answer:**

    1. **Pick an actor:** for example, a first-time traveller arriving late at night, with a heavy bag and low phone battery.
    2. **Walk the journey in phases:** land → collect bags → find network and book → find the pickup point → meet the driver → ride → pay → arrive.
    3. **Mark thoughts and emotions:** "Is this cab safe?" "Where is pickup zone C?" "Why did the price change?"
    4. **Pick the moments that matter:** finding the pickup point and meeting the driver (high anxiety), and the final fare (the ending).
    5. **Propose 2–3 solutions tied to those moments:** indoor wayfinding to the pickup point, a matching code shown on both phones, the fare locked at booking.
    6. **Add metrics and a guardrail:** time from booking to pickup, rides cancelled after booking, safety-report rate.

    Interviewers listen for one clear user, an end-to-end view, prioritising by pain rather than by feature ideas, and metrics.

## Research happening now

!!! info "Research happening now"
    - **Emotion leads the US customer-experience rebound (Forrester, August 2026).** Forrester's 2026 CX Index found US customer experience quality rose for the first time since 2021, with emotion making the biggest gain of its three dimensions. Among 225 brands measured in both 2025 and 2026, 26% improved significantly and 7% declined, and scores remain slightly below 2024 levels ([Forrester blog](https://www.forrester.com/blogs/emotion-leads-cx-quality-rebound-in-the-us/)). *Status: industry index of US brands; full report is paid.*
    - **"Simulated customers never walk away" (June 2026).** Liang Chen compared AI-simulated customers with 2,790 real conversations between an AI sales agent and customers, 793 of them with verified purchase outcomes. Simulated non-buyers kept engaging and asking about price where real ones said "not now" and left; expressed resistance fell from 25.1% to 13.5% ([arXiv preprint](https://arxiv.org/abs/2606.20708)). *Status: single-author preprint, not peer-reviewed.* For journey mapping, the warning is clear: the drop-off moments you most need to see are the ones simulated users are worst at showing.

## Try it yourself (25 minutes)

Pick a journey you did recently: ordering medicine online, recharging a metro card, or renewing vehicle insurance.

1. Write the actor and scenario in one sentence.
2. List 5–7 phases, including at least one step outside the app.
3. For each phase, write one action, one thought and an emotion score from −2 to +2.
4. Circle the two biggest lows, and look at the ending.
5. For each low, write one opportunity, a metric that would show it improved, and whether the fix is front stage (screens) or backstage (processes, systems).
6. Make a quick empathy map for yourself at the worst moment: says, does, thinks, feels.

??? success "Check your answer"
    For "ordering medicine online", a good answer might look like this:

    - **Actor and scenario:** "A 35-year-old orders a parent's monthly blood-pressure medicine on a phone, with a paper prescription."
    - **Phases:** search medicine → upload prescription → wait for pharmacist check → pay → wait for delivery → receive and check.
    - **Biggest lows:** waiting with no update after uploading the prescription (−2, "Was it rejected?"), and a substitute brand arriving without warning (−2, at the end).
    - **Opportunities:**
        - Show the prescription-check status with an expected time. Metric: % of orders cancelled during verification. Front stage, plus a backstage fix to the pharmacist queue.
        - Ask before substituting a brand. Metric: substitute-related complaints. Backstage process change.
    - **Empathy map at the worst moment:** says "Is my order even placed?"; does: checks the app repeatedly; thinks "I should have gone to the chemist"; feels anxious.

    Self-check: did you include an offline step, base emotions on what you actually felt, look at the ending, and name a metric for each opportunity?

## How this connects

- [A1.2 User research methods and interviews](02-user-research-methods-and-interviews.md): where the evidence for every row of a map comes from.
- [A1.3 Personas and Jobs-to-be-Done](03-personas-and-jobs-to-be-done.md): personas give you the actor; jobs give you the scenario.
- [A2.1 Continuous discovery and opportunity solution trees](../02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md): the lows on a map become opportunities on the tree.
- [A6.2 User story mapping](../06-product-design-and-ux/02-user-story-mapping.md): turns a journey into a plan for what to build, release by release.
- [A8.5 Funnels, cohorts and retention curves](../08-product-metrics/05-funnels-cohorts-and-retention-curves.md): puts numbers on each step of the journey.

## Go deeper

- **Article:** [NN/g: Journey Mapping 101](https://www.nngroup.com/articles/journey-mapping-101/). The clearest short guide to the parts of a journey map and how it differs from related maps.
- **Video:** [NN/g: Customer Journey Mapping 101](https://www.nngroup.com/videos/journey-mapping-101/). A short video version for sharing with your team.
- **Video:** [NN/g: Common journey mapping mistakes](https://www.nngroup.com/videos/common-journey-mapping-mistakes/). Worth watching before your first workshop.
- **Article:** [NN/g: Empathy mapping](https://www.nngroup.com/articles/empathy-mapping/). How to run an empathy-mapping session and use the four quadrants.
- **Article:** [Dave Gray: The updated empathy map canvas](https://medium.com/the-xplane-collection/46df22df3c8a). The creator explains why he added goals, sees, hears, pains and gains.
- **Article:** [NN/g: Service blueprints definition](https://www.nngroup.com/articles/service-blueprints-definition/). When the pain is backstage, this is the next tool.
- **Book:** [*Mapping Experiences*](https://www.oreilly.com/library/view/mapping-experiences-2nd/9781492076629/) by Jim Kalbach (2nd edition, O'Reilly). A complete guide to journey maps, blueprints and related diagrams, and to using them for alignment.

## Key takeaways

- A **journey map** shows the steps, thoughts and feelings of **one actor in one scenario**. An **empathy map** shows what that user **says, does, thinks and feels**.
- Map the **whole journey**, including offline and assisted steps, not just your screens.
- Keep **current state** and **future state** separate. Find problems first, then design the target.
- Look for **moments that matter**: the sharpest lows and the **ending**, which users remember most.
- **Size every pain point with data** and turn each into an opportunity with an **owner and a metric**.
- When the pain is behind the scenes, use a **service blueprint**.
- The same map can remove friction or exploit it. **Don't build dark patterns**; in India, regulators now name them.

## Updates

*No updates yet.*
