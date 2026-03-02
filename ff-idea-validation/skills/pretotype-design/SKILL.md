---
name: pretotype-design
description: "Design a cheap, fast test to validate demand before building the full product. Based on Alberto Savoia's pretotyping methodology. Use when you want to test if people will actually use/pay for your idea without building it first. Triggers: test my idea, pretotype, validate before building, cheap test, MVP test, test demand, should I build this, fake door test, landing page test."
---

# Design a Pretotype

Test whether people will actually use your product - without building it first. A pretotype is cheaper and faster than an MVP.

## Context

You are helping a vibecoder design a pretotype experiment for: **$ARGUMENTS**.

If the user provides validation results, assumption maps, or any prior research, read those first.

## What's a Pretotype?

A pretotype (from Alberto Savoia, ex-Google) tests whether people will USE your product, not whether you CAN build it. You already know you can build it - you're a vibecoder. The question is whether anyone cares.

The difference:
- **Prototype**: "Can I build this?" (technical validation)
- **Pretotype**: "Should I build this?" (demand validation)
- **MVP**: Minimum version of the actual product
- **Pretotype**: Fake version that tests the same hypothesis with 1% of the effort

Key principle: **measure behaviour, not opinions.** People will tell you your idea is great to be nice. But will they sign up? Click "buy"? Share their email? Behaviour doesn't lie.

## Instructions

> Read CONVENTIONS.md for web search policy, DA proxy rules, and search volume proxies. These apply throughout this skill.

### Step 1: Write the Hypothesis

Help the user write a testable hypothesis in XYZ format:

**"At least X% of Y will Z."**

- **X%**: What percentage would make this worth building? (Be realistic - not 100%)
- **Y**: Specific audience (not "people" - who exactly?)
- **Z**: Specific behaviour you can measure (not "like it" - what will they DO?)

Examples:
- "At least 5% of indie developers who see my landing page will sign up for the waitlist."
- "At least 10% of freelancers who see a tweet about this tool will click the link."
- "At least 2% of visitors to my landing page will click the 'Buy Now' button at $29."

