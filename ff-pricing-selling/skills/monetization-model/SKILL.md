---
name: monetization-model
description: "Evaluate how to make money from your app beyond just subscriptions. Scores 8 monetization models on predictability, effort, alignment, and scalability with indie-specific guidance. Triggers: monetization, how to monetize, revenue model, make money from my app, business model, how to monetize an app."
---

# Evaluate Your Monetization Model

Figure out how to actually make money from your app. Not every product should be a subscription SaaS. This skill evaluates 8 monetization models with scoring specific to indie founders and solo builders - not VC-backed companies optimising for growth-at-all-costs.

## Context

You are helping a founder evaluate monetization models for: **$ARGUMENTS**.

If the user provides product details, positioning work, customer research, or any prior context from this session, read those first and use them.

## The Framework

This skill uses a structured evaluation of 8 monetization models, scored on four dimensions. The models draw on patterns observed across thousands of indie founders documented on Starter Story and Indie Hackers, and real-world case studies from bootstrapped companies.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Understand the Product Type

Before evaluating models, classify the product. Ask or determine:

1. **What type of product is this?**
   - SaaS (software as a service - ongoing tool)
   - Tool / Utility (does one specific thing)
   - Marketplace (connects buyers and sellers)
   - Content product (courses, guides, templates, media)
   - API / Infrastructure (developers consume it programmatically)
   - Community / Network (value comes from members)
   - Hybrid (combination - specify which)

2. **What's the value delivery pattern?**
   - Ongoing value (the product is useful every day/week/month) - favours subscription
   - One-time value (solves a problem once) - favours one-time purchase
   - Variable value (some users get 100x more than others) - favours usage-based
   - Network value (more users = more value for everyone) - favours freemium

3. **What are the marginal costs?**
   - Near zero (static content, simple SaaS) - any model works
   - Per-user costs (AI API calls, storage, compute per customer) - must price above marginal cost
   - High transaction costs (payment processing, shipping) - factor into model

### Step 2: Evaluate 8 Monetization Models

Score each model on four dimensions (1-5 scale):

**Scoring criteria:**
- **Revenue predictability** (1-5): How reliable and forecastable is the income? 5 = highly predictable recurring revenue. 1 = feast-or-famine.
- **Effort to implement** (1-5, inverted): How much work to set up and maintain? 5 = plug in Stripe and go. 1 = requires complex infrastructure, payment splitting, or marketplace mechanics.
- **Alignment with product** (1-5): How well does this model match how the product delivers value? 5 = the model perfectly mirrors value delivery. 1 = the model fights the product's nature.
- **Scalability** (1-5): Can revenue grow without proportional increase in your time? 5 = revenue scales with zero marginal effort. 1 = every dollar requires your direct time.

**Model 1: Subscription SaaS (recurring MRR)**
The default. Monthly or annual recurring payments for access to software.
- When it works: Value is ongoing. Customers use the product regularly. Switching costs keep churn low.
- When it fails: Product solves a one-time problem. Customers don't use it often enough to justify monthly billing.
- Indie examples: Plausible Analytics (paid-only, no free tier, bootstrapped to $100K+ MRR), Fathom Analytics, Carrd.
- Watch out for: Churn. If monthly churn exceeds 5-8%, the subscription model becomes a leaky bucket.

**Model 2: Lifetime Deals (LTD)**
One-time payment for permanent access. Often launched via AppSumo or self-sold via LemonSqueezy/Gumroad.
- When it works: Early stage cash injection. Products with low per-user marginal costs. When you want fast validation and launch buzz.
- When it fails: Products with ongoing per-user costs (AI APIs). When LTD customers become >50% of your base and you can't fund development.
- Indie examples: AppSumo launches (thousands of indie tools), many Notion/Obsidian plugin developers.
- Watch out for: Selling your future for present cash. LTD customers use support forever. Plan the transition to subscription before launching the LTD.

