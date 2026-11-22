# Glossary

Plain-English meanings of the terms used in this book, A to Z. Each entry links to the chapter where it's explained.

**AARRR (pirate metrics)**: five stages of a customer's life with your product: Acquisition, Activation, Retention, Referral, Revenue. See [A8.3](../part-a/08-product-metrics/03-aarrr-and-google-s-heart-framework.md).

**Activation**: the moment a new user first gets real value from your product (the "aha moment"). See [A8.3](../part-a/08-product-metrics/03-aarrr-and-google-s-heart-framework.md).

**Agent (AI)**: a system where a language model decides, step by step, which tools to call and when the task is done. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**Agent inbox**: one screen listing everything AI agents need from you (approvals, questions, alerts), modelled on an email inbox. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Agent loop**: the cycle an AI agent repeats: think, call a tool, read the result, decide the next step. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**Ambient AI**: AI that runs in the background and starts work when an event happens (a new ticket, an overdue invoice), rather than when a user asks. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Anti-persona**: a description of a user you deliberately are not building for, so the team doesn't optimise for them. See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Approval fatigue**: when users are asked to approve AI actions so often that they click "yes" without really checking. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Articulation barrier**: the difficulty many people have in describing what they want in words, which makes typed prompts hard to use. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Assumption mapping**: plotting assumptions on importance × evidence to find the riskiest ones to test first (David Bland). See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Assumption types (discovery)**: the five kinds of belief a solution depends on: desirability, viability, feasibility, usability and ethical. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Attitudinal vs behavioural research**: what people *say* (opinions, beliefs) vs what people *do* (actions you can observe or log). See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Augmentation (AI)**: AI helps a person do a task better or faster while the person stays in control and makes the final call. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Automation (AI)**: AI does the task for the user, ideally with a way to preview, edit or undo. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Automation bias**: people trusting an automated suggestion too much and approving it without really checking. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Autonomy ladder (AI)**: the steps from AI that only suggests, to AI that drafts for review, acts then reports, or acts silently. Set per action. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Background error (AI)**: an AI mistake that nobody notices, so it only shows up in evals, audits or sampling. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Batch processing (AI APIs)**: sending AI work that can wait (like overnight jobs) in bulk, usually at a big discount. See [B0.3](../part-b/00-foundations/03-choosing-models-capability-cost-latency-open-vs.md).

**Battlecard**: a one-page guide for sales on how to compete against a specific rival: what buyers believe, questions to ask, proof to show. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Beachhead market**: the first small, specific group of customers a product aims to win completely. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Bottom-up sizing**: estimating a market by counting real buyers and multiplying by what each would pay. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Break-even accuracy**: the AI accuracy below which checking and fixing its output costs more than doing the task by hand. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Build trap**: when a company measures success by how much it ships rather than by the value it creates (Melissa Perri). See [A2.4](../part-a/02-problem-discovery/04-outcomes-over-outputs-escaping-the-build-trap.md).

**CAC (customer acquisition cost)**: what you spend to win one new customer. See [A8.3](../part-a/08-product-metrics/03-aarrr-and-google-s-heart-framework.md).

**Calibrated trust**: users trust an AI as much as its real accuracy deserves: more where it's good, less where it's weak. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Canary case**: a known-wrong AI output slipped into a review queue to check that human reviewers still catch errors. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Capability eval vs regression eval**: a capability eval checks whether the AI can do something hard yet (starts with a low pass rate); a regression eval checks it still does what it used to (should stay near 100%). See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Catastrophic forgetting**: a fine-tuned model getting worse at skills it wasn't trained on during fine-tuning. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

**Chain of thought**: getting an AI model to work through a problem step by step before answering. Helps some models; adds delay on reasoning models. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

**Chunk**: a small piece of a document (often a few hundred tokens) stored and retrieved on its own in a RAG system. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Cohort**: a group of users who share a start point, such as everyone who signed up in the same week. See [A8.5](../part-a/08-product-metrics/05-funnels-cohorts-and-retention-curves.md).