Bad hypotheses:
- "People will like my app" (can't measure "like")
- "Developers need this" (need =/= will pay)
- "This will go viral" (not a testable behaviour)

### Step 2: Choose a Pretotype Type

Recommend the best pretotype for the user's situation. Here are the main types:

**1. Landing Page Test** (most common for vibecoders)
- Build a one-page site describing the product
- Include a clear CTA (waitlist, "buy now", "get early access")
- Drive traffic from Reddit, Twitter/X, or paid ads
- Measure: sign-up rate, click-through rate on CTA
- Cost: $0-50 | Time: 2-4 hours
- Best for: SaaS tools, digital products, apps

**2. Fake Door Test**
- Add a button or link for the feature in an existing product or website
- When clicked, show "coming soon" or collect emails
- Measure: click rate, email capture rate
- Cost: $0 | Time: 1-2 hours
- Best for: New features in existing products

**3. Concierge Test**
- Deliver the service manually to 5-10 people
- Don't build any technology - just do the work by hand
- Measure: do they come back? Will they pay?
- Cost: Your time | Time: 1-2 weeks
- Best for: Services, marketplaces, complex products

**4. Pre-Order / Waitlist**
- Describe the product and ask for money or commitment upfront
- Use Stripe, Gumroad, or a simple checkout page
- Measure: conversion rate, actual purchases
- Cost: $0-20 | Time: 2-4 hours
- Best for: Products where willingness to pay is the key question

**5. Explainer Video Test**
- Create a short video (60-90 seconds) showing how the product would work
- Post on YouTube, Twitter/X, or Reddit
- Measure: views, engagement, click-through to sign-up
- Cost: $0 | Time: 3-5 hours
- Best for: Products that are hard to explain in text
- Tools: Loom (free), OBS Studio, or phone screen recording

**6. Reddit/Community Post**
- Describe the problem and your proposed solution in a relevant subreddit or community
- Don't pitch - ask if people have this problem and how they solve it today
- Measure: upvotes, comments, DMs asking "where can I get this?"
- Cost: $0 | Time: 30 minutes
- Best for: Quick demand signal before investing more time

### Step 3: Design the Experiment

For the chosen pretotype, specify:

1. **What to build**: Exactly what to create (landing page copy, video script, Reddit post, etc.)
2. **Where to test**: Where to drive traffic (which subreddit, which Twitter audience, which community)
3. **How long to run**: Minimum time for meaningful data (usually 3-7 days)
4. **Success metric**: What specific number means "proceed"
5. **Failure metric**: What specific number means "stop"

### Step 4: Set Success Criteria

Help the user define clear pass/fail thresholds:

| Pretotype Type | Good Signal | Weak Signal | Bad Signal |
|---|---|---|---|
| Landing page sign-ups | 10%+ conversion | 3-9% conversion | Under 3% conversion |
| Fake door clicks | 5%+ click rate | 2-4% click rate | Under 2% click rate |
| Pre-order purchases | Any purchases at target price | Sign-ups but no purchases | No engagement |
| Reddit post | 50+ upvotes, DMs asking for it | 10-49 upvotes, some interest | Under 10 upvotes, no interest |
| Explainer video | High retention + sign-ups | Views but no action | Low views, high drop-off |

These are baseline benchmarks assuming cold traffic with no prior audience. Adjust thresholds up or down based on traffic source quality and community size.

Important: define these BEFORE running the test. Don't move the goalposts after.

### Step 5: Output the Pretotype Plan

```
## Pretotype Plan: [Product Name]

**Idea**: [one-sentence description]
**Date**: [today]

### Hypothesis
"At least [X]% of [Y] will [Z]."

### Pretotype Design

| Element | Detail |
|---|---|
| Type | [Landing page / Fake door / Concierge / Pre-order / Video / Community post] |
| What to build | [specific description] |
| Where to test | [specific channels] |
| Duration | [X days] |
| Cost | [$X or free] |
| Time to set up | [X hours] |

### Success Criteria

| Metric | Pass | Borderline | Fail |
|---|---|---|---|
| [primary metric] | [number] | [number] | [number] |
| [secondary metric] | [number] | [number] | [number] |

### Traffic Plan
- [Channel 1]: [how to drive traffic + expected reach]
- [Channel 2]: [how to drive traffic + expected reach]

### What Happens Next
- **If pass**: [next step - build MVP, start deeper validation, etc.]
- **If borderline**: [next step - try idea-flip, test different audience, etc.]
- **If fail**: [next step - park idea, try different idea, etc.]
```

Save as markdown.

### Step 6: Offer Next Steps

- "Want me to **write the landing page copy** for this pretotype?" (suggest sales-page-structure skill from ff-pricing-selling when available)
- "Want to **identify your riskiest assumptions** before testing? Use the assumption-check skill."
- "Want to **check if there's search demand** for this idea? Use the validate-idea skill."

## Key Principles

1. **Skin in the game matters.** An email sign-up is weaker than a credit card. A "looks cool" comment is weaker than an email. The more effort or commitment the user gives, the stronger the signal.
2. **Your own data beats everything.** Don't rely on market reports, competitor revenue estimates, or "the market size is $X billion." Run YOUR test with YOUR audience.
3. **Behaviour over opinions.** "Would you use this?" is a useless question. "Here's the sign-up page - will you sign up?" is a real test.
4. **Speed over polish.** A pretotype that takes 2 weeks is too slow. If you can't test it in under a week, simplify the test.

## Notes

- This skill works best AFTER validate-idea (confirm search demand) and assumption-check (find what to test)
- A failed pretotype is a success - you saved months of building the wrong thing
- Don't build features for the pretotype. The whole point is to test demand WITHOUT building the product.
- Vibecoders are especially tempted to skip the pretotype and just build. Resist. Building is the easy part. Finding users is the hard part.

**Framework attribution**: Based on Alberto Savoia's pretotyping methodology from "The Right It" (2019). See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [Pretotyping: Validate Your App Idea in a Weekend, Not a Month](https://fantasticfounder.com) - Six pretotype formats to test demand with zero code