**Model 3: Freemium + Premium**
Free tier that's genuinely useful. Paid tier that unlocks power features or higher limits.
- When it works: The free tier drives adoption AND the product sells itself once people use it. Network effects or viral sharing exist.
- When it fails: Free users don't convert (typical rate: 2-5%). Free users cost significant money to serve with no upgrade path.
- Indie examples: Notion (free personal, paid team), Cal.com (open source + paid cloud), Excalidraw.
- Watch out for: The "free forever" expectation. Once you train users that your product is free, converting them is hard.

**Model 4: Usage-Based / Pay-Per-Use**
Customers pay based on consumption: API calls, AI credits, storage, events tracked, emails sent.
- When it works: Value varies dramatically between users. Light users would never pay a flat fee. Heavy users get enormous value.
- When it fails: Customers can't predict their bill (anxiety). Your product's value doesn't scale linearly with usage.
- Indie examples: OpenAI API (per-token), Vercel (per-compute), Resend (per-email).
- Watch out for: Unpredictable revenue. Consider hybrid: base subscription + usage overage.

**Model 5: Marketplace / Transaction Fees**
You take a percentage of each transaction between buyers and sellers on your platform.
- When it works: You're connecting two sides of a market. The transaction wouldn't happen without you.
- When it fails: Chicken-and-egg problem (need buyers to attract sellers, need sellers to attract buyers). Disintermediation risk (they take the deal off-platform).
- Indie examples: Gumroad (creator tools + marketplace), Toptal, micro-SaaS directories.
- Watch out for: The cold start problem. Marketplaces are the hardest business model to bootstrap.

**Model 6: Template / Asset Sales**
One-time purchases of digital products: templates, themes, plugins, datasets, design assets.
- When it works: You can create once and sell many times. The asset solves a specific, well-understood problem.
- When it fails: Commoditised market with free alternatives. No repeat purchase reason.
- Indie examples: Gumroad creators, ThemeForest sellers, Notion template creators, Tailwind UI.
- Watch out for: Revenue is lumpy. No recurring income unless you keep releasing new assets. Consider a bundle or membership to add recurrence.

**Model 7: Sponsorship / Advertising**
Revenue from sponsors or ad placements. Requires large, engaged audience.
- When it works: You have massive traffic (100K+ monthly visitors) or a highly targeted niche audience. Content-first businesses.
- When it fails: Almost always fails for indie software products. Traffic is too low. Ads degrade the user experience.
- Indie examples: Newsletter sponsors (Morning Brew, The Hustle before acquisition), niche blogs.
- Watch out for: You need scale that most indie products never reach. Consider this as a secondary model, not primary.

**Model 8: Consulting / Done-For-You**
Your product is your marketing. Your time is the product. You charge for implementation, strategy, or custom work.
- When it works: You're an expert in what your product does. Clients want the outcome, not the tool. High-ticket B2B.
- When it fails: You want passive income. You want to scale beyond your own time.
- Indie examples: Many developer tool founders do consulting on the side. Agency owners who build tools for their workflows and sell them.
- Watch out for: Consulting doesn't scale. The goal is usually to use consulting revenue to fund product development, then transition to product-only.

### Step 2b: Research Competitor Monetization (Web Search)

Before scoring, search for how competitors and similar products monetize. This grounds your evaluation in reality, not theory.

**Search for:**
- `"[product type] pricing"` - see how similar products charge
- `"[top competitor] pricing page"` - check actual price points and models
- `"[product type] monetization model"` or `"how does [competitor] make money"` - understand revenue strategy
- `"[product type] AppSumo"` or `"[product type] lifetime deal"` - check if LTDs are common in this space

**What to extract:**
- Which models are most common for this product type (subscription vs one-time vs freemium)?
- What price ranges are competitors using?
- Are there successful indie examples of unusual models (LTDs, template sales, consulting-led)?
- Is there a dominant model that customers expect? (e.g., design tools = freemium; developer tools = usage-based)

Use this research to inform your scoring in Step 3. A model that competitors have validated is lower risk. A model nobody uses might be a differentiation opportunity or a warning sign.

### Step 3: Score Each Model

Create the evaluation table:

