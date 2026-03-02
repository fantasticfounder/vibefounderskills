# Skill Execution Conventions

These conventions apply to ALL skills in the FantasticFounder marketplace. Every skill file should be read alongside these rules.

## Web Search Policy

When a skill requires market data, competitor information, community names, or any real-world verification:

1. **If the user provides data** (keyword research, competitor list, analytics, community names) - use it. Do not override user-provided data with web search.
2. **If the user provides NO data and the skill requires it** - use web search. State what you searched for and what you found. Do not fabricate market data, competitor names, community sizes, or statistics.
3. **If web search is unavailable** - state this clearly. Say: "I don't have access to live search data for this step. To complete this accurately, I'd need you to provide [specific data needed]." Do not silently skip the step or invent plausible-sounding numbers.

**Specific search triggers:**
- Competitor research: Search `"[product type] for [audience]"` and `"[product type] alternatives"`
- Community discovery: Search `"[audience] community Reddit"`, `"[audience] Discord"`, `"[audience] forum"`
- Market sizing: Search `"[industry] market size"`, check subreddit subscriber counts as proxies, look for competitor user counts in press releases or "about" pages
- Domain availability: Search for `[name].com` and check if a live site exists. Caveat: this does not confirm registration status. Advise the founder to check a registrar directly.

## Context Threading Between Skills

When skills are run in sequence (either via a command or manually by the user):

1. **Check conversation history first.** If a prior skill in this session already produced relevant output (keyword data, segment scores, competitor lists), use that data directly. Do not re-ask for information you already have.
2. **When passing context forward**, carry the specific outputs: segment name and score rationale, keyword lists and SERP classifications, competitor names and positioning, value proposition statements.
3. **If the user changes direction at a checkpoint** (e.g., picks a different segment), re-derive all downstream outputs from the new input. Do not mix old and new analysis.

## Scoring and Rubric Rules

When a skill uses a scoring rubric:

1. **Score honestly.** If evidence is missing, score 0 or Low. Do not inflate scores to be encouraging.
2. **When scores tie**, apply this tiebreaker order:
   - Prioritise factors the founder can verify with evidence (demand signals, competitor data) over factors based on inference (growth potential, referral potential)
   - Prioritise factors with higher real-world impact (willingness to pay, pain intensity) over secondary factors (scalability, founder fit)
3. **Document your reasoning.** For any score of 4 or 5, state the specific evidence. For any score of 1 or 2, state what's missing.

## Domain Authority (DA) - Proxy Rules

DA (Domain Authority) is a proprietary Moz metric not available in standard search results. When a skill references DA:

**Use these observable proxies instead:**

| Authority Level | What You See in Search Results |
|---|---|
| **High authority (DA 60+)** | Household brand names: Wikipedia, Forbes, HubSpot, Shopify, Amazon, Google, major SaaS companies, government sites (.gov), universities (.edu) |
| **Medium authority (DA 30-60)** | Established niche blogs, mid-size SaaS companies, well-known industry publications, sites with clear professional design and content depth |
| **Low authority (DA under 30)** | Personal blogs, new startups, forum threads (Reddit, Quora), sites with thin content, unrecognised domain names |

**For SERP classification:**
- **Wide open**: Top 5 results include Reddit threads, Quora answers, personal blogs, or pages that don't directly target the keyword in their title
- **Rankable**: Top 5 results are from medium-authority sites with some keyword targeting, but no dominant player owns the SERP
- **Competitive**: Top 5 results directly target the keyword from established brands with dedicated product/landing pages
- **Blocked**: Top 5 results are all from high-authority household brands (Google, Amazon, Forbes, Wikipedia) - a new site cannot realistically rank here

**For AI Overviews / Featured Snippets**: If an AI Overview appears for a keyword, note it. AI Overviews absorb clicks and reduce the value of ranking organically. Downgrade the keyword's opportunity by one level (e.g., "Rankable" becomes "Competitive" if an AI Overview dominates).

## Search Volume - Proxy Rules

Monthly search volume requires tools like Moz, Ahrefs, or SEMrush. When a skill references specific volume thresholds:

1. **If the user provides tool data** (Moz volume, Ahrefs estimates) - use it directly.
2. **If no tool data is available**, use these rough proxies:
   - Google autocomplete suggestions = at least moderate search volume
   - "People also ask" boxes = the topic has meaningful search activity
   - Multiple Reddit threads discussing the exact problem = problem-aware demand exists
   - No autocomplete, no PAA, no Reddit threads = very low or zero search volume
3. **Always flag when you're using proxies**: "I don't have exact search volume data. Based on Google autocomplete and Reddit activity, demand appears [strong/moderate/weak]."

## Framework Attribution

When a skill uses an established framework, cite the source inline so the user knows where to go deeper:

| Framework | Attribution |
|---|---|
| Jobs to Be Done (JTBD) | Clayton Christensen, "Competing Against Luck" (2016). Three-job structure (functional, emotional, social) from this work. Also: Tony Ulwick, "Jobs to Be Done: Theory to Practice" |
| Positioning (5 components) | April Dunford, "Obviously Awesome" (2019) |
| Blue Ocean Strategy / Four Actions Framework | W. Chan Kim and Renee Mauborgne, "Blue Ocean Strategy" (Harvard Business Review Press, 2004) |
| Porter's Generic Strategies | Michael Porter, "Competitive Strategy" (1980). Three strategies: cost leadership, differentiation, focus. |
| Porter's Five Forces | Michael Porter, "Competitive Strategy" (1980). Five forces: rivalry, suppliers, buyers, substitutes, new entrants. |
| Crossing the Chasm / Beachhead Strategy | Geoffrey Moore, "Crossing the Chasm" (1991, revised 2014) |
| Pretotyping / XYZ Hypothesis | Alberto Savoia, "The Right It" (2019). Formerly Google's Innovation Agitator. |
| Lean Canvas | Ash Maurya, "Running Lean" (2012). Adapted from Alexander Osterwalder's Business Model Canvas. |
| Value Proposition Canvas | Alexander Osterwalder and Yves Pigneur, "Value Proposition Design" (2014) |
| Mom Test (customer interviews) | Rob Fitzpatrick, "The Mom Test" (2013) |
| Keyword Demand Validation | Ed Sturm, Compact Keywords methodology (2024-2025) |
| SWOT Analysis | Albert Humphrey, Stanford Research Institute (1960s) |
| PESTLE Analysis | Francis Aguilar, "Scanning the Business Environment" (1967). Originally ETPS, expanded to PESTLE. |
| Ansoff Matrix | Igor Ansoff, "Corporate Strategy" (1965). Four growth strategies: market penetration, market development, product development, diversification. |

## Output Standards

1. **File naming**: Save output as `[idea-slug]-[skill-name].md`. Example: `meeting-notes-validation.md`, `freelancer-tools-positioning.md`.
2. **Date format**: Use YYYY-MM-DD (e.g., 2026-03-02).
3. **"Further Reading" links**: Only include if the URL points to an actual published article. Do not link to homepage placeholders.
4. **Metric targets**: When suggesting targets (sign-up rates, conversion benchmarks, etc.), always state the assumption (cold traffic, warm audience, niche community). Benchmarks without context are misleading.

## Skill Footer

Every skill output ends with:

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```
