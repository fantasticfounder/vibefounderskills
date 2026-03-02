---
name: pricing-strategy
description: "Choose the right pricing model and set your first price. Uses Van Westendorp, value-based pricing, and the 10x rule. Covers flat-rate, tiered, per-seat, usage-based, freemium, and lifetime deals with a decision tree for indie SaaS. Triggers: pricing strategy, how to price, what should I charge, pricing model, freemium vs paid, free trial, pricing page, how much to charge."
---

# Choose Your Pricing Strategy

Pick the right pricing model for your product, set your first price, and design tiers that make sense. This skill walks you through a decision tree built for indie SaaS and app founders - not enterprise pricing playbooks that assume you have a sales team.

## Context

You are helping a founder choose a pricing strategy for: **$ARGUMENTS**.

If the user provides positioning work, customer research, competitor analysis, monetization model evaluation, or any prior context from this session, read those first and use them.

## The Frameworks

This skill draws on several pricing methodologies:

- **Van Westendorp Price Sensitivity Meter** - a survey-based method that identifies the acceptable price range by asking four questions (too cheap, cheap, expensive, too expensive). Developed by Dutch economist Peter van Westendorp in 1976. Useful for validating a price range before launch.
- **Value-based pricing** - pricing based on what the customer is willing to pay for the outcome, not what it costs you to build. The foundation of SaaS pricing. Patrick Campbell (ProfitWell/Paddle) has written extensively on this for SaaS specifically.
- **Competitor-based pricing** - anchoring against what alternatives charge. Useful as a sanity check, dangerous as a primary strategy (you inherit their positioning).
- **Cost-plus pricing** - adding a margin to your costs. Works for physical goods. Almost always wrong for software because your marginal cost is near zero and your value to the customer has nothing to do with your hosting bill.
- **The 10x rule** - charge roughly 1/10th of the value you deliver. If your tool saves $1,000/month in time, charge ~$100/month. This gives customers a clear ROI while capturing meaningful revenue.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Understand the Product's Value

Before touching pricing models, you need to understand what value this product actually delivers. Ask or determine:

1. **What outcome does it deliver?** Not features - the end result. "Saves 5 hours per week on meeting follow-ups" is an outcome. "AI-powered meeting notes" is a feature.
2. **What's the alternative, and what does it cost?** What do people use today? A competitor ($X/month), a manual process (Y hours at $Z/hour), hiring someone ($W/month), or doing nothing (and suffering)?
3. **What time, money, or effort does it save?** Put a rough number on it. Even a back-of-napkin estimate gives you a pricing anchor.
4. **Who is the buyer?** A solo founder spending their own money prices differently than a team lead with a company card. B2B and B2C have radically different willingness to pay.

If the user has completed value-proposition or positioning-canvas work in this session, pull the "What Before" and "What After" sections directly - they contain most of what you need here.

### Step 2: Evaluate Pricing Models

Walk through this decision tree. Each model fits specific product types. Don't default to "tiered SaaS pricing" just because that's what everyone does.

**Flat-rate pricing**
- One price, one plan, everyone gets everything
- Best for: Simple products with one audience segment. Products where usage doesn't vary much between customers.
- The Basecamp model: "One plan, $99/month, everything included." Works when simplicity IS the positioning.
- Pros: Dead simple. No decision fatigue. Easy to communicate.
- Cons: Leaves money on the table from high-value users. Can't segment.
- Choose this when: Your product does one thing well for one type of customer.

**Tiered pricing (2-3 tiers)**
- Multiple plans at different price points, each with increasing features or limits
- Best for: Products that serve different user segments (solo vs team, basic vs power user)
- The most common SaaS model for a reason - it captures different willingness-to-pay levels.
- Pros: Captures more value. Creates upgrade path. Middle tier becomes the "obvious choice."
- Cons: Requires clear differentiation between tiers. Feature gating decisions are hard.
- Choose this when: You have meaningfully different user segments with different needs.

**Per-seat pricing**
- Price multiplied by number of users
- Best for: Collaboration and team products where more users = more value
- Pros: Revenue scales with adoption. Simple to understand.
- Cons: Discourages adoption (teams add fewer seats to save money). Punishes collaboration.
- Choose this when: Your product genuinely gets more valuable with more team members using it.

**Usage-based pricing**
- Pay for what you use (API calls, credits, storage, compute)
- Best for: APIs, AI products, infrastructure tools, or anything where value varies dramatically between users
- Pros: Low barrier to entry. Revenue scales with value delivered. Fair.
- Cons: Revenue is unpredictable. Customers worry about surprise bills. Hard to forecast MRR.
- Choose this when: A customer using 100x more gets 100x more value, and a flat price would be unfair to light users.