| Model | Predictability | Effort to Implement | Alignment | Scalability | Total |
|---|---|---|---|---|---|
| Subscription SaaS | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Lifetime Deals | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Freemium + Premium | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Usage-Based | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Marketplace Fees | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Template / Asset Sales | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Sponsorship / Ads | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |
| Consulting / DFY | [1-5] | [1-5] | [1-5] | [1-5] | [/20] |

For any score of 4 or 5, state the specific evidence. For any score of 1 or 2, state what's missing. Follow the scoring conventions in CONVENTIONS.md.

### Step 4: Recommend and Design the Evolution Path

Based on the scores:

1. **Recommend 1-2 models to start with.** The top scorer is your primary model. If a secondary model scores within 2 points and complements (not competes with) the primary, recommend it as a secondary revenue stream.

2. **Design the evolution path.** Most indie products evolve their monetization over time. Common paths:
   - LTD launch -> subscription migration after 6 months
   - Consulting first -> productise the service -> SaaS
   - Freemium for adoption -> paid tiers as features mature
   - Template sales -> subscription for updates and new templates
   - Usage-based -> hybrid (base fee + usage) for predictability

3. **Include validation experiments**: How can the founder test this model before fully building it?
   - Pre-sell at the target price (validate willingness to pay)
   - Offer a "founding member" deal (validate recurring commitment)
   - Do 5 founder-led sales conversations and quote the price
   - Run a landing page with pricing and measure clicks on "Buy" (even before the product exists)

### Step 5: Output the Monetization Evaluation

```
## Monetization Model Evaluation: [Product Name]

**Product type**: [SaaS / Tool / Marketplace / Content / API / Community / Hybrid]
**Value delivery pattern**: [Ongoing / One-time / Variable / Network]
**Marginal cost profile**: [Near zero / Per-user costs / High transaction costs]
**Date**: [today]

### Evaluation Table

| Model | Predictability | Effort | Alignment | Scalability | Total | Notes |
|---|---|---|---|---|---|---|
| [model] | [score] | [score] | [score] | [score] | [/20] | [key observation] |
| ... | ... | ... | ... | ... | ... | ... |

### Recommended Model(s)

**Primary**: [model name]
**Why**: [rationale - what about this product and audience makes this model the best fit]

**Secondary** (optional): [model name]
**Why**: [rationale - how it complements the primary model]

### Evolution Path

**Phase 1 (months 0-6)**: [starting model and why]
**Phase 2 (months 6-18)**: [evolution and trigger for the change]
**Phase 3 (18+ months)**: [mature model]

### Validation Experiments

1. [Experiment]: [what to do, what signal to look for, and how long it takes]
2. [Experiment]: [what to do, what signal to look for, and how long it takes]

### Models Ruled Out

| Model | Why It Doesn't Fit |
|---|---|
| [model] | [specific reason - not just "low score"] |
```

Save as markdown.

## Common Mistakes

- **Defaulting to subscription without thinking.** Subscription is the default SaaS model, but it's not always the best fit. A one-time tool that solves a one-time problem should be a one-time purchase.
- **Picking the model your favourite company uses.** Notion's freemium works because of network effects and a massive market. Your niche tool for accountants might not have either.
- **Ignoring marginal costs.** If each user costs you $5/month in API calls, a $9/month subscription leaves $4/month gross margin. That's a failing business at scale.
- **No evolution path.** What works at 10 customers rarely works at 1,000. Plan the transition before you need it.
- **Trying to monetise everything at once.** Pick one primary model. Nail it. Add a secondary model later when you understand your customers.

## Notes

- This skill feeds directly into pricing-strategy (which sets specific price points) and offer-creation (which wraps the price in a compelling package)
- If used within the /price command, the recommended model from here determines the pricing model evaluated in pricing-strategy
- When scores tie, apply the tiebreaker rules from CONVENTIONS.md: prioritise factors the founder can verify with evidence over factors based on inference

---

### Further Reading

- [How to Monetize an App: 7 Models That Actually Work for Indie Founders](https://fantasticfounder.com) - Beyond subscriptions: real monetization strategies from founders who shipped with Cursor and make money
