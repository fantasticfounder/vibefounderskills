---
name: growth-loops
description: "Design sustainable growth loops that compound over time - not one-off hacks. Evaluate loop types, score for fit, design mechanics, and build an implementation plan. Triggers: growth loops, flywheel, viral loop, how to grow, growth strategy, product led growth, PLG, growth mechanism."
---

# Design Your Growth Loops

You shipped a product and got some users. Now you need growth that doesn't depend on you posting on Reddit every day. Growth loops are self-reinforcing systems where the output of one cycle becomes the input of the next. One good loop is worth more than a hundred growth hacks.

## Context

You are helping a founder design growth loops for: **$ARGUMENTS**.

If the user provides details about their product, users, channels, or prior growth attempts, read those first. If a prior skill in this session produced a north star metric, retention diagnosis, or user data, use that context directly.

## Why This Matters

Most indie founders grow through manual effort: post on Reddit, launch on ProductHunt, send cold emails. These are linear actions - you do the work, you get some users, then it stops. Growth loops are different. They're systems where each new user creates the conditions for the next user. The best products grow because using the product IS the marketing.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Understand Current State

Ask the user (if not already clear from conversation context):
- How many users do you have right now?
- How did they find you? (list every channel and rough percentage)
- What do users actually DO in your product? (key actions, frequency)
- Is there any sharing or referral behaviour happening already? (even informal - "my friend told me about this")
- What's your current growth rate? (new users per week/month)
- Have you tried any growth tactics? What happened?

### Step 1b: Research How Similar Products Grow (Web Search)

Before evaluating loop types, search for how competitors and similar products acquire users. Real examples beat theory.

**Search for:**
- `"how [competitor] grew"` or `"[competitor] growth story"` - look for founder interviews, case studies
- `"[product type] growth strategy"` - see what channels and loops work in this space
- `"[product type] viral growth"` or `"[product type] word of mouth"` - check for existing viral/referral patterns
- Reddit: `site:reddit.com "[product type]" growth OR marketing` - find real founder conversations about what worked

**What to extract:**
- Which growth channels do successful competitors use? (product-led, content, paid, community)
- Are there natural sharing or referral patterns in this category?
- What K-factors or growth rates are realistic for this product type?
- Any examples of indie products that grew primarily through one loop?

Use this research to inform loop scoring in Step 3. A loop that works for similar products is more likely to work for you.

### Step 2: Evaluate 5 Growth Loop Types

For the user's specific product, evaluate each loop type:

**1. Viral Loop**
How it works: User creates something -> shares it on an external platform -> new user discovers the product through the shared output.
Examples: Loom (shared videos have Loom branding), Figma (shared design links), Calendly (every scheduling link is a product demo).
Best when: Your product's output is inherently shareable - documents, videos, images, links, reports that get seen by non-users.
Questions to assess fit: Does your product produce something users share externally? Would non-users see the output? Would seeing it make them want the product?

**2. Content Loop**
How it works: User creates content inside the product -> content ranks in search or gets discovered externally -> attracts new users.
Examples: Notion (public templates rank in Google), Canva (designs shared on social), Stack Overflow (answers rank for developer questions).
Best when: User-generated content has standalone value outside your product and can be indexed or discovered.
Questions to assess fit: Do users create content that has value to people who aren't using your product? Could that content rank in search or spread on social?

**3. Collaboration Loop**
How it works: User invites a colleague or collaborator -> collaborator discovers value through using the product together -> collaborator invites more people.
Examples: Slack (team invites), Google Docs (sharing for editing), Linear (team project management).
Best when: The product is better with more people and has natural collaboration triggers.
Questions to assess fit: Is your product more valuable when used with others? Does using it naturally require inviting someone else?

**4. Referral Loop**
How it works: User refers a friend -> friend signs up -> referrer gets a reward -> motivated to refer again.
Examples: Dropbox (both get extra storage), Uber (both get ride credits), Morning Brew (tiered rewards).
Best when: You can offer an incentive that doesn't erode margins and the product solves a problem people talk about.
Questions to assess fit: Can you offer something valuable as a reward without losing money? Do users talk about this type of product with peers?