**Competitive alternatives**: everything a customer would use if your product didn't exist, including doing nothing (April Dunford). See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Concierge test**: delivering a service by hand to a few customers who know it's manual, before building software. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Confidence threshold**: a cut-off score above which the AI acts on its own and below which a human decides. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Containment rate**: share of conversations an AI handled without a human; not the same as solving the problem. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Context engineering**: choosing everything that goes into an AI model's input on each step (instructions, documents, history, tool results), not just the written prompt. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

**Context window**: the maximum amount of text (in tokens) an AI model can look at in one request, including instructions, conversation and documents. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**Continuous discovery**: small, weekly customer touchpoints (interviews, prototype tests, experiments) by the team building the product, aimed at a clear outcome. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Contribution margin**: revenue from an order minus its direct variable costs (delivery, payment fees, discounts). See [A8.4](../part-a/08-product-metrics/04-lean-analytics-one-metric-that-matters-and-stage.md).

**Conway's law**: organisations tend to build products that mirror their own team structure and communication lines. See [A0.2](../part-a/00-the-pm-role/02-product-teams-the-trio-empowered-vs-feature-team.md).

**Copilot (pattern)**: AI that sits inside the user's own work and offers suggestions in context while the user stays in charge. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Cost per successful task**: total AI cost divided by tasks that actually succeeded, ideally including human fallback. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Counter metric (guardrail metric)**: a metric you watch to make sure improving one number isn't quietly hurting something else. See [A8.2](../part-a/08-product-metrics/02-north-star-metric-and-metric-trees.md).

**Criteria drift**: the way people's grading standards change as they read more AI outputs, so the first rubric is rarely the final one. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Cross-functional team**: a team that mixes skills (product, design, engineering, data) so it can build end to end. See [A0.2](../part-a/00-the-pm-role/02-product-teams-the-trio-empowered-vs-feature-team.md).

**Curse of knowledge**: once you know something, it's hard to imagine not knowing it, which makes experts poor judges of what confuses beginners. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

**Dark pattern**: a design that tricks or pressures users into something they didn't intend, like hidden fees or hard-to-cancel subscriptions. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**Data flywheel**: a loop where product use creates data, data improves the product, and a better product brings more use. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**Data moat**: a lasting advantage from data rivals can't easily get and that keeps improving your product. Rarer than claimed. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**Data provenance**: where a piece of data came from, under what permission, and what has been done to it. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**DAU / MAU**: daily active users / monthly active users. DAU ÷ MAU shows how often people come back ("stickiness"). See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**Degenerate feedback loop**: when a model's own outputs shape the data it later learns from, so its mistakes or biases grow. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**Delivery**: the work of building and shipping a product well: planning, building, testing and launching. See [A0.1](../part-a/00-the-pm-role/01-what-a-pm-actually-does.md).

**Desired outcome**: the one measurable change a product team is trying to cause, such as a higher renewal rate; the root of an opportunity solution tree. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Deterministic software**: software that gives the same output for the same input every time, because people wrote the rules. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Direct vs indirect competitor**: direct: same job, same customer, similar product. Indirect: a different kind of product solving the same job. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Discovery**: the work of figuring out what to build by understanding problems and testing ideas cheaply before full building. See [A0.1](../part-a/00-the-pm-role/01-what-a-pm-actually-does.md).

**Discussion guide**: the plan for a user interview: goals, main questions and follow-up prompts. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Distillation**: using a large model's good answers to train a smaller, cheaper model for one task. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

**DPO (direct preference optimisation)**: fine-tuning with pairs of a better and a worse answer, so the model learns which you prefer. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

**Drift**: quality slowly changing over time because users, data or the model changed. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Drip pricing**: showing a low price first and adding fees step by step until checkout; named as a dark pattern in India's 2023 guidelines. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**Embedding**: a list of numbers that captures the meaning of a piece of text, so similar meanings sit close together. Used for meaning-based search. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Empathy (in product work)**: understanding a user's situation, feelings and goals from their point of view, well enough to predict what they'll do. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

