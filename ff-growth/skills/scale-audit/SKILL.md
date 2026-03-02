---
name: scale-audit
description: "Assess whether your one-person business can scale - and what needs to change if it can't. Time allocation breakdown, bottleneck analysis, leverage opportunities, unit economics, and scaling roadmap. Triggers: scale, scaling, can this scale, one person business, solopreneur scale, grow beyond myself, bottleneck, scaling audit."
---

# Run a Scale Audit

You've got users, maybe revenue, and you're working 50+ hours a week. Something has to give. This skill helps you figure out what's actually bottlenecking your growth, what to automate, what to delegate, and whether scaling up is even the right goal for you.

## Context

You are helping a founder assess scaling readiness for: **$ARGUMENTS**.

If the user provides details about their product, revenue, time allocation, or team (even if "team" means just them), read those first. If a prior skill in this session produced retention data, growth loop design, or north star metrics, use that context.

## Why This Matters

Most solo founders hit a ceiling. They're doing everything - building features, answering support tickets, writing blog posts, managing billing, fixing bugs. Growth stalls not because the product is bad, but because the founder's time is the bottleneck. This audit identifies what breaks at scale and what to do about it.

But here's the thing: not every business needs to scale. A profitable $5K/month business that takes 20 hours/week is a perfectly valid outcome. This audit surfaces the CHOICE, not the assumption.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Current State Assessment

Ask the user (if not already clear):
- What's your current monthly revenue? (MRR for subscriptions, total for one-time)
- What are your monthly costs? (hosting, tools, services, any contractors)
- How many customers/users do you have?
- How many hours per week do you spend on the business?
- What does a typical week look like? Walk me through what you do.
- Do you have anyone helping? (co-founder, contractor, VA, anyone)
- What's your current growth rate? (new users/customers per month)
- What's your goal? Do you want to grow this as big as possible, or do you have a target income/lifestyle in mind?

That last question matters. The entire audit changes based on the answer.

### Step 2: Map Time Allocation

Help the founder map where their time actually goes. Most people are wrong about this until they write it down.

Break activities into 4 categories:

**Build (product development, features, bug fixes, technical infrastructure)**
- What: coding, designing, deploying, testing, technical research
- Healthy range: 40-60% early stage, decreasing to 20-30% as the product matures
- Watch for: spending 80%+ on building while neglecting everything else

**Sell (marketing, sales, outreach, content creation, community engagement)**
- What: writing blog posts, social media, cold outreach, SEO, partnerships, demo calls
- Healthy range: 20-30%
- Watch for: spending 0% here (common for technical founders who just want to build)

**Support (customer support, onboarding help, bug reports, documentation)**
- What: answering emails, chat support, writing help docs, handling refunds
- Healthy range: 10-20%
- Watch for: support eating 30%+ of time (this is the most common scaling bottleneck)

**Operate (admin, billing, infrastructure management, legal, accounting)**
- What: invoices, taxes, domain renewals, server management, compliance, analytics setup
- Healthy range: under 10%
- Watch for: operational overhead creeping up as the business grows

**Map it:**

| Category | Hours/Week | % of Total | Activities |
|---|---|---|---|
| Build | [hours] | [%] | [list main activities] |
| Sell | [hours] | [%] | [list main activities] |
| Support | [hours] | [%] | [list main activities] |
| Operate | [hours] | [%] | [list main activities] |
| **Total** | [hours] | 100% | |

Compare to the healthy ranges. Flag any category that's significantly over or under.

### Step 3: Apply the Leverage Test

For each major activity within each category, ask four questions:

**1. Can it be automated?**
- Code: scripts, cron jobs, CI/CD pipelines
- No-code: Zapier, Make, IFTTT
- AI: ChatGPT for drafting, AI support bots, automated responses
- Examples: billing reminders (automate), onboarding emails (automate), server monitoring (automate)

**2. Can it be eliminated?**
- Does anyone actually need this? Did a user request it, or did you assume?
- The most leveraged thing you can do is stop doing something nobody needs
- Examples: features nobody uses (eliminate), manual reports nobody reads (eliminate)

**3. Can it be delegated?**
- VA (virtual assistant): $5-15/hour for support, scheduling, data entry
- Freelancer: $30-100/hour for design, copywriting, specialised development
- Contractor: ongoing relationship for consistent work
- Examples: customer support responses (delegate to VA with templates), design work (delegate to freelancer)

**Research delegation and automation options (Web Search):**

Search for practical tools and services relevant to the founder's bottleneck activities:

- `"[task] automation tool"` or `"automate [activity] SaaS"` - find automation options for their specific bottlenecks
- `"virtual assistant for [task type]"` - find VA services and typical pricing
- `"[product type] support automation"` or `"[product type] self-service"` - see how competitors handle support at scale
- `"solopreneur tools [year]"` - find curated lists of tools for solo founders

Use specific findings to populate the leverage matrix with real tool names, pricing, and time savings estimates.

**4. Does it scale linearly or sub-linearly?**
- Linear: 1 customer = 1 hour of support. 100 customers = 100 hours. This BREAKS at scale.
- Sub-linear: 1 blog post serves 1,000 readers. Writing scales sub-linearly.
- Super-linear: a community moderates itself as it grows. Network effects.
- Every linear activity is a ticking time bomb. Identify them and plan to automate or delegate.

**Create the leverage matrix:**

| Activity | Category | Hours/Week | Automate? | Eliminate? | Delegate? | Scales? |
|---|---|---|---|---|---|---|
| [activity] | Build/Sell/Support/Operate | [hours] | [Y/N + how] | [Y/N + why] | [Y/N + to whom] | [Linear/Sub/Super] |
| [activity] | | [hours] | | | | |
| [activity] | | [hours] | | | | |

The activities that are: high hours + linear scaling + can be automated or delegated = highest priority for action.

### Step 4: Unit Economics at Scale

Current economics:
- Revenue per customer per month: MRR / number of customers
- Cost per customer per month: (total costs + founder time valued at market rate) / number of customers
- Margin per customer: revenue - cost
- Founder time per customer per month: total hours / number of customers

**At 10x current customers:**

| Metric | Current | At 10x | Notes |
|---|---|---|---|
| Customers | [N] | [10N] | |
| Revenue | [$] | [$] | Linear with customers (usually) |
| Hosting/infrastructure | [$] | [$] | Usually sub-linear (bulk pricing) |
| Support hours | [hours] | [hours] | Linear unless automated |
| Founder hours needed | [hours] | [hours] | What's realistic? |
| Margin per customer | [$] | [$] | Improves or degrades? |

**What breaks at 10x?**
- Support: If you spend 10 hours/week on support for 100 customers, 1,000 customers means 100 hours/week. That's impossible solo.
- Infrastructure: Does your tech stack handle 10x traffic/data without a rewrite?
- Quality: Can you maintain product quality with 10x users and 10x feature requests?
- Time: At 10x, the total hours exceed what one person can do. Where's the breaking point?

**At 100x current customers:**
- Is this still a one-person business? (Almost certainly not)
- What does the team look like? (support person, developer, marketer?)
- What's the monthly burn rate?
- Is the margin strong enough to support a small team?

These projections are estimates. The point isn't precision - it's identifying which constraints hit first.

### Step 5: Build the Scaling Roadmap

Based on the leverage test and unit economics, create a staged plan:

**Stage 1: Automate First (do this now, regardless of revenue)**
Automation costs almost nothing and saves time permanently.
- [ ] Automate [activity] using [tool/method] - saves [X] hours/week
- [ ] Automate [activity] using [tool/method] - saves [X] hours/week
- [ ] Automate [activity] using [tool/method] - saves [X] hours/week
- Estimated time saved: [X] hours/week

**Stage 2: Eliminate Next (do this now)**
Cut things that don't matter.
- [ ] Stop doing [activity] because [reason]
- [ ] Stop doing [activity] because [reason]
- Estimated time saved: [X] hours/week

**Stage 3: Delegate When Revenue Justifies It**
Set a revenue milestone for each hire/contractor:
- At $[X] MRR: hire a [role] for [hours/week] at $[Y]/month. This frees up [Z] hours/week.
- At $[X] MRR: hire a [role] for [hours/week] at $[Y]/month.
- Rule of thumb: the hire should cost less than 30% of the revenue they enable you to earn or save.

**Stage 4: Restructure If Needed**
Some businesses need architectural changes to scale:
- Self-serve onboarding (replaces manual onboarding calls)
- Knowledge base / FAQ (replaces repetitive support answers)
- API / integrations (replaces manual data transfers)
- Community forum (users help each other, reducing support load)

### Step 6: The Lifestyle Business Option

Not everything needs to scale. Surface this explicitly.

**Calculate the "comfortable solo" scenario:**
- At what number of customers are you earning enough and not overwhelmed?
- What MRR gives you the lifestyle you want?
- How many hours per week do you want to work?

