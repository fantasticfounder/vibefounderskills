---
name: channel-scorer
description: "Score and rank acquisition channels for YOUR specific product. Uses channel-market fit analysis to identify where your customers actually discover products - not where founders hang out. Triggers: which channels, best marketing channel, where to market, channel strategy, acquisition channels, marketing plan, where to find users."
---

# Score Your Acquisition Channels

Not all channels work for all products. This skill scores marketing channels against YOUR specific product, audience, and resources - so you stop wasting time on channels that feel productive but don't convert.

## Context

You are helping a founder evaluate acquisition channels for: **$ARGUMENTS**.

If the user provides details about their product, audience, competitors, or prior marketing attempts, read those first.

## Why Most Channel Advice Is Wrong

Generic advice says "launch on ProductHunt, post on Reddit, build on Twitter." But channels aren't universally good or bad - they're good or bad FOR YOUR PRODUCT.

The honest truth about popular channels:
- **ProductHunt**: Often founders upvoting founders. Great for visibility in the tech bubble, unreliable for sustained acquisition. Works best for developer tools and design products where the PH audience IS the customer. Poor for B2B, consumer, or niche products.
- **Reddit**: Powerful but fragile. Communities hate self-promotion. Works when you genuinely contribute value. Fails when you drop links and run.
- **Twitter/X**: Slow to build, high maintenance. Works for build-in-public founders with personality. Fails for products that need to reach non-tech audiences.
- **SEO**: Highest long-term ROI but slowest to start. Only works if people search for your product type (use validate-idea to check).
- **TikTok/Shorts**: Massive reach potential but unpredictable. Works for visual or "wow factor" products. Fails for complex B2B tools.
- **Cold outreach**: High effort, high conversion when done right. Works for high-value B2B products. Fails for low-price consumer tools.

## Instructions

Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Gather Context

You need to know:
- What the product does and who it's for (beachhead segment)
- Price point and business model
- Founder's resources: time per week for marketing, budget, existing audience/network
- Any prior channel experience (what's been tried, what happened)
- Which channels do you currently use regularly or feel confident posting on?
- Do you have any existing analytics data showing where your current users come from?

### Step 2: Evaluate Channels Against 6 Factors

Score each candidate channel on a 1-5 scale.

**Before scoring Audience Presence, verify it.** Use web search or ask the user: How many members does the subreddit have? Is the hashtag active? Do competitors post here? Do not guess - check.

| Factor | 1 (Poor) | 3 (Moderate) | 5 (Strong) |
|---|---|---|---|
| **Audience presence** | Target segment barely exists here | Some presence, mixed with others | Target segment is highly active here |
| **Discovery intent** | People socialise, don't discover products | Some product discovery happens | People actively look for tools/solutions here |
| **Content-format fit** | Product doesn't demo well in this format | Decent fit with effort | Natural fit - product shines in this format |
| **Competitive saturation** | Competitors dominate, hard to stand out | Some competition, room to differentiate | Low competition or untapped |
| **Effort-to-reach ratio** | High effort for few impressions | Moderate effort for moderate reach | Low effort for high reach |
| **Founder fit** | Founder hates this channel or lacks skills for it | Neutral - can learn | Founder has existing presence, skills, or network here |

**Founder fit matters.** A channel you'll never consistently use is worse than a "suboptimal" channel you'll show up to every day.

### Step 3: Score Each Channel

Evaluate these channels (skip any clearly irrelevant to the product):

**Organic / Community Channels:**
- Reddit (r/SideProject, r/SaaS, r/startups, niche subreddits)
- Twitter/X (build in public, threads, engagement)
- Hacker News (Show HN, comments)
- IndieHackers (posts, milestones, community)
- LinkedIn (for B2B products)
- Facebook Groups (for consumer/SMB products)
- Discord / Slack communities (niche product communities)
- Quora (answering questions related to the problem)

**Launch Platforms:**
- ProductHunt
- BetaList
- AlternativeTo
- G2 / Capterra (for SaaS)
- App stores (for mobile apps)

**Content / SEO:**
- SEO blog content (requires search demand)
- YouTube tutorials / demos
- TikTok / Instagram Reels
- Podcasts (guesting or own show)

**Outbound:**
- Cold email outreach
- LinkedIn DMs
- Partner / integration marketing
- Referral / word-of-mouth programs

### Step 4: Rank and Recommend

Rank channels by total score. Recommend a channel strategy:

- **Primary channel** (highest score): Spend 50% of marketing time here
- **Secondary channel** (second highest): Spend 30% of marketing time here
- **Experimental channel** (third highest): Spend 20% testing here
- **Avoid list**: Channels that scored below 15/30 - don't waste time. Below 15/30 means the channel fails on at least 3 of 6 factors - too many structural weaknesses to overcome with effort alone.

### Step 5: Output the Scorecard

```
## Channel Scorecard: [Product Name]

**Product**: [one-sentence description]
**Beachhead segment**: [who specifically]
**Price point**: [pricing model]
**Founder time for marketing**: [hours/week]
**Date**: [today]

### Channel Scores

| Channel | Audience (1-5) | Discovery (1-5) | Format Fit (1-5) | Competition (1-5) | Effort/Reach (1-5) | Founder Fit (1-5) | Total (/30) |
|---|---|---|---|---|---|---|---|
| [channel] | [score] | [score] | [score] | [score] | [score] | [score] | [total] |
| [channel] | [score] | [score] | [score] | [score] | [score] | [score] | [total] |
| ... | ... | ... | ... | ... | ... | ... | ... |

### Recommended Strategy

| Role | Channel | Score | Time Allocation | Why |
|---|---|---|---|---|
| **Primary** | [channel] | [/30] | 50% ([X] hrs/wk) | [specific reason for this product] |
| **Secondary** | [channel] | [/30] | 30% ([X] hrs/wk) | [specific reason] |
| **Experimental** | [channel] | [/30] | 20% ([X] hrs/wk) | [specific reason] |

### Channels to Avoid
| Channel | Score | Why Not |
|---|---|---|
| [channel] | [/30] | [specific reason - audience mismatch, too competitive, etc.] |

### Key Insight
[One paragraph: the most important strategic takeaway about where this product's customers actually discover solutions]
```

Save as markdown.

## Scoring Discipline

- Don't inflate scores for channels you personally like. Score based on evidence.
- "Audience presence" should be validated - check the subreddit, search the hashtag, look at competitor traffic sources.
- If you score every channel 3/5 on everything, you're not being honest. Force yourself to differentiate.
- ProductHunt scores high for "launch day buzz" but often low for "sustained acquisition." Be clear about which you need.
- A channel with a 28/30 score that the founder will never use is worse than a 20/30 channel they'll commit to daily.

## Notes

- Reassess channels every 4-8 weeks. What works at 0 users may not work at 500 users.
- The best channel mix is usually one slow-build channel (SEO, community) + one fast-feedback channel (Reddit, outreach) + one experimental channel.
- This skill pairs with first-users-plan (which builds the execution plan) and community-marketing (which goes deep on community channels).

---

### Further Reading

- [How to Market an App When You Have Zero Marketing Experience](https://fantasticfounder.com) - Honest channel-by-channel breakdown including which popular advice is wrong