**Empathy map**: a one-page picture of what one type of user says, does, thinks and feels. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**Empowered product team**: a team handed a problem and a target outcome, trusted to find the best solution, and judged on results. See [A0.2](../part-a/00-the-pm-role/02-product-teams-the-trio-empowered-vs-feature-team.md).

**Error analysis**: reading real AI traces, noting what went wrong, and grouping the notes into failure modes you can count. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Escalation (AI handoff)**: passing a case from an AI to a human, with the context the human needs. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Eval (evaluation)**: a repeatable test that scores an AI's outputs across many real examples. See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**Explicit feedback**: feedback users give on purpose, such as thumbs up/down, ratings or 'report a problem'. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**Failure mode**: one specific, named way an AI feature goes wrong, such as promising a refund time the policy doesn't allow. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Faithfulness (grounding)**: whether an AI answer sticks to what its retrieved sources actually say. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Fake door test**: showing a button or offer for something not yet built, to measure how many people try it, then explaining honestly. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Feature factory**: a team that turns out features on demand without checking whether they work. See [A2.4](../part-a/02-problem-discovery/04-outcomes-over-outputs-escaping-the-build-trap.md).

**Feature team**: a team handed a roadmap of features to build and judged mainly on shipping them. See [A0.2](../part-a/00-the-pm-role/02-product-teams-the-trio-empowered-vs-feature-team.md).

**Few-shot prompting**: including a few worked examples in a prompt to show the model what good output looks like. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

**Fine-tuning**: training an existing model further on your own examples so a behaviour is built into the model. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

**Five Whys**: asking "why?" about five times to dig from a symptom towards a root cause; credited to Toyota. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Follow-me-home**: watching a user do a real task in their own setting instead of asking them about it; a practice made well known by Intuit. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

**Four forces of progress**: push and pull that drive someone to switch products; anxiety and habit that hold them back (Moesta and Spiek). See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Four risks**: value, usability, feasibility and viability, the four ways a product idea can fail (Marty Cagan). See [A0.1](../part-a/00-the-pm-role/01-what-a-pm-actually-does.md).

**Funnel**: the series of steps a user takes toward a goal, showing how many drop off at each step. See [A8.5](../part-a/08-product-metrics/05-funnels-cohorts-and-retention-curves.md).

**Generative vs evaluative research**: research to discover problems and opportunities vs research to check whether a specific design works. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Golden dataset**: a set of real or realistic test cases with agreed correct answers or pass/fail labels. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Goodhart's law**: when a measure becomes a target, people game it and it stops being a good measure. See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**Graceful failure**: when an AI can't help, it fails safely and clearly and offers the user a next step. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Grader (eval)**: whatever scores an AI's answer in an eval: code, another AI model, or a person. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Ground truth**: the verified correct answer for a case, confirmed by an expert or a real-world outcome. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**Hallucination**: when an AI states something false as if it were true. See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**HEART**: Google's user-experience metric framework: Happiness, Engagement, Adoption, Retention, Task success. See [A8.3](../part-a/08-product-metrics/03-aarrr-and-google-s-heart-framework.md).

**How Might We (HMW)**: a question that turns a problem into an open invitation for ideas, e.g. "How might we help first-time sellers finish their listing?" See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Human-in-the-loop**: a design where a person checks, approves or corrects the AI's work before it matters. See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**Human-on-the-loop**: the AI acts on its own while a person monitors and can step in or stop it. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Hybrid search**: running keyword search and meaning-based (embedding) search together and merging the results. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Impact (business)**: the big business result that outcomes add up to, such as revenue, profit or market share. See [A2.4](../part-a/02-problem-discovery/04-outcomes-over-outputs-escaping-the-build-trap.md).

