---
name: referral-system
description: "Build a referral system that actually generates new users. Covers referral types, two-sided incentive design, mechanics, tracking, and realistic targets for indie products. Triggers: referral system, referral program, word of mouth, how to get referrals, referral loop, ambassador program, refer a friend."
---

# Build Your Referral System

Word of mouth is the most trusted acquisition channel. But "hoping users tell their friends" isn't a strategy. A referral system turns informal recommendations into a repeatable, measurable engine. This skill helps you design one that fits your product, your audience, and your resources.

## Context

You are helping a founder build a referral system for: **$ARGUMENTS**.

If the user provides details about their product, user base, or current referral behaviour, read those first. If a prior skill in this session produced growth loop analysis, use that context directly.

## Why This Matters

Most indie products grow through word of mouth whether or not the founder designs for it. The question isn't "should people refer my product?" - it's "am I making it easy, rewarding, and trackable?" A well-designed referral system typically generates 5-15% of new signups for indie products. That's free, high-quality users who already trust you because a friend sent them.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Determine If Referrals Make Sense

Not every product is a good fit for a formal referral system. Assess these three conditions:

**1. Natural conversation fit**: Does your product naturally come up in conversation?
- High fit: "I've been using this app to track my workouts and it's changed my routine" (lifestyle, productivity, health)
- Medium fit: "We switched our invoicing tool and it's way faster" (B2B tools, niche software)
- Low fit: "I use this database migration tool" (deeply technical, embarrassing, or invisible products)

**2. Informal referral signals**: Are users already recommending you without being asked?
- Check: support tickets mentioning "my friend told me about this", app store reviews saying "recommended by a colleague", sign-up source data showing referral traffic
- If yes: you have organic referral energy to amplify
- If no: you need to create the conditions first (make the product worth talking about)

**3. Audience connectivity**: Are your target users connected to each other?
- High: freelancers in the same Slack communities, developers on the same Twitter circles
- Medium: small business owners in the same industry
- Low: consumers with no shared identity or community

If all three are low, a referral system is unlikely to work. Focus on other growth channels first (content, paid, community). If at least two are medium or high, proceed.

**Research referral patterns in this space (Web Search):**

Before designing the system, search for how competitors and similar products handle referrals:

- `"[product type] referral program"` or `"[competitor] referral"` - see if formal programs exist
- `"[product type] word of mouth"` or `"how did [competitor] get first users"` - look for organic referral patterns
- Reddit: `site:reddit.com "[product type]" referral OR "told my friend"` - find real user referral behaviour
- `"[product type] ambassador program"` - check for community-based referral models

Use what you find to inform the referral type selection in Step 2 and the incentive design in Step 3.

### Step 2: Choose the Referral Type

**Product-led referral**: Sharing is built into the product itself.
- How it works: Using the product naturally exposes it to non-users. Invite to collaborate, share output with branding, embed links.
- Best for: Collaboration tools, content creation tools, scheduling tools.
- Examples: Figma (shared design links), Calendly (every meeting link is a product demo), Notion (shared workspaces).
- Implementation: Medium - requires product changes.
- Founder effort: Low once built - runs automatically.

**Incentivized referral**: Give-get model where both parties receive something.
- How it works: User gets a unique referral link. When someone signs up through it, both the referrer and the new user get a reward.
- Best for: Products with clear value units (storage, credits, subscription time).
- Examples: Dropbox (both get 500MB), Uber (both get ride credit), Wise (both get fee-free transfer).
- Implementation: Medium - need referral tracking and reward fulfillment.
- Founder effort: Medium - need to monitor fraud and manage rewards.

**Status-based referral**: Recognition and status drive referrals.
- How it works: Top referrers get badges, leaderboard positions, "founding member" status, early access to features.
- Best for: Community-oriented products, products with engaged power users.
- Examples: Morning Brew (tiered rewards including merchandise), Product Hunt (maker badges), many Discord communities.
- Implementation: Low-medium - leaderboard and badge system.
- Founder effort: Low - self-managing once the status system is in place.

