---
name: north-star-metric
description: "Define the ONE metric that best captures the value your product delivers. Candidate evaluation, input metrics, dashboard spec, and targets. Triggers: north star metric, key metric, what should I measure, most important metric, NSM, success metric, KPI."
---

# Define Your North Star Metric

You're tracking sign-ups, page views, MRR, and a dozen other numbers. But you don't know which one actually matters. A North Star Metric is the single number that, when it goes up, means your customers are getting more value from your product. Everything else is noise until you define this.

## Context

You are helping a founder define a North Star Metric for: **$ARGUMENTS**.

If the user provides details about their product, users, business model, or existing metrics, read those first. If a prior skill in this session produced relevant analysis, use that context directly.

## Why This Matters

Without a North Star Metric, you'll optimise for the wrong things. You'll celebrate sign-up spikes that don't convert, chase vanity metrics that look good but don't predict growth, and spread your attention across a dozen dashboards without knowing what to focus on.

The NSM gives you clarity. One number to check every morning. One number to make decisions against. One number that tells you if you're winning or losing.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Understand the Product's Core Value

Ask the user (if not already clear):
- What does your product do? (one sentence)
- What's the core value your product delivers? Not features - VALUE. What's the user's life or work like AFTER using your product?
- What do users DO in your product? (key actions, frequency)
- What's your business model? (free, freemium, subscription, one-time, ads)
- What metrics are you currently tracking? (anything - analytics, revenue, sign-ups)
- When a user is getting real value from your product, what does that look like? What are they doing?

### Step 2: Generate Candidate Metrics