**Implicit feedback**: what users' actions reveal about an AI answer: copying, editing, retrying, giving up or asking for a human. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Inference**: one run of an AI model to produce an answer; each run has a cost. See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**Input metric**: a number your team can move directly that drives a bigger result. See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**Insight**: a non-obvious truth about users that explains what you observed and points to a decision. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

**Intent-based outcome specification**: Jakob Nielsen's name for the AI interface style where you say what result you want and the computer works out the steps. See [B2.2](../part-b/02-discovery-and-design/02-ai-ux-patterns-chat-copilot-agent-ambient.md).

**Interview snapshot**: a one-page summary of a single customer interview, made right after it: who, a key quote, the story and the opportunities heard. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Jagged frontier**: AI being excellent at some tasks and surprisingly weak at others that look similar or easier. See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**Job story**: a need written as "When [situation], I want to [motivation], so I can [outcome]." See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Jobs-to-be-done (JTBD)**: the progress a person is trying to make in a particular situation; they "hire" a product to get it. See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Journey map**: a picture of the steps one person takes to reach a goal, with what they do, think and feel at each. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**Keep-the-lights-on (KTLO) work**: necessary work that keeps a product running (fixes, upgrades, compliance) but isn't aimed at a new outcome. See [A2.4](../part-a/02-problem-discovery/04-outcomes-over-outputs-escaping-the-build-trap.md).

**Labelling (annotation)**: people marking data with the right answer or category so it can be used to train or test AI. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**Lagging metric**: a number that shows results after the fact (e.g. revenue, churn). See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**Latency**: how long a user waits for a response, often split into time to first token and total response time. See [B0.3](../part-b/00-foundations/03-choosing-models-capability-cost-latency-open-vs.md).

**Leading metric**: an early signal that predicts a future result. See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**Leading question**: an interview question that hints at the answer you want ("Wouldn't it be easier if…?"). See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Least privilege**: giving an agent or system only the permissions a task needs, and no more. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**Lethal trifecta**: an AI agent with private data, exposure to untrusted content and a way to communicate externally: the combination that enables data leaks (Simon Willison). See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**LLM (large language model)**: a model trained on huge amounts of text to predict the next token; the engine behind tools like ChatGPT, Claude and Gemini. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**LLM-as-judge**: using a language model to grade another AI's output against specific criteria; it must be checked against human labels. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**LoRA (low-rank adaptation)**: a cheap fine-tuning method that trains small add-on pieces instead of the whole model. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

**LTV (lifetime value)**: the total profit you expect from one customer over their whole relationship with you. See [A8.3](../part-a/08-product-metrics/03-aarrr-and-google-s-heart-framework.md).

**MCP (Model Context Protocol)**: an open standard for connecting AI apps to tools and data, so one integration works across many AI apps. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**Metric tree**: a diagram that breaks one big metric into the smaller metrics that add or multiply up to it. See [A8.2](../part-a/08-product-metrics/02-north-star-metric-and-metric-trees.md).

**Mix shift**: an average changing because the share of each user segment changed, not their behaviour. See [A8.6](../part-a/08-product-metrics/06-diagnosing-a-metric-drop.md).

**Model routing**: sending each request to a different AI model depending on how hard or important it is, to save cost and time. See [B0.3](../part-b/00-foundations/03-choosing-models-capability-cost-latency-open-vs.md).

**Moment that matters**: a step in a journey that strongly shapes how users feel about the whole experience. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**MVP (minimum viable product)**: the smallest thing you can put in front of real users to learn whether they'll use or pay for it (Eric Ries). See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**North Star metric**: the one number that best captures the value customers get from your product. See [A8.2](../part-a/08-product-metrics/02-north-star-metric-and-metric-trees.md).

**NRR (net revenue retention)**: this year's revenue from last year's customers ÷ their revenue last year; above 100% means existing customers grew. See [A8.5](../part-a/08-product-metrics/05-funnels-cohorts-and-retention-curves.md).