**Community-based referral**: Structured ambassador or power user program.
- How it works: Select engaged users as ambassadors. Give them exclusive access, direct communication with the founder, and tools to spread the word.
- Best for: Products with passionate early adopters, niche communities.
- Examples: Notion ambassadors, Figma community advocates, early Superhuman users.
- Implementation: Low - mostly relationship-building.
- Founder effort: High - requires personal relationship management.

### Step 3: Design the Incentive Structure

The incentive must pass three tests:

**1. Value test**: Is the reward valuable enough to motivate action?
- Bad: "Get a badge on your profile" (unless your community highly values status)
- Good: "Get one month free" (clear, tangible, valuable)
- Great: "You and your friend both get one month free" (two-sided, feels fair)

**2. Economics test**: Can you afford it?
- Calculate: If 10% of users refer and each referral costs you $X in rewards, does the math work?
- Rule of thumb: referral reward should be less than 30% of first-year LTV
- Free/freemium products: the reward is product value (storage, features, time) not cash

**3. Alignment test**: Does the incentive attract the RIGHT users?
- Cash incentives for consumer products attract deal-seekers who churn fast. Avoid.
- Product-value incentives (free months, extra features, storage) attract users who actually want the product.
- Two-sided incentives (both referrer and referred get something) outperform one-sided by 2-3x.

**Design the two-sided incentive:**
- Referrer gets: [free months / credits / premium features / storage / recognition]
- Referred user gets: [extended trial / discount on first payment / bonus features / credits]
- Make the referred user's reward immediate (they feel the value on day one)
- Make the referrer's reward trigger on the referred user's activation (not just sign-up) to reduce fraud

### Step 4: Design the Mechanics

**How does the user share?**
- Unique referral link (simplest - generate per user, works everywhere)
- In-app invite button (email, SMS, or messaging app)
- Share on social with pre-filled message (Twitter, LinkedIn)
- Referral code (manual but trackable)