**5. Paid Loop**
How it works: Revenue from users -> reinvest in ads or paid content -> acquire new users -> generate more revenue.
Examples: Many SaaS products, Masterclass (YouTube ads funded by subscriptions), subscription boxes.
Best when: Unit economics support it - your lifetime value (LTV) is at least 3x your customer acquisition cost (CAC).
Questions to assess fit: Do you know your LTV? Can you profitably acquire users through paid channels? Do you have enough margin to reinvest?

### Step 3: Score Each Loop

For each of the 5 loop types, score on a 1-5 scale:

| Loop Type | Product Fit | Implementation Effort | Compound Potential | Founder Resources | Total |
|---|---|---|---|---|---|
| Viral | [1-5] | [1-5, inverted: 5=easy] | [1-5] | [1-5, inverted: 5=low effort] | [/20] |
| Content | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Collaboration | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Referral | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Paid | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |

**Scoring guide:**
- **Product fit (1-5):** How naturally does this loop type align with what your product does? 5 = the loop is a natural extension of product usage. 1 = you'd have to bolt it on artificially.
- **Implementation effort (1-5, inverted):** How much engineering and design work? 5 = minimal changes needed. 1 = months of development.
- **Compound potential (1-5):** How strongly does this loop compound? 5 = each cycle amplifies the next. 1 = linear growth, each cycle independent.
- **Founder resources (1-5, inverted):** How much ongoing founder time? 5 = runs itself once built. 1 = requires constant founder attention.

Score honestly. If there's no evidence that users share your product output, viral loop product fit is a 1 or 2, not a 3. Document your reasoning for any score of 4-5 or 1-2. When scores tie, apply the tiebreaker rules from CONVENTIONS.md: prioritise loops the founder can validate with evidence over loops based on inference.

### Step 4: Design the Primary Loop

Take the highest-scoring loop and design the full mechanics:

**Trigger**: What initiates the loop? This could be:
- A user action (creating a report, completing a task, hitting a milestone)
- A time-based event (weekly summary, end of month)
- A feature-based prompt (after using a specific feature)

**Incentive**: Why would the user participate? Two types:
- Intrinsic: the product is genuinely better when shared (collaboration tools, multiplayer features)
- Extrinsic: there's a tangible reward (free months, credits, status, unlocked features)

