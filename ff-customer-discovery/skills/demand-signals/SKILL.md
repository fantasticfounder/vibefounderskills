---
name: demand-signals
description: "Read demand signals from Reddit, Twitter/X, forums, and search behaviour to validate that people want what you're building. Checks 5 signal sources and scores overall demand confidence. Triggers: demand signals, is there demand, do people want this, market demand, validate demand, demand check."
---

# Demand Signals

Check whether real people actually want what you're building - by reading the signals they're already sending.

## Context

You are helping a vibecoder read demand signals for: **$ARGUMENTS**.

If running in sequence from /discover-customers, use the target audience from find-target-audience and the competitive landscape from competitor-scan to scope and inform the demand analysis.

## Why This Matters

Building without checking demand is the number one way vibecoders waste months of effort. You can build a perfect product that nobody wants. The signals that tell you whether demand exists are often already out there - in Reddit threads, Google autocomplete, competitor revenue, and community discussions. You just need to know where to look and what to look for.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Define What "Demand" Means for This Product

Not all demand looks the same. Ask:
- What type of product is this? (SaaS, tool, template, marketplace, mobile app)
- What would demand look like for this product? (people searching for it, complaining about the problem, paying for alternatives, asking for solutions)
- Who is the target audience? (use data from find-target-audience if available)

Establish the demand question clearly: "We're checking whether [target audience] actively wants [product type] to solve [problem]."

### Step 2: Check 5 Signal Sources

Work through each source systematically. Use web search for each one. If web search is unavailable, state this clearly and ask the user to provide the data (per CONVENTIONS.md web search policy).

#### Source 1: Search Signals

Check whether people are searching for this type of product or problem.

**What to search:**
- Google autocomplete: type `[product type]` and `[problem]` into Google and note what autocomplete suggests
- "People Also Ask" boxes: do problem-related searches trigger PAA? (indicates meaningful search activity)
- Related searches: what does Google show at the bottom of the results page?

**What to look for:**
- Product-language queries (containing "tool", "app", "software", "template", "free", "best") = strong signal. People KNOW they want a product.
- Problem-language queries ("how to", "help with", "fix") = moderate signal. People have the problem but may not want a product yet.
- No autocomplete, no PAA = weak signal. Very few people search for this.

**Score**: Strong / Moderate / Weak / None

Per CONVENTIONS.md search volume proxy rules: if no tool data is available, use Google autocomplete and PAA as rough proxies, and flag that you're using proxies.

#### Source 2: Reddit Signals

Reddit is where people complain honestly about problems, recommend tools, and ask for alternatives.

**What to search:**
- `"[product type]" site:reddit.com`
- `"[problem]" site:reddit.com`
- `"[product type] alternative" site:reddit.com`
- Check specific subreddits relevant to the target audience

**What to look for:**
- Thread frequency: How often do people post about this problem/product type? (daily = strong, monthly = moderate, rarely = weak)
- Upvotes: High-upvote threads mean the community cares about this topic
- Comment depth: Long comment threads with detailed responses = people have strong opinions = real pain
- Specific language: Note the exact words and phrases people use (these become your marketing copy)

**Score**: Strong / Moderate / Weak / None

#### Source 3: Twitter/X Signals

Twitter/X shows real-time demand - people complaining, asking for solutions, and praising alternatives.

**What to search:**
- `"[problem]"` on Twitter/X
- `"[product type]"` on Twitter/X
- `"looking for [product type]"` or `"anyone know a good [product type]"`

**What to look for:**
- People actively asking for solutions
- People complaining about the problem
- People praising competitors (proves they care enough to talk about solutions)
- Indie builders launching similar products (proves builder-side demand, check engagement for user-side demand)

**Score**: Strong / Moderate / Weak / None

#### Source 4: Community Signals

Beyond Reddit and Twitter, where does this audience gather?

**What to search:**
- `"[audience] community"`, `"[audience] Discord"`, `"[audience] forum"`
- IndieHackers: search for the product type or problem
- Hacker News: search for related launches or discussions
- Facebook groups, Slack communities, Discord servers relevant to the audience

**What to look for:**
- Active communities discussing this problem (size and engagement matter more than existence)
- People sharing workarounds or manual solutions (proves the job exists)
- Product launches in the space getting engagement (proves interest)

**Score**: Strong / Moderate / Weak / None

#### Source 5: Alternative Signals (Proof of Willingness to Pay)

The strongest demand signal is people already spending money on similar solutions.

**What to look for:**
- Competitors with paid tiers and visible customer counts
- Competitor pricing pages (if they charge $X/month, people are willing to pay $X/month for this)
- Job postings that describe the problem (companies paying salaries to solve it manually = strong demand)
- Freelancers offering services to solve this problem (proves people pay for solutions)
- Kickstarter/Product Hunt launches with strong support