A North Star Metric is NOT:
- Revenue (revenue is a lagging indicator - it tells you what happened, not what's happening)
- Sign-ups (vanity metric - sign-ups without activation are meaningless)
- Page views or DAU (engagement without value delivery is just time-wasting)

A North Star Metric IS:
- A measure of the VALUE your product delivers
- A leading indicator that predicts future revenue
- An action-based metric (something users DO, not something that happens to them)

**Generate 3-5 candidates using the value test.** For each, ask: "If this number goes up, does it mean customers are getting MORE VALUE from the product?"

The North Star Metric framework was developed by Sean Ellis (coined "growth hacking") and popularised by Amplitude's growth team. The core principle: your NSM should measure value delivery, not value extraction.

**Examples by product type to guide thinking:**

| Product Type | Common NSM | Why It Works |
|---|---|---|
| Task management | Tasks completed per user per week | Completing tasks = getting value |
| Invoicing | Invoices sent per user per month | Sending invoices = using the core feature |
| Habit tracker | Habits logged per user per day | Logging = actively engaging with the habit system |
| Analytics tool | Reports viewed per user per week | Viewing reports = extracting insights |
| Marketplace | Transactions completed per week | Transactions = both sides getting value |
| Social / Community | Posts or interactions per user per week | Interaction = engagement and value exchange |
| Content tool | Documents created per user per week | Creating = using the product's core function |
| Scheduling | Meetings booked per user per week | Bookings = the product doing its job |

**Research how similar products measure success (Web Search):**

Before brainstorming candidates, search for what metrics similar products track:

- `"[product type] north star metric"` or `"[product type] key metric"` - see what industry leaders use
- `"[similar product] metrics"` or `"how [competitor] measures success"` - find case studies or blog posts about their approach
- `"SaaS metrics [product type]"` - find benchmark data and common KPIs for this category

Use these examples as inspiration, not templates. Your NSM should reflect YOUR product's unique value delivery.

**For the user's product, brainstorm 3-5 candidate metrics.** Frame each as: "[action] per [user type] per [time period]".

### Step 3: Test Each Candidate Against 5 Criteria

For each candidate, score against these criteria:

| Criteria | Question | Scoring |
|---|---|---|
| **Measures value** | Does this metric go up when customers get more value? | 1 = weakly correlated, 5 = directly measures value delivery |
| **Leading indicator** | Does this predict future revenue and retention? | 1 = lagging (reports the past), 5 = strongly predictive |
| **Actionable** | Can you directly influence this metric with product changes? | 1 = too abstract to act on, 5 = clear levers to pull |
| **Simple** | Can you explain this metric in one sentence? Would a new team member understand it? | 1 = requires a paragraph, 5 = instantly clear |
| **Connected to revenue** | Is there a clear chain: this metric up -> retention up -> revenue up? | 1 = no clear connection, 5 = obvious causal chain |

**Score all candidates:**

| Candidate Metric | Value | Leading | Actionable | Simple | Revenue | Total |
|---|---|---|---|---|---|---|
| [metric 1] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |
| [metric 2] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |
| [metric 3] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |
| [metric 4] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |
| [metric 5] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |

Score honestly. If there's no evidence that a metric predicts revenue, don't score it 4. Document reasoning for any score of 4-5 or 1-2.

**Select the highest-scoring metric as the NSM.** If two tie, prefer the one that's simpler and more actionable (per CONVENTIONS.md tiebreaker rules).

### Step 4: Define Input Metrics

Input metrics are the 3-4 levers that DRIVE the North Star Metric. These are what you work on day-to-day.

Think of it as a tree:
```
North Star Metric
  |
  +-- Input metric 1 (e.g., new user activation rate)
  +-- Input metric 2 (e.g., feature X usage rate)
  +-- Input metric 3 (e.g., return visit frequency)
  +-- Input metric 4 (e.g., completion rate of key action)
```

**For each input metric, define:**
- What it measures (one sentence)
- How it drives the NSM (the causal chain)
- What you can do to improve it (specific actions)
- Current value (if known) and realistic target

**Example:**
- NSM: Invoices sent per user per week
- Input 1: Activation rate (% of sign-ups who send first invoice) - drives NSM by increasing the base of active users
- Input 2: Template usage rate (% of invoices using templates) - drives NSM by reducing friction per invoice
- Input 3: Payment integration completion (% of users who connect Stripe/PayPal) - drives NSM by enabling the full workflow
- Input 4: Weekly return rate (% of activated users who return each week) - drives NSM by maintaining the sending habit

### Step 5: Build the Metrics Dashboard Spec

The founder needs to track these metrics regularly without it becoming a full-time job. Design a simple dashboard:

**Daily check (30 seconds):**
- NSM current value (today/this week/this month depending on frequency)
- NSM trend (up, down, flat vs. previous period)

**Weekly review (10 minutes):**
- NSM value + trend
- Each input metric value + trend
- Notable changes or anomalies
- One decision: what to focus on next week based on which input metric has the most room to improve

**Monthly review (30 minutes):**
- NSM over time (chart)
- Input metrics over time (chart)
- Cohort analysis: are newer cohorts performing better than older ones?
- What worked this month? What didn't?

**Tool recommendations by stage:**

| Stage | Tool | Cost | Good For |
|---|---|---|---|
| 0-100 users | Spreadsheet (Google Sheets) | Free | Manual tracking, full control, good enough to start |
| 100-1K users | PostHog (free tier) | Free up to 1M events | Event tracking, funnels, retention charts |
| 100-1K users | Mixpanel (free tier) | Free up to 20M events | More polished UI, good retention analysis |
| 1K+ users | Amplitude | Free tier available | Advanced analytics, NSM tracking built-in |

For solo founders with under 100 users: a Google Sheet updated weekly is fine. Don't over-engineer your analytics before you have enough users to make the data meaningful.

### Step 6: Set Realistic Targets

Targets should be:
- Based on current performance (improve from baseline, don't pick aspirational numbers from thin air)
- Time-bound (this month, this quarter)
- Aggressive but not delusional

**If you have current data:**
- Month 1 target: 10-20% improvement over current baseline
- Month 3 target: 30-50% improvement over starting point
- Quarter target: 2x from starting point (ambitious but achievable with focused effort)

**If you're starting from zero (no data yet):**
- Month 1: establish the baseline. Just measure it consistently.
- Month 2: identify the weakest input metric and set a 20% improvement target
- Month 3: NSM should show visible upward trend

**Attribution**: The North Star Metric framework is attributed to Sean Ellis and was developed further by the Amplitude growth team. The concept of leading vs lagging indicators is a foundational business measurement principle. The input metrics approach draws from the "metrics tree" concept used in growth engineering.

### Output Format

```
## North Star Metric: [Product Name]

**Product**: [one-sentence description]
**Date**: [today]
**Business model**: [free/freemium/subscription/etc.]

### Candidate Evaluation

| Candidate | Value | Leading | Actionable | Simple | Revenue | Total |
|---|---|---|---|---|---|---|
| [metric 1] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |
| [metric 2] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |
| [metric 3] | [1-5] | [1-5] | [1-5] | [1-5] | [1-5] | [/25] |

### North Star Metric

**NSM**: [metric name]
**Definition**: [one sentence - what it measures]
**Why this metric**: [2-3 sentences - how it captures value delivery]
**Current value**: [if known, or "to be established"]
**Targets**:
- Month 1: [target]
- Month 3: [target]
- Quarter: [target]

### Input Metrics

| Input Metric | What It Measures | Drives NSM By | Current | Target |
|---|---|---|---|---|
| [metric 1] | [definition] | [causal chain] | [value] | [target] |
| [metric 2] | [definition] | [causal chain] | [value] | [target] |
| [metric 3] | [definition] | [causal chain] | [value] | [target] |
| [metric 4] | [definition] | [causal chain] | [value] | [target] |

### Dashboard Spec

**Daily check**: [what to look at]
**Weekly review**: [what to review + decide]
**Monthly review**: [what to analyse]
**Tool**: [recommendation]
```

Save as markdown.

## Common Mistakes

- **Choosing revenue as the NSM.** Revenue is a lagging indicator. By the time revenue drops, the problem started weeks or months ago. Measure the activity that CREATES revenue.
- **Choosing a vanity metric.** Total sign-ups, page views, and app downloads feel good but don't predict success. Active usage metrics are what matter.
- **Too many metrics.** The whole point of a North Star is that it's ONE number. If you're tracking 5 "key metrics" equally, you don't have a North Star. Pick one, support it with 3-4 inputs.
- **A metric you can't influence.** "Market share" is nice to know but you can't directly act on it. Your NSM should have clear levers (the input metrics).
- **Never changing it.** Your NSM should evolve as your product matures. A pre-launch product might track "sign-ups who complete onboarding." A mature product might track "weekly active usage." Revisit quarterly.

## Notes

- For very early-stage products (under 50 users), the NSM might be as simple as "users who completed the core action this week." Don't over-engineer it.
- The NSM is a communication tool as much as a measurement tool. It aligns everyone (even if "everyone" is just you) on what matters.
- If you can't decide between two candidate metrics, run both for a month and see which one better predicts the outcomes you care about (retention, revenue, engagement).
- This skill pairs naturally with retention-audit. The NSM tells you what success looks like; the retention audit tells you where that success breaks down.

---

### Further Reading

- [The One Metric That Actually Matters for Your App](https://fantasticfounder.com) - Choosing a North Star Metric that tells you if your product is winning
