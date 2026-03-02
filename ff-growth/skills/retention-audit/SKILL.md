---
name: retention-audit
description: "Find out why users leave and what to do about it. Stage-by-stage retention diagnosis, habit loop analysis, activation metrics, and a prioritised improvement plan. Triggers: retention, churn, why users leave, user retention, churn audit, keeping users, user engagement, drop off."
---

# Run a Retention Audit

Acquiring users is expensive. Losing them is worse. If your retention is broken, every user you acquire leaks out the bottom of the bucket. This skill helps you diagnose WHERE users leave, WHY they leave, and what ONE thing to fix first.

## Context

You are helping a founder audit retention for: **$ARGUMENTS**.

If the user provides analytics data, user feedback, support tickets, or any retention metrics, read those first. If a prior skill in this session produced a north star metric, use that to frame the retention analysis.

## Why This Matters

Most indie founders focus on acquisition - getting more users in the door. But if 90% of users leave after a week, doubling your acquisition just doubles the waste. Retention is the foundation. Fix retention first, then pour users in through growth loops and referrals.

Here's the math: If you have 100 users and 80% churn in month 1, you need to acquire 80 new users per month just to stay flat. If you improve retention to 50% churn, you only need 50. That's not a small improvement - it's 37% less acquisition work for the same result.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Gather Data

Ask the user what data they have available:

**Analytics tools:**
- PostHog, Mixpanel, Amplitude, Google Analytics, or anything else?
- Can you see: daily/weekly/monthly active users, user actions, sign-up dates, last active dates?

**User feedback:**
- Any surveys, NPS scores, or feedback forms?
- App store reviews mentioning why they stopped using it?
- Support tickets or emails about frustrations?

**Cancellation data:**
- If paid: do you track why people cancel? (cancellation survey, email reply)
- If free: do you know when users go inactive?

**Usage patterns:**
- What are the key actions in your product? (creating something, completing a task, viewing a report)
- How often do engaged users do these actions? (daily, weekly, monthly)
- What's the typical session length?

### Step 2: If NO Data - Set Up Minimum Viable Tracking

If the founder has no analytics, help them set up the basics before attempting a retention audit. You can't fix what you can't measure.

**Minimum viable retention metrics (set up this week):**

1. **DAU / WAU / MAU**: Daily, weekly, monthly active users. The ratio DAU/MAU tells you engagement intensity (messaging apps: 50%+, SaaS tools: 10-25%, consumer apps: 15-30%).

2. **Activation rate**: % of new sign-ups who complete the key action that correlates with retention. This is the single most important metric to define. Examples:
   - Slack: sent a message in a channel
   - Dropbox: uploaded a file
   - Notion: created a page
   Ask: "What's the ONE action that, when a user does it, means they 'get' your product?"

3. **Day 1 / Day 7 / Day 30 retention**: % of users who come back on day 1, day 7, day 30 after sign-up.
   - Day 1 retention under 30%: onboarding is broken
   - Day 7 retention under 15%: users don't find ongoing value
   - Day 30 retention under 5%: the product isn't sticky

4. **Churn rate**: % of users (or paying customers) who leave per month. For paid products: (customers lost in month / customers at start of month) x 100.

**Tool recommendation**: PostHog (free tier: 1M events/month, session recordings, feature flags). Set up event tracking for: sign-up, activation action, key product actions, and payment events.

After setting up tracking, wait 2-4 weeks to collect data before running the full audit. In the meantime, talk to users directly (see Step 3, "If no data" fallback).

**Research retention benchmarks (Web Search):**

Whether or not the founder has data, search for industry benchmarks to calibrate expectations:

- `"[product type] retention rate"` or `"[product type] churn rate benchmarks"` - find what's typical for this category
- `"SaaS churn benchmarks [year]"` or `"mobile app retention benchmarks [year]"` - get current industry data
- `"[competitor]" churn OR retention` - see if competitor retention data is available (sometimes in case studies or blog posts)

This context helps you assess whether the founder's retention is above or below par for their product type.

### Step 3: Diagnose Retention Across 4 Stages

If data exists (or the user can provide qualitative insights), diagnose retention at each stage:

**Stage 1: Onboarding Retention (Day 0-3)**

The question: Do new users reach the "aha moment"?

Check:
- What % of sign-ups complete the activation action? (If unknown, estimate from user feedback)
- How long does it take to reach the first value? (minutes, hours, days?)
- Where do users drop off in the onboarding flow?
- Is the onboarding too long, too confusing, or asking for too much before delivering value?