**Freemium**
- Free tier (limited) + paid tier(s)
- Best for: Products with network effects, viral sharing mechanics, or where the free tier acts as a marketing channel
- The Notion model: free is genuinely useful, paid unlocks power features.
- Pros: Massive top-of-funnel. Low friction. Users sell themselves.
- Cons: Most users never pay (typical conversion 2-5%). Free users cost money to serve. Can devalue the product.
- Choose this when: Free users generate value for you (content, network effects, word of mouth) OR the product sells itself once people use it.

**One-time purchase / Lifetime Deal (LTD)**
- Pay once, use forever
- Best for: Solo tools, plugins, templates, utilities. Products with low ongoing development costs.
- The AppSumo / Gumroad model.
- The LTD debate for indie founders:
  - **Pros:** Immediate cash flow (critical when bootstrapping). Great for launch momentum. AppSumo can put you in front of thousands of buyers fast. LTD customers become evangelists. Validates demand with real money.
  - **Cons:** You sell future revenue for present cash. LTD customers use support forever but never pay again. If your costs grow (AI API calls, storage), LTD users become a liability. Hard to transition LTD users to subscription later.
  - **When LTDs make sense:** Early stage cash injection. Products with near-zero marginal cost. When you plan to evolve the product beyond what the LTD covers (LTD gets v1 features, subscription gets v2+).
  - **When LTDs are dangerous:** Products with ongoing per-user costs. When you need predictable MRR. When LTD customers will comprise >50% of your user base.
- Choose this when: The product is self-contained, has low marginal costs, and you want fast cash or launch buzz.

### Step 3: Research Competitor Pricing

Use web search to check what alternatives charge. Search for:
- `"[product type] pricing"` - direct competitors
- `"[product type] alternatives"` - comparison pages that list pricing
- `"[specific competitor] pricing"` - if you know names

For each competitor found, note:
- Their pricing model (flat, tiered, usage, freemium, etc.)
- Their price points
- What feature gates they use between tiers
- Whether they have a free tier or trial

This is a sanity check, not a strategy. You're not trying to match competitors - you're trying to understand the price range customers expect so you can position within or deliberately outside it.

If web search is unavailable, ask the user to provide competitor pricing data. Do not fabricate pricing.

### Step 4: Apply Value-Based Pricing

Now calculate what the product is worth to the customer:

1. **Quantify the value delivered**: Time saved (hours x hourly rate), money saved, revenue generated, pain eliminated. Use the numbers from Step 1.
2. **Apply the 10x rule**: Charge roughly 1/10th of the value delivered. If your tool saves $250/week ($1,000/month), charge ~$100/month. This gives the customer a clear 10x return and makes the price a no-brainer.
3. **Adjust for market context**:
   - B2C products: Customers are more price-sensitive. You might need to charge 1/20th or 1/50th of value.
   - B2B products with company budgets: 1/10th is standard and accepted.
   - Competitive markets: Price might need to be lower to win adoption, then increase.
   - New categories: You might need to price aggressively low to create the market, then raise.

4. **Check against Van Westendorp ranges** (if you can survey customers):
   - "At what price would this be so cheap you'd question the quality?" (floor)
   - "At what price is this a bargain - a great deal?" (low anchor)
   - "At what price is this getting expensive but you'd still consider it?" (high anchor)
   - "At what price is this too expensive to consider?" (ceiling)
   - Your price should sit between the "bargain" and "getting expensive" answers.

If you can't survey customers yet, use the 10x rule as your starting point and plan to validate through conversations and experiments (Step 7).

### Step 5: Design Pricing Tiers

If you chose tiered pricing, design 2-3 tiers:

**Tier design principles:**
- **2-3 tiers max** for indie products. More creates decision fatigue. Enterprise can do 4, but you're not enterprise.
- **Name tiers by who they're for**, not by size: "Solo," "Team," "Agency" is better than "Basic," "Pro," "Enterprise."
- **Gate features on value metrics** - the thing that increases as the customer gets more value. For a CRM: number of contacts. For an email tool: number of sends. For an analytics tool: number of tracked events. Not arbitrary limits like "3 projects" when 10 would be fine.
- **Make the middle tier the obvious choice.** This is the one most people should buy. Price it at the sweet spot from Step 4. The bottom tier exists for people who aren't ready. The top tier exists to make the middle look reasonable.

**Tier template:**

| | Free / Starter | Pro (recommended) | Team |
|---|---|---|---|
| **Price** | $0 or $X/mo | $Y/mo | $Z/mo |
| **For** | [who] | [who] | [who] |
| **Value metric limit** | [amount] | [amount] | [amount] |
| **Key features** | [list] | [everything in Starter +] | [everything in Pro +] |
| **What's gated** | [missing features] | [what they get that Free doesn't] | [team/collab features] |

