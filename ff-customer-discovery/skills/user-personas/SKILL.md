---
name: user-personas
description: "Create 2-3 data-driven personas from real research. JTBD-based, not demographic fiction. Clearly marks unvalidated hypothesis personas when data is missing. Triggers: user personas, create persona, customer persona, who is my user, user profiles."
---

# User Personas

Build personas that drive product decisions - not pretty posters that hang on a wall and do nothing.

## Context

You are helping a vibecoder create user personas for: **$ARGUMENTS**.

If running in sequence from /discover-customers, use data from previous steps: target audience segments, interview summaries, competitor insights, and demand signals. Carry all of it forward.

## Why This Matters

Traditional personas are demographic fiction. "Sarah, 28, lives in Brooklyn, drinks oat milk, works at a startup." That tells you nothing about what to build or how to market it.

Good personas are built on JTBD - Jobs to Be Done (Clayton Christensen, "Competing Against Luck", 2016). They describe what people are trying to ACCOMPLISH, not what they look like. A 25-year-old freelancer and a 55-year-old consultant can have the exact same JTBD. If you build for the job, you serve both.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Assess Available Data

Ask what data the founder has:
- Interview transcripts or summaries (from summarize-interview or their own notes)
- Analytics data (sign-ups, usage patterns, feature adoption)
- Survey responses
- Reddit/forum posts about the problem
- Support tickets or user feedback
- App store reviews (theirs or competitors')

**Critical distinction**: The quality of personas depends entirely on the quality of input data.

### Step 2: Choose Your Track

**Track A: Data-Driven Personas** (when real data exists)

If the founder has interview data, analytics, or meaningful user feedback, proceed to Step 3.

**Track B: Hypothesis Personas** (when no data exists)

If the founder has NO real user data, flag this clearly:

```
IMPORTANT: These personas are HYPOTHESES, not research findings.

You don't have real user data yet, so these personas are educated guesses
based on market research and competitor analysis. They are useful for
planning, but they MUST be validated through customer interviews before
you make product decisions based on them.

Recommended next step: Use the customer-interview-script skill to
prepare for 8-12 interviews, then rebuild these personas with real data.
```

Proceed to Step 3, but mark every persona as **UNVALIDATED** in the output.

### Step 3: Identify Distinct Segments by JTBD

Group users NOT by demographics, but by what they're trying to accomplish. Two users with the same job title but different JTBD are different personas. Two users with different demographics but the same JTBD are the SAME persona.

Look for patterns across the data:
- What are the 2-3 distinct jobs people are hiring this product to do?
- Are there users who use the product for fundamentally different purposes?
- Do some users care about speed while others care about depth?
- Are there power users vs occasional users with different needs?

Aim for 2-3 personas. More than 4 is too many - you can't build for everyone at once.

### Step 4: Build Persona Cards

For each persona:

```markdown
## Persona [number]: [Name] - "[one-sentence JTBD summary]"

**Status**: [DATA-DRIVEN / UNVALIDATED HYPOTHESIS]

### Who They Are
[2-3 sentences describing this person in terms relevant to their JTBD. Include role/context, not just demographics.]

### Primary Job to Be Done
(Clayton Christensen, "Competing Against Luck", 2016)

- **Functional**: [What they're trying to accomplish - the practical task]
- **Emotional**: [How they want to feel - confident, in control, less stressed, creative]
- **Social**: [How they want to be perceived - professional, innovative, reliable, smart]

### Top 3 Pain Points
Ranked by severity:

1. **[Pain point]** - Severity: [HIGH/MEDIUM/LOW]
   Evidence: [quote from interview, data point, or "hypothesis - needs validation"]

2. **[Pain point]** - Severity: [HIGH/MEDIUM/LOW]
   Evidence: [quote from interview, data point, or "hypothesis - needs validation"]

3. **[Pain point]** - Severity: [HIGH/MEDIUM/LOW]
   Evidence: [quote from interview, data point, or "hypothesis - needs validation"]

### Current Solution
[What they use today and why. Include what works and what's broken.]

### One Unexpected Insight
[Something surprising that emerged from the data - a need, behaviour, or preference the founder didn't anticipate. If hypothesis-based, note: "To discover: validate in interviews."]

### Product Fit Assessment
- **How your app serves them**: [what features/aspects of your product map to their JTBD]
- **Where it falls short**: [gaps between their needs and your product - be honest]
- **Feature priority for this persona**: [top 3 features or improvements that would make them a loyal user]
```

### Step 5: Rank Personas

Create a ranking table:

```
| Persona | Pain Intensity | Willingness to Pay | Reachability | Recommendation |
|---|---|---|---|---|
| [Persona 1] | HIGH/MED/LOW | HIGH/MED/LOW | HIGH/MED/LOW | PRIMARY / SECONDARY / DEPRIORITISE |
| [Persona 2] | HIGH/MED/LOW | HIGH/MED/LOW | HIGH/MED/LOW | PRIMARY / SECONDARY / DEPRIORITISE |
| [Persona 3] | HIGH/MED/LOW | HIGH/MED/LOW | HIGH/MED/LOW | PRIMARY / SECONDARY / DEPRIORITISE |
```

Scoring rules from CONVENTIONS.md apply: prioritise factors the founder can verify with evidence (willingness to pay, pain intensity) over factors based on inference.

### Step 6: Recommend Primary Persona

Choose ONE persona as the primary build target. State:

1. **Who**: persona name and JTBD
2. **Why them first**: specific rationale tied to ranking criteria
3. **What this means**: implications for features, positioning, messaging
4. **Validation status**: whether this persona is data-driven or hypothesis-based
5. **Next step**: if hypothesis-based, recommend customer-interview-script. If data-driven, recommend positioning (ff-positioning plugin) or demand validation.

## Output

Save as `[product-slug]-personas.md`. The report should include:

1. Data quality assessment (what data was available, what was missing)
2. 2-3 persona cards with full JTBD analysis
3. Ranking table
4. Primary persona recommendation
5. Clear labelling of DATA-DRIVEN vs UNVALIDATED HYPOTHESIS throughout

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

## Common Mistakes

- **Building personas from imagination.** "I think our user is a 25-year-old developer" is not a persona - it's a guess. Label it as such.
- **Too many personas.** Three is the maximum for a solo founder. You can't build for 7 different people at once. Pick the best beachhead.
- **Demographic-first thinking.** Age, gender, and location rarely determine product behaviour. JTBD determines product behaviour. Build personas around jobs, not demographics.
- **Treating hypothesis personas as fact.** If you haven't talked to real users, your personas are fiction. Useful fiction for planning, but fiction. Validate before you bet the product on them.
- **Never updating personas.** Personas are living documents. After every batch of interviews, update them. After launch, update them with real usage data.

## Notes

- Creating personas takes 10-15 minutes with data, 15-20 minutes without (because more inference is needed)
- Hypothesis personas should be treated as "version 0.1" - expect to rewrite them after interviews
- When running as part of /discover-customers, these are always hypothesis personas (interviews haven't happened yet) and should be marked accordingly
- Pair with customer-interview-script to validate hypothesis personas and with summarize-interview to rebuild them from real data

**Framework attribution**: JTBD-based persona development from Clayton Christensen, "Competing Against Luck" (2016). Three-job structure (functional, emotional, social) from Christensen's work. Also: Tony Ulwick, "Jobs to Be Done: Theory to Practice". See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [Why Most Personas Are Useless (And How to Build Ones That Aren't)](https://fantasticfounder.com) - JTBD-based persona development that drives actual product decisions