Red flags:
- Activation rate below 30% (most users never experience the product's value)
- Time-to-value over 10 minutes (too much setup before the first win)
- Multiple steps before the user sees any output (long form, account setup, integrations required)

Common fixes:
- Reduce steps to first value (can they see output in under 2 minutes?)
- Add sample data or templates so users don't start from a blank screen
- Remove unnecessary sign-up fields (name + email is enough to start)
- Show a progress indicator ("3 steps to your first [output]")

**Stage 2: Short-term Retention (Week 1-4)**

The question: Do activated users come back?

Check:
- Week 1 retention rate (% who return after first session)
- What brings them back? (habit, notification, need, external trigger)
- How often does the product expect users to return? (daily? weekly? monthly?)
- Is the expected frequency realistic for this type of product?

Red flags:
- Week 1 retention below 25% among activated users (even people who "got it" aren't returning)
- No trigger to return (the product waits passively for users to remember it)
- Usage is event-driven but rare (e.g., tax software - used once a year)

Common fixes:
- Add a trigger to return: email digest, push notification, weekly report
- Create a recurring use case (daily check-in, weekly review, ongoing tracking)
- Build a streak or progress mechanic if appropriate for the product type

**Stage 3: Medium-term Retention (Month 1-3)**

The question: Are users building the product into their workflow?

Check:
- Month 1 and month 3 retention rates
- Are users increasing their usage over time (more features, more data, more integrations)?
- Are they investing in the product? (customisation, data entry, integrations, team invites)
- What's the switching cost? (if they leave, how much do they lose?)

Red flags:
- Users plateau at basic usage and never go deeper
- No investment: users haven't customised, haven't entered data, haven't integrated
- Easy to switch: competitor could replace you with zero migration cost

Common fixes:
- Progressive feature disclosure (reveal advanced features as users grow)
- Increase investment: encourage data entry, customisation, integrations
- Build switching costs (export is easy, but they'd lose their setup, history, or integrations)

**Stage 4: Long-term Retention (Month 3+)**

The question: Why do long-term users eventually leave?

Check:
- What % of 3-month users are still active at 6 months? 12 months?
- Why do long-term users leave? Common reasons:
  - Feature gaps: they outgrew the product
  - Competitive switching: a better alternative appeared
  - Problem solved: they no longer need the product (e.g., job search tool after getting hired)
  - Life change: role change, company change, priority shift
- Are you losing your BEST users or your least engaged?

Red flags:
- Best users leave (they outgrew you - you have a ceiling problem)
- A competitor is consistently named in exit interviews
- The product solves a finite problem (once solved, no reason to stay)

Common fixes:
- Add depth for power users (advanced features, analytics, customisation)
- Monitor competitive landscape and respond to feature gaps
- If the problem is finite: build a recurring value layer on top (e.g., job search tool becomes career management tool)

### Step 4: Apply the Habit Loop

Use the Habit Loop model from Nir Eyal's "Hooked" (2014) to assess whether your product builds habits:

**1. Trigger**
What prompts the user to open your product?
- External triggers: push notification, email, calendar reminder, colleague's message
- Internal triggers: boredom, anxiety, curiosity, routine ("every morning I check...")
- Products that rely only on external triggers are fragile. Internal triggers create lasting habits.
- Ask: "When does your user FEEL the need to open your product? What emotion or situation triggers it?"

**2. Action**
What does the user do when they open the product?
- Is the action simple enough? (Fogg Behavior Model: Motivation + Ability + Trigger = Behavior)
- Can they complete the core action in under 30 seconds?
- Is there unnecessary friction? (loading time, navigation, decisions before action)

**3. Variable Reward**
Does the product deliver value that's slightly unpredictable or engaging?
- Three types of variable reward (Nir Eyal "Hooked"):
  - Rewards of the Tribe: social validation, likes, comments, recognition
  - Rewards of the Hunt: resources, information, deals (the "feed" effect)
  - Rewards of the Self: mastery, completion, achievement, competence
- Fixed rewards get boring. Variable rewards create anticipation.
- Ask: "Is there anything slightly unpredictable about what the user gets each time they open the product?"

**4. Investment**
Does the user put something into the product that makes leaving harder?
- Data: personal information, history, records
- Content: posts, documents, notes, projects
- Customisation: settings, preferences, workflows
- Social: connections, team setup, shared resources
- Reputation: karma, status, achievements
- The more a user invests, the higher the switching cost and the stronger the retention.

**Score the product on each dimension:**

| Dimension | Strength (1-5) | Current State | Improvement Opportunity |
|---|---|---|---|
| Trigger | [1-5] | [what exists] | [what could be added] |
| Action | [1-5] | [what exists] | [what could be simplified] |
| Variable Reward | [1-5] | [what exists] | [what could be added] |
| Investment | [1-5] | [what exists] | [what could be deepened] |

**Attribution**: The Habit Loop (Trigger -> Action -> Variable Reward -> Investment) is from Nir Eyal, "Hooked: How to Build Habit-Forming Products" (2014). The concept of variable reward draws on B.F. Skinner's research on variable-ratio reinforcement schedules. Activation metric concepts are widely used in growth engineering; Brian Balfour's work on retention curves provides additional context for understanding how retention shapes differ by product type.

### Step 5: Identify the #1 Retention Lever

Based on the stage-by-stage diagnosis and habit loop analysis, identify the ONE change that would have the biggest impact on retention.

The #1 lever should be:
- Specific: "Add a weekly email digest showing usage stats" not "improve engagement"
- Measurable: tied to a metric you can track (activation rate, Day 7 retention, etc.)
- High-impact: addresses the stage where the most users are lost
- Feasible: something a solo founder can implement in 1-2 weeks

Common #1 levers by stage:
- Onboarding gap -> reduce time-to-value (remove steps, add templates)
- Short-term gap -> add a return trigger (email, notification, recurring task)
- Medium-term gap -> increase investment (encourage data entry, customisation)
- Long-term gap -> add depth for power users (advanced features, integrations)

### Step 6: Create the Retention Improvement Plan

**Quick wins (this week):**
- [ ] [Action that takes under 4 hours and has immediate impact]
- [ ] [Action that takes under 4 hours]
- [ ] [Action that takes under 4 hours]

**Medium-term (this month):**
- [ ] [Action that requires 1-2 weeks of work]
- [ ] [Action that requires 1-2 weeks of work]

**Long-term (this quarter):**
- [ ] [Action that requires sustained effort over weeks]
- [ ] [Action that requires sustained effort over weeks]

### Output Format

```
## Retention Audit: [Product Name]

**Product**: [one-sentence description]
**Date**: [today]
**Current users**: [number]
**Data sources**: [what data was used for this audit]

### Retention by Stage

| Stage | Time Period | Retention Rate | Status | Key Issue |
|---|---|---|---|---|
| Onboarding | Day 0-3 | [%] or [unknown] | [Healthy/Warning/Critical] | [what's wrong] |
| Short-term | Week 1-4 | [%] or [unknown] | [Healthy/Warning/Critical] | [what's wrong] |
| Medium-term | Month 1-3 | [%] or [unknown] | [Healthy/Warning/Critical] | [what's wrong] |
| Long-term | Month 3+ | [%] or [unknown] | [Healthy/Warning/Critical] | [what's wrong] |

### Biggest Gap: [Stage]

**What's happening**: [description]
**Why**: [root cause]
**Impact**: [how many users this affects]

### Habit Loop Analysis

| Dimension | Score (1-5) | Current State | Opportunity |
|---|---|---|---|
| Trigger | [1-5] | [what exists] | [improvement] |
| Action | [1-5] | [what exists] | [improvement] |
| Variable Reward | [1-5] | [what exists] | [improvement] |
| Investment | [1-5] | [what exists] | [improvement] |

### #1 Retention Lever

**Change**: [specific action]
**Metric**: [what to measure]
**Expected impact**: [realistic improvement]
**Effort**: [hours/days to implement]

### Improvement Plan

**Quick wins (this week)**:
- [ ] [action]
- [ ] [action]

**Medium-term (this month)**:
- [ ] [action]
- [ ] [action]

**Long-term (this quarter)**:
- [ ] [action]
- [ ] [action]
```

Save as markdown.

## Common Mistakes

- **Focusing on acquisition when retention is broken.** Getting more users into a leaky bucket is waste. Fix the bucket first.
- **Using vanity metrics.** Total sign-ups means nothing if 90% never return. Track activated users and returning users.
- **Not defining the activation action.** If you can't name the ONE action that predicts retention, you can't measure or improve activation.
- **Treating all churn the same.** Someone who left after day 1 (never activated) needs a different fix than someone who left after month 3 (outgrew the product).
- **Adding features to fix retention.** Often the problem isn't missing features - it's that users never discovered the features you already have. Better onboarding beats more features.

## Notes

- If you have fewer than 50 users, quantitative retention data won't be statistically meaningful. Talk to users directly instead.
- Retention benchmarks vary wildly by product type. A daily-use app (messaging, social) needs much higher retention than a monthly-use tool (invoicing, tax prep).
- The best retention lever is almost always in onboarding. Most users who activate and get value in the first session will come back. Most who don't, won't.
- If the user hasn't defined a north star metric yet, run the north-star-metric skill first. The NSM tells you what "retained and engaged" looks like.

---

### Further Reading

- [Why Your Users Leave (And the One Metric That Tells You Why)](https://fantasticfounder.com) - Retention diagnosis for indie products using the Hooked model and activation metrics