**OMTM (One Metric That Matters)**: the single number a team focuses on for the current stage of the business (from *Lean Analytics*). See [A8.4](../part-a/08-product-metrics/04-lean-analytics-one-metric-that-matters-and-stage.md).

**Online eval**: an automatic quality check run on a sample of real production traffic. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Open-weight model**: an AI model whose trained weights you can download and run yourself; a closed model is only available through its maker's API or app. See [B0.3](../part-b/00-foundations/03-choosing-models-capability-cost-latency-open-vs.md).

**Opportunity (discovery)**: an unmet customer need, pain point or desire, phrased in the customer's words; not a feature. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Opportunity solution tree (OST)**: Teresa Torres's visual map linking one desired outcome to customer opportunities, the solutions for them, and the assumption tests for each solution. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Outcome vs output**: an outcome is a change in customer behaviour or business results; an output is something the team produced, like a feature. See [A0.1](../part-a/00-the-pm-role/01-what-a-pm-actually-does.md).

**Pain point**: a moment where a user is confused, slowed down, worried or annoyed. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**pass@k and pass^k**: pass@k: the AI succeeds at least once in k tries; pass^k: it succeeds every time in k tries. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Payback period**: how long a customer's profit takes to repay the cost of acquiring them. See [A8.4](../part-a/08-product-metrics/04-lean-analytics-one-metric-that-matters-and-stage.md).

**Peak–end rule**: people judge an experience mostly by its most intense moment and its ending. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**Penetration**: the share of possible customers who actually use a kind of product. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Persona**: a short, research-based description of one type of user: goals, behaviours, context and frustrations. See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Pilot purgatory**: when an AI project works in a demo or pilot but never reaches real use or measurable value. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Point-of-view (POV) statement**: a design-thinking format for a problem: user + need + insight. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Positioning map (perceptual map)**: a chart placing options on two dimensions customers care about, to reveal gaps. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Pretotyping**: Alberto Savoia's term for faking a product cheaply to test whether people will really use it, before building a prototype. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Pretraining**: the first, most expensive stage of building an LLM, where it learns to predict the next token across vast amounts of text. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**Probabilistic**: producing a likely guess that can vary and can be wrong, as most AI does (the opposite of deterministic). See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**Problem statement**: a short, evidence-backed description of who is struggling, in what situation, why, and how you'll know it's fixed, without naming a solution. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Product kata**: Melissa Perri's routine for working towards an outcome: direction, current state, target condition, obstacles, experiments, repeat. See [A2.4](../part-a/02-problem-discovery/04-outcomes-over-outputs-escaping-the-build-trap.md).

**Product manager (PM)**: the person responsible for deciding what a team builds and why, and for whether it creates value. See [A0.1](../part-a/00-the-pm-role/01-what-a-pm-actually-does.md).

**Product operations (product ops)**: a team that gives PMs shared tools, data and processes so they can spend more time on customers. See [A0.3](../part-a/00-the-pm-role/03-product-vs-project-vs-program-management-types-o.md).

**Product owner**: in Scrum, the one person accountable for maximising the value of the team's work; often a hat the PM wears. See [A0.3](../part-a/00-the-pm-role/03-product-vs-project-vs-program-management-types-o.md).

**Product trio**: the PM, designer and tech lead working together as one decision-making team. See [A0.1](../part-a/00-the-pm-role/01-what-a-pm-actually-does.md).

**Program**: a group of related projects managed together to achieve a benefit none could achieve alone. See [A0.3](../part-a/00-the-pm-role/03-product-vs-project-vs-program-management-types-o.md).

**Project**: a temporary piece of work with a start, an end and a defined result. See [A0.3](../part-a/00-the-pm-role/03-product-vs-project-vs-program-management-types-o.md).

**Prompt injection**: an attack where text from a user or a document tricks an AI model into ignoring its instructions. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