**Friction points**: What could stop the loop from working?
- Privacy concerns (users don't want to share their data)
- Effort to share (too many steps between action and sharing)
- Poor onboarding for new users arriving via the loop (referred user lands on confusing page)
- Wrong audience (the people who see shared content aren't potential users)

**Measurement**: How do you know the loop is working?
- **Viral coefficient (K-factor)**: K = number of invites sent per user x conversion rate of those invites. K > 1 means exponential growth. K = 0.5 means each user brings half a new user (still valuable).
- **Loop time**: How long from one user entering to the next user entering? Shorter = faster compounding. Days are better than weeks.
- **Conversion at each step**: Map the full funnel. Example: 100 users -> 30 share something -> 150 people see it -> 15 click -> 5 sign up. K = 5/100 = 0.05. That's low - find which step leaks the most.

**Attribution**: The growth loops framework draws from Ognjen Boskovic's work on loop-based growth models and the broader product-led growth movement. Viral coefficient (K = invites x conversion rate) is a standard growth metric. The AARRR pirate metrics framework (Acquisition, Activation, Retention, Referral, Revenue) was created by Dave McClure (2007) and provides the broader context for where growth loops fit in the user lifecycle.

### Step 5: Build the 30-60-90 Day Implementation Plan

**Days 1-30: Foundation**
- Instrument the loop. Set up tracking for every step (trigger -> action -> share -> new user -> activation).
- Build the minimum viable version of the loop mechanism (share button, referral link, content publishing, collaboration invite).
- Test with existing users. Don't launch publicly - ask 10-20 engaged users to try the loop.
- Measure the baseline K-factor and loop time.
- Fix the biggest friction point identified in testing.

**Days 31-60: Optimise**
- A/B test the trigger: when do you prompt users? What copy works?
- Improve the new user experience for loop-acquired users. They have different context than organic sign-ups.
- Increase the incentive if K-factor is below target.
- Reduce friction at the step with the biggest drop-off.
- Set a weekly review cadence: check loop metrics every Monday.

**Days 61-90: Scale**
- If K > 0.3: the loop is working. Invest more in the trigger and the new user landing experience.
- If K < 0.1: the loop isn't natural for your product. Consider switching to your second-highest scoring loop.
- Begin designing the secondary loop to layer on top.
- Document what works as a playbook for future products.

### Step 6: Identify the Secondary Loop

Pick the second-highest scoring loop from Step 3. This is your next growth investment after the primary loop is running.

Explain:
- Why this loop complements the primary one (different acquisition channel, different user behaviour)
- When to start building it (what primary loop metrics should trigger the switch)
- How the two loops can reinforce each other

### Output Format

```
## Growth Loops Analysis: [Product Name]

**Product**: [one-sentence description]
**Date**: [today]
**Current users**: [number]
**Current growth**: [rate and channels]

### Loop Scoring

| Loop Type | Product Fit | Effort (inv) | Compound | Resources (inv) | Total | Notes |
|---|---|---|---|---|---|---|
| Viral | [1-5] | [1-5] | [1-5] | [1-5] | [/20] | [key reason] |
| Content | [1-5] | [1-5] | [1-5] | [1-5] | [/20] | [key reason] |
| Collaboration | [1-5] | [1-5] | [1-5] | [1-5] | [/20] | [key reason] |
| Referral | [1-5] | [1-5] | [1-5] | [1-5] | [/20] | [key reason] |
| Paid | [1-5] | [1-5] | [1-5] | [1-5] | [/20] | [key reason] |

### Recommended Primary Loop: [Type]

**Why this loop**: [2-3 sentences]

**Mechanics**:
- Trigger: [what starts it]
- Incentive: [why users participate]
- Friction points: [what could block it + mitigation]
- K-factor target: [realistic number]
- Loop time target: [days/weeks]

### 30-60-90 Day Plan

**Days 1-30 (Foundation)**:
- [ ] [specific action]
- [ ] [specific action]
- [ ] [specific action]

**Days 31-60 (Optimise)**:
- [ ] [specific action]
- [ ] [specific action]
- [ ] [specific action]

**Days 61-90 (Scale)**:
- [ ] [specific action]
- [ ] [specific action]
- [ ] [specific action]

### Secondary Loop: [Type]

**When to start**: [trigger condition]
**How it complements the primary loop**: [explanation]
```

Save as markdown.

## Common Mistakes

- **Building a referral program when nobody refers your product naturally.** If users aren't already telling friends about you, adding a referral reward won't fix it. The product needs to be worth talking about first.
- **Copying a growth loop from a product in a different category.** Dropbox's referral loop worked because storage has a clear, tangible value. Your SaaS might not have an equivalent.
- **Optimising a loop before validating it works at all.** Don't A/B test the share button colour when you don't know if anyone will click it.
- **Ignoring loop time.** A loop that takes 3 months per cycle will never compound meaningfully for an indie product. Prioritise loops with shorter cycle times.
- **Not measuring each step.** "We have a share button" is not a loop. You need numbers at every step: how many share, how many see, how many click, how many sign up, how many activate.

## Notes

- Growth loops work best when retention is solid. If users churn after a week, acquiring more users through loops just fills a leaky bucket. Run the retention-audit skill first if you haven't.
- K-factor below 1 is fine. K = 0.5 means each user brings half a new user, which combined with other channels creates strong overall growth.
- For most indie products, the content loop and referral loop are the most realistic starting points. Viral and collaboration loops usually require specific product architecture.

---

### Further Reading

- [Growth Loops for Indie Products: Beyond "Just Post on Reddit"](https://fantasticfounder.com) - Sustainable growth mechanisms for products built by solo founders