**When do you ask?**
Timing matters more than the incentive. Ask at the moment of highest satisfaction:
- After the user's first success (completed a task, got a result, hit a milestone)
- After receiving positive feedback or a compliment on something made with your product
- NOT on signup (they haven't experienced value yet)
- NOT when they're frustrated (after a bug, during a support ticket)

**Where does it live in the product?**
- Dedicated referral page (linked from settings or profile)
- Contextual prompts at success moments
- Share buttons on shareable outputs
- Email follow-up after key milestones

**How do you track?**
- Unique referral codes or links per user
- UTM parameters for attribution
- Referral dashboard showing: shares sent, clicks, sign-ups, activations, rewards earned
- Tools: Rewardful (SaaS-focused, Stripe integration), ReferralCandy (e-commerce), custom build with unique codes + webhook tracking

### Step 5: Set Realistic Targets

Referral benchmarks for indie products (not enterprise or VC-backed):

| Metric | Low | Average | Strong |
|---|---|---|---|
| % of users who share their referral link | 2-5% | 5-10% | 10-20% |
| Conversion rate on referral clicks | 10-15% | 15-25% | 25-40% |
| % of new signups from referrals | 3-5% | 5-10% | 10-20% |
| Referral K-factor contribution | 0.03-0.05 | 0.05-0.15 | 0.15-0.30 |

These numbers assume: a product people genuinely like, a clear incentive, and a referral system that's been live for at least 4-6 weeks. Week 1 numbers will be much lower as users discover the system.

**Set your targets based on current state:**
- If users already refer informally: aim for "Average" or "Strong" within 3 months
- If no referral behaviour exists: aim for "Low" in month 1, "Average" by month 3
- If you're unsure: start with "Low" targets and increase as you learn

### Step 6: Implementation Plan

**Week 1-2: Build the minimum viable referral system**
- [ ] Generate unique referral links per user
- [ ] Build the referral landing page (where referred users arrive)
- [ ] Set up tracking (link clicks, sign-ups from referral, activations)
- [ ] Design the reward fulfillment (manual is fine to start)
- [ ] Create the in-app referral prompt (placed at a success moment)

**Week 3-4: Launch to existing users**
- [ ] Email existing users announcing the referral program
- [ ] Add the referral prompt to the product at the right moment
- [ ] Monitor: are people sharing? Are referred users signing up?
- [ ] Respond personally to every referrer (builds goodwill and feedback)

**Month 2: Optimise**
- [ ] Analyse the funnel: where do referrals drop off?
- [ ] Test different incentives if share rate is low
- [ ] Test different timing if click-through is low
- [ ] Improve the referred user's landing experience if conversion is low

**Month 3: Scale or pivot**
- [ ] If referrals generate 5%+ of new signups: invest more (better incentives, more prompts, referral dashboard for users)
- [ ] If referrals generate under 2%: the product might not be a natural fit for referrals. Redirect effort to content or community growth.

**Tool recommendations for solo founders:**
- **Rewardful**: Best for SaaS with Stripe billing. Handles tracking, rewards, and payouts. Free plan available.
- **ReferralCandy**: Best for e-commerce. Automated reward fulfillment.
- **Custom build**: Unique codes + webhook tracking + manual reward. Best when you want full control and have few users. Good enough to start.
- **Viral Loops**: Template-based referral campaigns. Good for quick launch.

### Output Format

```
## Referral System Design: [Product Name]

**Product**: [one-sentence description]
**Date**: [today]
**Current users**: [number]
**Current referral behaviour**: [organic referrals happening? Y/N + details]

### Referral Fit Assessment

| Factor | Rating | Evidence |
|---|---|---|
| Natural conversation fit | [Low/Medium/High] | [why] |
| Informal referral signals | [Low/Medium/High] | [why] |
| Audience connectivity | [Low/Medium/High] | [why] |

**Verdict**: [Proceed / Proceed with caution / Not recommended]

### Referral Type: [Product-led / Incentivized / Status / Community]

**Why this type**: [2-3 sentences]

### Incentive Structure

- **Referrer gets**: [reward]
- **Referred user gets**: [reward]
- **Trigger**: [when reward is granted - on sign-up or activation?]
- **Economics**: [cost per referral vs LTV]

### Mechanics

- **Sharing method**: [link / invite / social / code]
- **Timing**: [when to prompt]
- **Placement**: [where in the product]
- **Tracking**: [tool or method]

### Targets (3-month)

| Metric | Month 1 | Month 2 | Month 3 |
|---|---|---|---|
| Share rate | [%] | [%] | [%] |
| Referral conversion | [%] | [%] | [%] |
| % new users from referrals | [%] | [%] | [%] |

### Implementation Timeline

[Week-by-week plan]
```

Save as markdown.

## Common Mistakes

- **Launching a referral program before the product is worth referring.** If retention is bad, referrals just bring more people into a leaky bucket. Fix retention first.
- **Rewarding sign-ups instead of activations.** People will game the system with throwaway accounts. Reward when the referred user actually does something valuable.
- **One-sided incentives.** Giving the referrer a reward but nothing to the referred user feels exploitative. Two-sided always outperforms.
- **Hiding the referral system.** If it's buried in settings, nobody will find it. Surface it at success moments.
- **Cash rewards for consumer products.** This attracts deal-hunters who churn immediately. Offer product value instead.

## Notes

- The best referral systems feel like a natural part of the product, not a bolted-on marketing gimmick.
- Start manually. For your first 50 referrals, handle rewards by hand. You'll learn more from the process than from automating it.
- Word of mouth happens whether you design for it or not. A referral system doesn't CREATE word of mouth - it AMPLIFIES and TRACKS it.
- If you haven't designed growth loops yet, run the growth-loops skill first. Referrals are one type of loop.

---

### Further Reading

- [How to Get Referrals: Building Word-of-Mouth Into Your Product](https://fantasticfounder.com) - Referral system design for indie products that don't have a marketing budget