**Proto-persona**: a persona drafted from the team's assumptions before research; a hypothesis to test. See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Prototype fidelity**: how close a prototype looks and behaves to the real product, from paper sketch to near-real. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Proxy metric**: a number tracked because the real thing (like happiness) is hard to measure directly. See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**RAG (retrieval-augmented generation)**: finding relevant text from your own documents and adding it to the prompt so the model can answer from it. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Reasoning model**: an AI model that produces hidden step-by-step "thinking" before answering; better on hard problems, slower and costlier. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**Recall@k**: how often the right document or chunk appears in the top *k* search results across a test set. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Reframing**: looking at a problem from a different angle (for example "the wait is annoying" instead of "the elevator is slow") so new solutions appear. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Reranker**: a second model that re-reads the top search results and orders them by real relevance. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Retention**: the share of users who keep coming back over time. See [A8.5](../part-a/08-product-metrics/05-funnels-cohorts-and-retention-curves.md).

**Riskiest assumption**: the belief behind an idea that is most important and has the least evidence; test it first. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**RLHF (reinforcement learning from human feedback)**: training a model towards answers that people ranked as better. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**Root cause**: the underlying reason a problem happens, as opposed to its visible symptom. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Rule of Two (agents)**: Meta's guideline that an agent session should have at most two of: untrusted input, sensitive data access, and the ability to act externally. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**SAM (serviceable available market)**: the part of the TAM your product, price, language and reach can serve today. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Saturation (research)**: the point where new interviews stop teaching you anything new. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Say–do gap**: the difference between what people say they do and what they actually do. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

**Screener**: a short questionnaire used to recruit the right research participants. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Service blueprint**: a journey map extended to show the staff, processes and systems behind each step. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**SFT (supervised fine-tuning)**: fine-tuning with input and ideal-output pairs. See [B1.4](../part-b/01-building-blocks/04-prompting-vs-rag-vs-fine-tuning-how-to-decide.md).

**Simpson's paradox**: every segment moves one way while the total moves the other way, usually because of a mix shift. See [A8.6](../part-a/08-product-metrics/06-diagnosing-a-metric-drop.md).

**Solution in disguise**: a request that names a feature ("add a leaderboard") instead of the problem behind it. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**SOM (serviceable obtainable market)**: the part of the SAM you can realistically win in the next few years. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Span**: one step inside a trace, such as a single model call or tool call. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Status quo (competitor)**: the customer carrying on with what they do today; often the alternative that wins most deals. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Story-based interviewing**: asking participants about a specific past event ("Tell me about the last time…") instead of general opinions. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**Structured output**: AI output in a fixed, machine-readable shape (such as JSON with named fields) that code can check and use. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

**Success threshold**: the number, set before a test, that decides whether the assumption passed. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Switch interview**: a jobs-to-be-done interview about the moment someone recently switched to or from a product. See [A1.3](../part-a/01-understanding-users-user-sense/03-personas-and-jobs-to-be-done.md).

**Switching cost**: what a customer loses or must redo to change products: money, data, learning, risk. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Synthetic data**: data generated by a model or program rather than collected from real people or events. See [B4.1](../part-b/04-data-safety-and-law/01-data-strategy-and-feedback-loops.md).

**System prompt**: standing instructions a product team writes for an AI model, applied to every conversation. See [B1.1](../part-b/01-building-blocks/01-prompt-engineering-for-pms.md).

**Table stakes**: features every option must have just to be considered; missing them loses deals, having them doesn't win them. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**TAM (total addressable market)**: everyone who could ever pay for this kind of product, if you had no limits. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Temperature**: a setting that controls how varied an AI model's answers are; low is predictable, high is creative. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**Time to first token (TTFT)**: seconds from sending a request to an AI model until the first word of the reply arrives. See [B0.3](../part-b/00-foundations/03-choosing-models-capability-cost-latency-open-vs.md).

**Token**: a small chunk of text that AI models read and write; providers usually charge per token. See [B0.1](../part-b/00-foundations/01-what-makes-ai-products-different.md).

