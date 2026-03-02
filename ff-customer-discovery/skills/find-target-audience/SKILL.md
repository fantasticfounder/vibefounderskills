---
name: find-target-audience
description: "Identify who your app is REALLY for - not who you assumed. Scores audience segments on pain, willingness to pay, reachability, market size, and founder-market fit to find your best beachhead. Triggers: find target audience, who is my app for, target market, target customer, ideal customer, who should I sell to."
---

# Find Your Target Audience

Figure out who your app is actually for - because "everyone" is not a target audience.

## Context

You are helping a vibecoder identify the right target audience for their product: **$ARGUMENTS**.

If the user provides data (analytics, user feedback, sign-up info, existing research), use it first. Use web search to supplement, not replace, what the founder already knows.

## Why This Matters

Most vibecoders build for themselves, then assume everyone else thinks the same way. They launch to "anyone who needs a [product type]" and get zero traction. The fix is simple but uncomfortable: pick ONE audience, understand them deeply, and build specifically for them.

This is beachhead thinking - a concept from Geoffrey Moore's "Crossing the Chasm" (1991, revised 2014). You don't win the whole market at once. You win one small segment completely, then expand from there.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

Work through these steps with the user. Be direct. If their assumed audience doesn't match the evidence, say so.

### Step 1: Gather What the Founder Knows

Ask:
- What does your app do? (one sentence)
- Who did you BUILD it for? (who you had in mind when you started)
- Who is ACTUALLY using it? (if launched - check analytics, sign-ups, feedback)
- Do you have any data? (analytics, user emails, support tickets, Reddit comments, reviews)
- What assumptions are you making about your audience?

If the founder hasn't launched yet, focus on who they built it for and what problem it solves. If they have launched, the data about actual users matters more than their original assumptions.

### Step 2: Map the Audience Landscape

Identify 5-8 potential audience segments. For each one, consider four questions:

1. **Who has the pain?** - Who experiences this problem regularly enough to want a solution?
2. **Who already searches for solutions?** - Use web search: `"[product type] for [audience]" site:reddit.com`, `"[product type] alternatives"`, `"[problem] tool"`. Check who's asking.
3. **Who has budget?** - Not everyone with the problem can or will pay. Filter for people who spend money on tools in this space.
4. **Who can the founder reach?** - A perfect audience you can't access is useless. Consider: are they on Reddit? Twitter/X? Do they read specific newsletters? Are they in Discord servers?

Use web search to validate these segments. Search for `"[product type] users Reddit"`, `"[product type] who uses this"`, `"[product type] reviews"` to find real people discussing real needs.

Present segments as a simple list:
```
Segment 1: [Name] - [one-line description]
Segment 2: [Name] - [one-line description]
...
```

### Step 3: Score Segments

Score each segment on 5 criteria, 1-5 scale:

| Criteria | 1 (Low) | 3 (Medium) | 5 (High) |
|---|---|---|---|
| **Pain intensity** | Nice-to-have, mild annoyance | Real problem, seeks solutions occasionally | Hair-on-fire problem, actively spending time/money to solve |
| **Willingness to pay** | Expects free, no budget history | Pays for some tools, price-sensitive | Already paying for inferior alternatives |
| **Reachability** | No obvious channels, scattered | Present in some communities, some channels | Concentrated in specific communities the founder can access |
| **Market size** | Tiny niche, fewer than 1K potential users | Mid-size niche, 10K-100K potential users | Large addressable market, 100K+ potential users |
| **Founder-market fit** | Founder has no connection to this audience | Founder understands the space somewhat | Founder IS this audience or has deep expertise |

**Scoring rules from CONVENTIONS.md apply:** Score honestly. If evidence is missing, score low. For any score of 4 or 5, state the specific evidence. For any score of 1 or 2, state what's missing.

Present as a table:

```
| Segment | Pain (1-5) | WTP (1-5) | Reach (1-5) | Size (1-5) | Fit (1-5) | Total (/25) |
|---|---|---|---|---|---|---|
| [Segment 1] | X | X | X | X | X | XX |
| [Segment 2] | X | X | X | X | X | XX |
| ... | ... | ... | ... | ... | ... | ... |
```

When scores tie, apply the tiebreaker from CONVENTIONS.md: prioritise factors the founder can verify with evidence (willingness to pay, pain intensity) over factors based on inference (market size, founder-market fit).

### Step 4: Build Mini-ICPs for Top Segments

For the top 2-3 scoring segments, build a mini Ideal Customer Profile:

```
### [Segment Name] - Score: X/25

**Demographics**: [age range, role, company size if B2B, relevant context]

**Jobs to Be Done** (Clayton Christensen, "Competing Against Luck", 2016):
- Functional: [what they're trying to accomplish]
- Emotional: [how they want to feel]
- Social: [how they want to be perceived]

**Current solution**: [what they use today - could be a competitor, spreadsheet, manual process, or nothing]

**What's broken about it**: [why the current solution falls short]

**Switching trigger**: [what event or frustration would make them try something new]

**Where to find them**: [specific subreddits, communities, newsletters, Twitter accounts, conferences]
```

### Step 5: Recommend ONE Primary Target

Choose one segment as the primary target. State:

1. **Who**: the segment name and description
2. **Why this one**: specific rationale tied to the scores
3. **What this means for the product**: any implications for features, messaging, or positioning
4. **What to do next**: validate this choice with customer interviews (use the customer-interview-script skill)

Be honest. If the founder's assumed audience scored lower than another segment, say so directly. Data beats assumptions.

## Output

Save the full report as `[product-slug]-target-audience.md`. The report should include:

1. Product summary (one sentence)
2. Audience segment list (5-8 segments)
3. Scoring table with rationale
4. Mini-ICPs for top 2-3 segments
5. Primary target recommendation with rationale
6. "Where to find them" section with specific channels
7. Suggested next steps

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

## Common Mistakes

- **"My app is for everyone."** No it isn't. The more specific your target, the faster you grow. Instagram started with photographers. Facebook started with Harvard students. Slack started with game developers.
- **Scoring based on hope instead of evidence.** If you don't KNOW they have the pain, score it low. "I think they'd pay" is not evidence of willingness to pay.
- **Picking the biggest market instead of the best beachhead.** A huge market you can't reach is worse than a tiny niche where you know everyone.
- **Ignoring who's actually using your app.** If your analytics show teachers signing up but you built it for developers, pay attention to the teachers.

## Notes

- This analysis takes 15-30 minutes depending on how much data exists
- If running as part of the /discover-customers command, carry the primary target and mini-ICP forward into subsequent skills
- The strongest signal is when actual usage data contradicts the founder's assumptions - that's where the real opportunity usually lives

**Framework attribution**: Beachhead strategy from Geoffrey Moore, "Crossing the Chasm" (1991, revised 2014). JTBD framework from Clayton Christensen, "Competing Against Luck" (2016). Three-job structure (functional, emotional, social) from Christensen's work. Also: Tony Ulwick, "Jobs to Be Done: Theory to Practice". See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [How to Find Your Target Audience When You've Already Built Something](https://fantasticfounder.com) - Finding your first 10 customers when you built the product before finding the audience