If the answer is "I'm happy at $5K/month working 25 hours/week," that's a valid scaling strategy: MAINTAIN. Cap growth, optimise for efficiency and quality of life, and invest time in other things.

**The lifestyle path:**
- Set a customer cap or waitlist if support becomes too much
- Raise prices to increase revenue per customer instead of customer count
- Automate everything possible to reduce hours
- Focus on retention over acquisition (keep the customers you have happy)
- Build recurring revenue so income is predictable

**The growth path:**
- Follow the scaling roadmap from Stage 1-4
- Accept that you'll need to hire eventually
- Invest in systems and processes that work without you
- Think about the business as a system, not as your personal project

Present both options honestly. The founder should make an informed choice, not a default one.

**Attribution**: Bottleneck theory draws from Eliyahu Goldratt's "The Goal" (1984), where the principle of identifying and resolving system constraints was established. The leverage concept (automate, eliminate, delegate) is a practical application of systems thinking. Unit economics analysis is a foundational business strategy tool.

### Output Format

```
## Scale Audit: [Product Name]

**Product**: [one-sentence description]
**Date**: [today]
**Current MRR**: [$]
**Current customers**: [number]
**Founder hours/week**: [number]

### Time Allocation

| Category | Hours/Week | % | Healthy Range | Status |
|---|---|---|---|---|
| Build | [hours] | [%] | 40-60% | [OK/Over/Under] |
| Sell | [hours] | [%] | 20-30% | [OK/Over/Under] |
| Support | [hours] | [%] | 10-20% | [OK/Over/Under] |
| Operate | [hours] | [%] | <10% | [OK/Over/Under] |

### Bottleneck: [Category/Activity]

**What's eating your time**: [description]
**Why it matters**: [impact on growth]
**Scaling risk**: [what happens at 10x]

### Leverage Matrix (Top Priorities)

| Activity | Hours | Action | Tool/Method | Time Saved |
|---|---|---|---|---|
| [activity] | [hours] | Automate | [how] | [hours/week] |
| [activity] | [hours] | Eliminate | [why] | [hours/week] |
| [activity] | [hours] | Delegate | [to whom] | [hours/week] |

### Unit Economics

| Metric | Current | At 10x | At 100x |
|---|---|---|---|
| Revenue/customer | [$] | [$] | [$] |
| Cost/customer | [$] | [$] | [$] |
| Margin/customer | [$] | [$] | [$] |
| Founder hours/customer | [hours] | [hours] | [hours] |

**What breaks first at 10x**: [specific constraint]

### Scaling Roadmap

**Now: Automate**
- [ ] [action + tool + time saved]

**Now: Eliminate**
- [ ] [action + reason]

**At $[X] MRR: First hire**
- Role: [what]
- Cost: [$]/month
- Frees up: [hours/week]

### Lifestyle vs Growth

**Comfortable solo scenario**: [MRR, hours/week, customer count]
**Growth scenario**: [target MRR, team needed, timeline]
**Founder's stated preference**: [what they said]
**Recommendation**: [honest assessment based on the data]
```

Save as markdown.

## Common Mistakes

- **Hiring too early.** Don't hire at $2K MRR just because you're busy. Automate and eliminate first. Most solo founders can handle much more than they think with the right systems.
- **Hiring too late.** Don't wait until you're burned out and dropping balls. Plan ahead - know your revenue milestone for the first hire and start looking before you hit it.
- **Scaling what shouldn't scale.** If support takes 50% of your time, the fix might not be "hire a support person." It might be "fix the product so users don't need support."
- **Assuming growth is always the goal.** Some of the happiest founders run small businesses that stay small. The audit should surface the choice, not assume the answer.
- **Valuing your time at $0.** When calculating unit economics, include your time at a market rate. If you're spending 2 hours per customer per month, that's real cost even if you're not paying yourself yet.

## Notes

- This audit works best with at least 3 months of operating data. Earlier than that, the patterns aren't clear.
- Revenue milestones for hiring vary by region, role, and business type. The $X MRR suggestions in the roadmap should be calculated based on the specific founder's costs and goals.
- The leverage test should be re-run every quarter. As the business changes, so do the bottlenecks.
- If you haven't defined your north star metric or designed growth loops yet, run those skills first. Scaling without knowing what to optimise for is just growing chaos.

---

### Further Reading

- [How to Scale a One-Person Business (Or Why You Might Not Want To)](https://fantasticfounder.com) - Scaling assessment for solo founders who want to grow without burning out