**Tool use (function calling)**: a model asking your software to run a named function and reading back the result. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**Top-down sizing**: estimating a market by starting from a big published number and cutting it down with percentages. See [A3.1](../part-a/03-market-research/01-market-sizing-tam-sam-som.md).

**Touchpoint**: any place a user meets your product or company: a screen, an SMS, a call, a delivery person. See [A1.4](../part-a/01-understanding-users-user-sense/04-journey-maps-and-empathy-maps.md).

**TPM (technical program manager)**: a program manager with deep technical knowledge who coordinates complex engineering work across many teams. See [A0.3](../part-a/00-the-pm-role/03-product-vs-project-vs-program-management-types-o.md).

**Trace (AI)**: the full record of one AI interaction: the input, every step and tool call, and the final answer. See [B3.1](../part-b/03-quality/01-evals-the-ai-pm-s-most-important-skill.md).

**Transformer**: the model design behind almost all modern LLMs, built around "attention" to earlier tokens. See [B0.2](../part-b/00-foundations/02-how-llms-work-for-pms.md).

**TTFT (time to first token)**: how long before the first word of an AI answer appears. See [B3.2](../part-b/03-quality/02-ai-product-metrics-and-production-monitoring.md).

**Two-pizza team**: Amazon's idea that a team should be small enough for two pizzas to feed, ideally under ten people. See [A0.2](../part-a/00-the-pm-role/02-product-teams-the-trio-empowered-vs-feature-team.md).

**Two-way door decision**: a decision that is easy to reverse, so it should be made quickly; a one-way door is hard to undo and deserves more care. See [A2.1](../part-a/02-problem-discovery/01-continuous-discovery-and-opportunity-solution-tr.md).

**Undertrust**: users ignore or redo an AI's work even when it's right, so it adds no value. See [B2.3](../part-b/02-discovery-and-design/03-designing-for-trust-failure-and-human-in-the-loo.md).

**Usability test**: watching someone try real tasks with a product or prototype, usually while thinking aloud. See [A1.2](../part-a/01-understanding-users-user-sense/02-user-research-methods-and-interviews.md).

**User sense**: the trained ability to predict how real users will behave and feel, built from regular contact with them. See [A1.1](../part-a/01-understanding-users-user-sense/01-building-user-sense-and-empathy.md).

**Vanity metric**: a number that looks good but doesn't help you make a decision (e.g. total downloads ever). See [A8.1](../part-a/08-product-metrics/01-metric-basics-leading-lagging-input-output-vanit.md).

**Vector database**: a store built to quickly find the chunks whose embeddings are closest to a question's embedding. See [B1.2](../part-b/01-building-blocks/02-rag-giving-ai-your-knowledge.md).

**Verification cost**: the time and skill a person needs to check whether an AI output is right. See [B2.1](../part-b/02-discovery-and-design/01-finding-ai-opportunities-and-when-not-to-use-ai.md).

**Viral coefficient (K)**: new users each existing user brings in = invites sent per user × invite conversion rate. See [A8.3](../part-a/08-product-metrics/03-aarrr-and-google-s-heart-framework.md).

**Why–how ladder**: asking "why?" to broaden a problem towards the user's goal, or "how?" to narrow it towards solutions. See [A2.2](../part-a/02-problem-discovery/02-framing-the-problem-problem-statements.md).

**Win-loss analysis**: interviewing buyers after a decision to learn why they chose you or a rival. See [A3.2](../part-a/03-market-research/02-competitive-analysis.md).

**Wizard of Oz test**: a real-looking product where humans secretly do the work behind the screen. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

**Workflow (AI)**: an AI system where your code fixes the steps in advance and the model fills in parts; the simpler alternative to an agent. See [B1.3](../part-b/01-building-blocks/03-agents-tool-use-and-mcp.md).

**XYZ hypothesis**: Savoia's format for a testable belief: at least X% of Y will do Z. See [A2.3](../part-a/02-problem-discovery/03-assumption-testing-prototypes-and-mvps.md).