### Step 6: Set the Anchor

Pricing psychology matters:

- **Show the recommended tier visually**: highlight it, add a badge ("Most Popular"), use colour.
- **Annual discount**: Offer 2 months free on annual billing (16.7% discount). This improves cash flow and reduces churn.
- **Round numbers vs .99 pricing**: For SaaS, use round numbers ($29/mo, $49/mo, $99/mo). Rounded prices signal quality and simplicity. The $X.99 trick is for retail, not software.
- **Price anchoring**: If you show value delivered ($1,000/month saved) next to your price ($99/month), the price feels small.

### Step 7: Plan Pricing Experiments

Your first price is a hypothesis. Test it:

1. **Landing page price test**: Create two versions of your pricing page and split traffic. Even small traffic (100 visitors per variant) gives directional signal.
2. **Conversation test**: In founder-led sales conversations, quote the price and read the reaction. "That's it?" means you're too cheap. Long pause means you're at the ceiling. Immediate yes means you might be leaving money on the table.
3. **"What would you pay?" interviews**: Not perfectly reliable (people underestimate willingness to pay) but useful for identifying the ceiling. Ask: "What would this need to do for you to pay $X?" - this tells you the feature threshold, not just the number.
4. **Willingness-to-pay survey**: Use the Van Westendorp four questions with 20-30 target customers. Even a Twitter/X poll can give rough signal.

### Step 8: Output the Pricing Strategy

```
## Pricing Strategy: [Product Name]

**Date**: [today]

### Product Value Analysis
- **Outcome delivered**: [what the customer achieves]
- **Alternative cost**: [what they pay or sacrifice today]
- **Value delivered**: [quantified in $/time]
- **Buyer context**: [B2B/B2C, budget size, price sensitivity]

### Recommended Pricing Model
**Model**: [flat-rate / tiered / per-seat / usage-based / freemium / LTD]
**Why this model**: [rationale tied to product type and audience]
**Why NOT [alternative model]**: [brief rationale for ruling out the next-best option]

### Pricing Tiers

| | [Tier 1] | [Tier 2 - Recommended] | [Tier 3] |
|---|---|---|---|
| **Price** | [price] | [price] | [price] |
| **For** | [who] | [who] | [who] |
| **Value metric** | [limit] | [limit] | [limit] |
| **Key features** | [list] | [list] | [list] |

### Value Metric
**What you charge on**: [the metric that scales with customer value]
**Why this metric**: [rationale]

### Competitor Context
| Competitor | Model | Price Range | Notes |
|---|---|---|---|
| [name] | [model] | [range] | [key observation] |

### Key Assumption to Test
[The single riskiest assumption in this pricing - the one that could make it all wrong]

### Risks
- [Risk 1 and mitigation]
- [Risk 2 and mitigation]

### Pricing Experiments to Run
1. [Experiment 1]: [what to test and how]
2. [Experiment 2]: [what to test and how]
```

Save as markdown.

## Common Mistakes

- **Pricing based on costs.** Your hosting bill is $20/month. Your product saves people $500/month. Charging $29/month because "it only costs me $20 to run" is leaving $70+/month on the table.
- **Starting too low.** It's psychologically easier to lower prices than raise them. Start at the high end of your range and discount if needed. Founders who undercharge attract price-sensitive customers who churn fast.
- **Too many tiers.** Three is the max for indie. Four or five tiers creates analysis paralysis. You're not Salesforce.
- **Gating on the wrong metric.** If your value metric is "number of projects" but your customers only ever have 2-3 projects, the limit doesn't drive upgrades. Gate on the thing that actually increases when someone gets more value.
- **Copying competitor pricing without understanding their positioning.** A VC-backed competitor can afford to undercharge for years to win market share. You can't. Price for your business model, not theirs.
- **Never changing the price.** Your first price is wrong. Plan to revisit every 3-6 months as you learn more about willingness to pay.

## Notes

- This skill pairs with monetization-model (which evaluates revenue model types) and offer-creation (which wraps the price in a compelling offer)
- If used within the /price command, the monetization model evaluation feeds directly into the model selection here
- Pricing is the highest-leverage growth lever for indie SaaS. A 1% improvement in pricing has more impact than a 1% improvement in acquisition or retention (Patrick Campbell, ProfitWell)

---

### Further Reading

- [How to Price a SaaS Product When You Have No Idea What to Charge](https://fantasticfounder.com) - Pricing frameworks for indie SaaS and micro-SaaS founders