**Score**: Strong / Moderate / Weak / None

### Step 3: Score Each Source

Build the assessment table:

```
| Signal Source | Score | Key Evidence | Demand Language Found |
|---|---|---|---|
| Search signals | [Strong/Moderate/Weak/None] | [what you found] | [exact phrases] |
| Reddit signals | [Strong/Moderate/Weak/None] | [what you found] | [exact phrases] |
| Twitter/X signals | [Strong/Moderate/Weak/None] | [what you found] | [exact phrases] |
| Community signals | [Strong/Moderate/Weak/None] | [what you found] | [exact phrases] |
| Alternative signals | [Strong/Moderate/Weak/None] | [what you found] | [exact phrases] |
```

### Step 4: Calculate Overall Demand Confidence

**High confidence**: Strong signals across 3 or more sources. People are searching, discussing, and paying for solutions. Demand clearly exists.

**Moderate confidence**: Strong signals in 1-2 sources, moderate in others. Demand exists but may be niche, seasonal, or concentrated in specific communities. Worth pursuing with focused execution.

**Low confidence**: Weak or None across most sources. Very little evidence that people want this or are actively looking for solutions. Reconsider the audience, the product framing, or the problem you're solving.

State the confidence level clearly and back it up with the evidence.

### Step 5: Extract Demand Language

This is one of the most valuable outputs of this analysis. Compile the exact words and phrases people use when describing the problem, asking for solutions, or reviewing alternatives. Group them:

```markdown
### Demand Language

**Problem language** (how people describe the pain):
- "[exact phrase from Reddit/Twitter/forums]"
- "[exact phrase]"
- "[exact phrase]"

**Solution language** (how people describe what they want):
- "[exact phrase]"
- "[exact phrase]"
- "[exact phrase]"

**Comparison language** (how people evaluate options):
- "[exact phrase]"
- "[exact phrase]"

**Use these words in**: landing page headlines, app store descriptions, ad copy, blog post titles, and SEO keywords. This is the language of your market. Use it.
```

Based on Ed Sturm's demand validation methodology (Compact Keywords, 2024-2025): the exact words your audience uses are more valuable than any keyword tool suggestion. These phrases come from real people with real needs.

### Step 6: Make a Recommendation

Based on the evidence:

- **High confidence**: "There's real demand for this. People are searching, discussing, and spending money in this space. Proceed with confidence. Focus on [strongest signal source] as your primary distribution channel."
- **Moderate confidence**: "Demand exists but it's not overwhelming. Consider narrowing your audience or adjusting your positioning to match the specific demand language you found. The strongest signal is [source] - start there."
- **Low confidence**: "The signals are weak. Before investing more time, either change your target audience (go back to find-target-audience), reframe the product to match language people actually use, or validate directly through customer interviews (use customer-interview-script)."

Be honest. Low confidence is not a death sentence - it means you need more information or a different angle. But don't dress up weak signals as validation.

## Output

Save as `[product-slug]-demand-signals.md`. The report should include:

1. Demand question statement
2. Source-by-source assessment table
3. Overall confidence score with rationale
4. Demand language compilation
5. Recommendation with specific next steps

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

## Common Mistakes

- **Confusing interest with demand.** People saying "cool idea!" on Twitter is not demand. People spending $50/month on a competitor IS demand.
- **Only checking one source.** Reddit might be silent but Google might be loud. Check all five sources before concluding.
- **Ignoring the "do nothing" signal.** If people have the problem but aren't searching for solutions, aren't discussing it, and aren't paying for alternatives - maybe the pain isn't bad enough to generate demand.
- **Treating search volume as the only signal.** Many valuable niches have low search volume but high willingness to pay. A keyword with 100 searches/month where every searcher spends $100/month is better than a keyword with 10,000 searches/month where nobody pays.
- **Not capturing the language.** The specific words people use are marketing gold. Don't just note whether demand exists - note HOW people talk about it.

## Notes

- This analysis takes 10-20 minutes depending on search result richness
- When running as part of /discover-customers, carry the demand confidence and demand language forward into the final report
- This skill complements validate-idea from the ff-idea-validation plugin. validate-idea focuses on search demand specifically; this skill checks broader signal sources
- If demand confidence is Low, recommend going back to find-target-audience before proceeding with interviews or personas

**Framework attribution**: Demand validation methodology based on Ed Sturm's Compact Keywords framework (2024-2025). See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [Reading Demand Signals Before You Build: A Vibecoder's Guide](https://fantasticfounder.com) - How to validate that people want what you're building using free tools and community signals
