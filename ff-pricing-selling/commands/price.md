---
description: Run a full pricing and selling workflow - pricing model, offer creation, sales page structure, and objection handling
argument-hint: "<your product or app>"
---

# /price -- Full Pricing & Selling Strategy

Price your product and learn to sell it: evaluate monetization models, set your price, create a compelling offer, structure your sales page, and prepare for objections - all in one workflow.

## Invocation

```
/price AI meeting notes tool for freelancers
/price Shopify analytics dashboard for indie store owners
/price [paste your product description]
```

## Workflow

### Step 1: Understand the Product

Ask:
- What does your product do? (one sentence)
- Who is it for? (specific audience, not "everyone")
- What do they currently pay for alternatives? (competitor products, manual processes, hiring someone, or nothing)
- What outcome does your product deliver? (not features - the end result)
- Have you done any positioning or validation work? (if so, share it)

Accept context from uploaded files, prior skill outputs, competitor research, or conversation.

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These rules govern the entire workflow.

If the founder's product description is less than 3 sentences, ask clarifying questions before proceeding. If a full paragraph or more, proceed and surface gaps during checkpoints.

### Step 2: Evaluate Monetization Models (~10 min)

Apply the **monetization-model** skill:

- Classify the product type and value delivery pattern
- Score all 8 monetization models on predictability, effort, alignment, and scalability
- Recommend 1-2 models with rationale
- Design the evolution path (how the model evolves as you grow)
- Suggest validation experiments

**Checkpoint**: "Based on your product type, [model] is the strongest fit. Here's why: [rationale]. Does this match your instinct, or do you see a different path?"

If the user disagrees or has a strong preference, adjust and re-derive downstream outputs from their chosen model.

### Step 3: Set Pricing (~15 min)

Apply the **pricing-strategy** skill:

- Understand the product's value (outcome, alternative cost, time/money saved)
- Evaluate pricing models using the decision tree (informed by the monetization model chosen in Step 2)
- Research competitor pricing via web search
- Apply value-based pricing and the 10x rule
- Design pricing tiers (2-3 tiers max for indie)
- Set the anchor and plan pricing experiments

**Checkpoint**: "Here's your recommended pricing: [model] at [price points]. The key assumption to test is [assumption]. Does this feel right for your market?"

If the user pushes back on price, explore why. Often "that feels too high" means the value framing needs work (which Step 4 addresses), not that the price is wrong.

### Step 4: Create the Offer (~10 min)

Apply the **offer-creation** skill:

- Identify the dream outcome (using value proposition work if available)
- Apply Hormozi's Value Equation
- Build the value stack (core product + bonuses that reduce time, effort, and risk)
- Set the price anchor (total value vs price)
- Add risk reversal (guarantee type and wording)
- Create urgency mechanism (real, not fake)
- Write the offer summary paragraph

Thread the pricing from Step 3 directly into the offer. The offer should make the price from Step 3 feel like a steal.

### Step 5: Structure the Sales Page (~15 min)

Apply the **sales-page-structure** skill:

- Gather all inputs from prior steps (product, audience, value prop, pricing, offer)
- Build section-by-section page structure: Hero, Problem (PAS), Solution, How It Works, Features/Benefits, Social Proof, Pricing, FAQ, Final CTA
- Write actual copy recommendations for each section (not just descriptions)
- Include headline options and CTA text
- Flag missing elements the founder still needs (screenshots, testimonials, etc.)

Thread the offer framing from Step 4 into the pricing and CTA sections. Thread the value proposition from positioning work (if available) into the Hero and Solution sections.

### Step 6: Prepare the Objection Playbook (~10 min)

Apply the **objection-handler** skill:

- Identify the product's top objections based on pricing, positioning, and competitive landscape
- Build response frameworks for 5-8 key objections (Acknowledge - Explore - Reframe - Bridge)
- Include the selling mindset section (you're helping, not convincing)
- Provide channel-specific responses (email, DM, call, FAQ)
- Design the follow-up cadence

Thread the pricing from Step 3 and guarantee from Step 4 into the objection responses. "It's too expensive" responses should reference the specific value and guarantee already decided.

### Step 7: Generate the Full Pricing & Selling Report

Note: Full skill outputs from each step should be saved as separate files (e.g., `[slug]-monetization-model.md`, `[slug]-pricing-strategy.md`). This report is a summary that ties everything together.

```
## Pricing & Selling Strategy: [Product Name]
**Product**: [one-sentence]
**Date**: [today]
**Generated by**: FantasticFounder Pricing & Selling Strategy

### 1. Monetization Model
**Recommended model**: [model]
**Why**: [rationale]
**Evolution path**: [how the model evolves as you grow]

### 2. Pricing
**Model**: [flat/tiered/usage/etc.]
**Tiers**:

| | [Tier 1] | [Tier 2 - Recommended] | [Tier 3] |
|---|---|---|---|
| **Price** | [price] | [price] | [price] |
| **For** | [who] | [who] | [who] |
| **Key features** | [list] | [list] | [list] |

**Value metric**: [what you charge on]
**Key assumption to test**: [the riskiest pricing assumption]

### 3. The Offer
**Value stack**:

| Component | Value |
|---|---|
| Core product | $[value] |
| [Bonus 1] | $[value] |
| [Bonus 2] | $[value] |
| [Bonus 3] | $[value] |
| **Total value** | **$[sum]** |
| **Your price** | **$[price]** |

**Risk reversal**: [guarantee type and wording]
**Urgency**: [mechanism if applicable]
**Offer summary**: [one paragraph]

### 4. Sales Page Structure
**Hero headline**: [recommended headline]
**Problem**: [one-sentence summary]
**How it works**: [3 steps]
**Key CTA**: [text and action]
**FAQ topics**: [list of 5 objection-as-question topics]

[Note: Full section-by-section copy in the separate sales-page-structure output file]

### 5. Objection Playbook

| Objection | One-Line Response |
|---|---|
| [objection 1] | [response] |
| [objection 2] | [response] |
| [objection 3] | [response] |
| [objection 4] | [response] |
| [objection 5] | [response] |

**Follow-up cadence**: [summary - e.g., "5 touchpoints over 21 days via email"]

[Note: Full responses with channel-specific scripts in the separate objection-handler output file]

---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

Save as markdown.

### Step 8: Offer Next Steps

- "Want to **validate demand** before investing more in sales? Use the ff-idea-validation plugin."
- "Want to **position your product** more clearly? Use the ff-positioning plugin."
- "Want to **plan your launch** with this pricing? Use the ff-launch-acquisition plugin."
- "Ready to **build the actual landing page**? Take the sales page structure to Cursor or Replit and ship it."

## Notes

- Allow 60-90 minutes across multiple exchanges
- At each checkpoint, the user can redirect, go deeper, or change direction. If they change direction, re-derive all downstream outputs from the new input.
- Pricing is a hypothesis, not a commitment. The output should be treated as a starting point to test, not a final answer.
- The strongest pricing and selling strategy comes from real customer conversations, not just analysis. If the user hasn't talked to customers yet, flag this at Step 1.
