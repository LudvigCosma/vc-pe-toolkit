---
name: pitch-deck-triage
description: "Triage tool for VC/PE inbound pitch decks. Use when analyzing startup pitch decks to: (1) Extract structured data (team, financials, market, ask), (2) Identify missing information and gaps, (3) Surface questions to ask founders, (4) Find comparable companies via web search, (5) Flag red flags and inconsistencies, (6) Assess founder-market fit and timing thesis. Works standalone or with optional firm-specific context files."
---

# Pitch Deck Triage

Quick triage for inbound pitch decks. Extracts what matters, flags what's missing, surfaces questions to ask, finds comps. No scoring, no opinions—structured analysis that feeds into human decision-making.

**Core philosophy:** VC is a power law business. We're not optimizing for "good companies"—we're hunting for outliers. Every analysis should answer: "What would need to be true for this to return the fund?"

## Workflow

1. Extract PDF content using the PDF skill
2. Parse and structure the data
3. Assess founder-market fit (primary signal at early stage)
4. Extract and interrogate the timing thesis
5. Identify gaps and missing information
6. Generate questions based on gaps and red flags
7. Search web for comparable companies (including failures)
8. Evaluate deal structure and ask
9. Output structured report

## Output Structure

Generate a markdown report that starts with a quick triage summary, followed by deep analysis.

---

### IC Triage Summary

**This section comes first. It should fit in a Slack message and be scannable in 15 seconds.**

Format (copy-paste ready):

```
**[Company Name]** | [Stage] | [Sector] | [Geography]
[One-sentence description of what they do]

Ask: [Amount] at [valuation if stated] → [Primary use of funds]
Team: [Founder names] — [1-line on relevant background]
Timing: [Why now in <10 words]

Thesis fit: ✅ Yes / ⚠️ Maybe / ❌ No — [one-line reason]

Top 2 questions:
1. [Most critical question]
2. [Second most critical question]

**Recommendation:** Proceed to partner meeting / Dig deeper first / Pass
[One sentence on why]
```

**Example output:**

```
**Acme Robotics** | Series A | Industrial Automation | US/Germany
Autonomous mobile robots for warehouse picking, 10x faster than manual.

Ask: $15M at $60M pre → Expand sales team, EU launch
Team: Jane Smith (ex-Amazon Robotics), Bob Lee (PhD MIT, 3 patents)
Timing: Labor costs crossed automation ROI threshold in 2024

Thesis fit: ✅ Yes — Industrial automation, $10M+ ARR, strong technical founders

Top 2 questions:
1. What's the sales cycle and why no named enterprise customers yet?
2. Amazon doing this in-house — what's the moat against them?

**Recommendation:** Proceed to partner meeting
Strong team, right timing, but need to stress-test Amazon risk on the call.
```

---

### Full Analysis

*Everything below is the deep dive. Read before founder calls or partner meetings.*

---

### 1. Executive Summary
The 30-second version:
- **Company**: Name, stage, sector, geography
- **One-liner**: What they do in one sentence
- **Ask**: Amount + use of funds + implied valuation (if stated)
- **Team snapshot**: Founders + key hires (names, titles, relevant background)
- **Timing thesis**: Why now? (one sentence)
- **Fund-returner path**: What would need to be true for 100x? (one sentence)
- **Critical questions**: 3-5 questions that need answers before proceeding

### 2. Founder-Market Fit Assessment

This is PRIMARY analysis at Seed/Series A, not optional. Evaluate:

**Earned Secret**
- What insight do they have from lived experience?
- Is this knowledge hard to acquire without doing the work?
- Have they seen something others haven't?

**Obsession vs Opportunism**
- How long have they been working on this problem?
- Is there evidence of deep domain immersion?
- Would they work on this even if it wasn't fundable?

**Specific Skills Match**
- Does their background map to what this company specifically needs?
- Technical founder for technical product? Sales founder for GTM-heavy model?
- What's the gap between their skills and the job to be done?

**Founder-Market Desperation**
- Do they *have* to solve this? (Personal pain, mission-driven, can't not do it)
- Or is this one of several ideas they could pursue?

**Summary**: Strong fit / Moderate fit / Weak fit / Unclear from deck

### 3. Timing Thesis (Why Now?)

Every great investment has a forcing function. Extract and evaluate:

**Stated timing drivers** (from deck):
- Technology inflection? (AI, mobile, cloud, etc.)
- Regulatory change? (New law, deregulation, compliance requirement)
- Behavioral shift? (Generational, pandemic-driven, cultural)
- Market structure change? (Consolidation, unbundling, platform shift)
- Cost curve crossing? (Something becoming 10x cheaper)

**Timing thesis strength**:
- Is this the right time, or would this have worked 5 years ago?
- Are they early, on time, or late?
- What would kill the timing thesis?

**If timing thesis is missing or weak**: Flag as critical gap.

### 4. Extracted Data
Structured data from the deck:

**Financials** (if present)
- Revenue (current, historical)
- Burn rate / runway
- Growth rate (stated vs calculated—do they match?)
- Unit economics (CAC, LTV, margins, payback period)

**Market**
- TAM / SAM / SOM claims
- Target customer profile
- Geographic focus

**Business Model**
- Pricing model
- Revenue streams
- Key metrics they track

**Traction**
- Customers (count, names if mentioned)
- Partnerships
- Key metrics / milestones

**Team**
- Founders (background, relevant experience)
- Key hires
- Advisory board
- Team size

**The Wedge**
- What's the initial use case that gets them in the door?
- How do they land customers before the full vision is realized?
- Is the wedge compelling enough to drive adoption?

### 5. Deal Structure Analysis

Evaluate whether the ask makes sense:

**The Ask**
- Amount requested
- Use of funds breakdown
- Implied valuation (if stated or calculable)
- Runway this provides

**Sanity Checks**
- Is valuation reasonable for stage and traction?
- Does use of funds match stated strategy?
- Is the runway consistent with their milestone targets?
- How much dilution are they taking? Does that signal confidence or desperation?

**Flag if**: Ask seems disconnected from traction, use of funds doesn't match strategy, or runway doesn't reach stated milestones.

### 6. Gap Analysis
What's missing or unclear:
- **Missing sections**: Unit economics, cap table, GTM timeline, etc.
- **Unstated assumptions**: Where are they making implicit assumptions?
- **Information asymmetry**: What do they know that you don't?
- **Suspiciously absent slides**: No traction slide often = no traction

Format as a bulleted list with brief explanation of why each matters.

### 7. Defensibility Assessment

Interrogate their moat claims:

**Network Effects**
- What type? (Direct, indirect, data, marketplace)
- How strong? (Local or global? Linear or exponential?)
- When do they kick in?

**Data Moats**
- What proprietary data do they generate?
- Why can't it be replicated by a well-funded competitor?
- Does data quality compound over time?

**Scale Economies**
- Unit economics improve at scale?
- Learning curve advantages?
- Fixed cost leverage?

**Switching Costs**
- Technical lock-in? (Integration depth, data migration pain)
- Workflow dependency? (Habit formation, process embedding)
- Contractual? (Multi-year deals, enterprise procurement cycles)

**Regulatory/Legal**
- Licenses, certifications, compliance moats?

**Summary**: Strong moat / Emerging moat / Moat thesis unclear / No moat visible

### 8. Questions to Ask

Prioritized questions based on gaps and red flags. Categorize by topic:

**Founders**
- Background verification, founder-market fit depth, commitment level
- Why are you the right team to solve this?
- What have you learned that others haven't?

**Timing**
- Why now? What changed?
- Why didn't this work 3 years ago? Why will it work now?

**Market**
- TAM validation, competitive dynamics
- Who have you lost deals to? Why?

**Financials**
- Unit economics, path to profitability, assumptions
- Walk me through your burn and runway math

**Product**
- Differentiation, defensibility, roadmap
- What's the wedge? How do you land the first customers?

**Go-to-Market**
- Sales motion, customer acquisition, expansion
- What does a typical sales cycle look like?

### 9. Reference Check Priorities

Based on gaps and red flags, identify the 3 people you'd most want to speak with:

Format:
1. **[Role/Relationship]**: [What you'd want to ask them]

Examples:
- "Their VP Sales from previous company: Can they actually build and scale a sales org?"
- "A churned customer: Why did they leave? What was missing?"
- "A current customer's end user: Is this actually sticky, or just management mandate?"
- "Former co-founder (if applicable): Why did the relationship end?"

### 10. Comparable Companies

Use web search to build a comprehensive comp landscape:

**Direct Competitors** (same problem, same approach)
- Search: `[sector] startups [geography] funding [year]`
- Search: `competitors to [named competitors in deck]`

**Dead Companies** (critical—why did they fail?)
- Search: `[sector] startup failed shutdown [year range]`
- Search: `[company model] startup post-mortem`
- For each: Name, funding raised, why they died, is this team different?

**Adjacent Winners** (parallel race in nearby vertical)
- Search: `[adjacent sector] market leader startup`
- What playbook did they run? Is it applicable here?

**Acqui-hires and Small Exits** (the graveyard)
- Search: `[sector] acquisition acquihire [year range]`
- What does the ceiling look like for mediocre execution?

**Public Company Analogues**
- Search: `[business model] public company`
- Is there a large-cap playbook here? What multiple do they trade at?

For each comp, note:
- Name, stage, funding raised, outcome (if known)
- Key similarity to this company
- Key difference
- What can we learn?

### 11. Red Flags & Inconsistencies
Things that warrant attention:

**Math Errors**
- Growth rates that don't add up
- Burn vs runway inconsistencies
- Revenue projections that contradict stated assumptions
- Stated growth vs calculated growth (from their own numbers)

**Narrative Gaps**
- Founder story doesn't match the business
- Experience gaps for the domain
- Team composition vs. stage mismatch
- The wedge isn't clear or compelling

**Deck Forensics**
- Who made this deck? (Professional design vs founder-made tells you about priorities)
- What's the slide order? (Burying financials = hiding something?)
- What slides are suspiciously missing?
- Is this version 1 or version 50? (Iteration suggests feedback)
- Polished deck with inconsistent metrics = carelessness or deception
- Rough deck but internally consistent = rigorous founder

**Timing Red Flags**
- "Why now" answer is weak or generic
- Market timing feels early or late
- No clear forcing function

### 12. Power Law Assessment

**The Fund-Returner Question**

What would need to be true for this to return the fund (100x)?

- Market size sufficient? (Need $1B+ outcome potential)
- Team capable of scaling to that level?
- Timing right for exponential growth?
- Defensibility that compounds?

**Risk-Adjusted Thinking**

A minor red flag on a 10x opportunity? Pass.
The same red flag on a potential 100x? Worth the risk.

Classify this opportunity:
- **Potential fund-returner**: High ceiling, worth significant diligence
- **Solid 3-5x potential**: Good company, but not outlier trajectory
- **Unclear ceiling**: Need more information to assess
- **Capped outcome**: Structural limits on upside

## Dig Deeper Prompts

After initial output, users can request:
- "Deep dive on founder-market fit" → Extended background research on founders
- "Interrogate the timing thesis" → Search for market timing evidence
- "Run GTM reality check" → Validate sales assumptions against team/market
- "Validate TAM assumptions" → Break down market sizing claims with external data
- "Check financial consistency" → Verify all math across stated metrics
- "Find more comps in [sector/geo]" → Expanded comparable search
- "Search for failed companies in this space" → Graveyard analysis
- "Analyze the wedge strategy" → Evaluate initial go-to-market approach

## Firm Context (Recommended)

For better analysis, users should add these files to the skill folder:

- `investment-thesis.md` — Firm's focus areas, stage preferences, geography, check size. **Required for thesis alignment scoring.**
- `portfolio-companies.md` — Past investments with basic data. Enables portfolio overlap and conflict checks.
- `evaluation-criteria.md` — Firm-specific red flags, must-haves, or weighted criteria.

If `investment-thesis.md` is present, add a section:

### Thesis Alignment
- **In strike zone**: Yes / No / Partial
- **Alignment factors**: What matches
- **Misalignment factors**: What doesn't match
- **Recommendation**: Proceed to partner meeting / Need more info / Pass

Example prompt to user:
> "For thesis alignment analysis, add `investment-thesis.md` to the skill folder with your firm's focus areas and check size."

## Stage-Specific Calibration

Auto-detect stage from deck content (round mentioned, revenue, team size). Apply appropriate expectations:

**Pre-seed / Seed**
- Product may not exist yet — focus on team and vision
- No revenue expected — look for early signals (waitlist, LOIs, pilots)
- Missing unit economics is normal
- **Primary signal**: Founder-market fit
- **Key question**: Do these founders have an earned secret?

**Series A**
- Expect product-market fit signals
- Some revenue/traction expected
- Unit economics should be emerging
- No CFO is normal, but finance narrative matters
- **Primary signal**: Evidence of PMF (retention, expansion, pull)
- **Key question**: Is this repeatable?

**Series B+**
- Clear unit economics required
- Strong revenue and growth metrics
- Team should be scaling (key hires beyond founders)
- Missing finance function is a yellow flag
- **Primary signal**: Scalable economics and growth
- **Key question**: Can this be a market leader?

## Red Flag Patterns

Common patterns to flag (as questions, not conclusions):

**Team**
- First-time founder in deep tech / regulated industry
- Solo founder at growth stage
- No technical co-founder for tech product
- Founder experience doesn't match domain
- Founding team changed significantly (why?)

**Market**
- TAM is total market, not serviceable
- "No direct competitors" claim (almost always false or bad sign)
- Market timing unclear or unconvincing
- The "why now" is generic (e.g., "AI is growing")

**Financials**
- Hockey stick with no explanation
- Burn rate inconsistent with team size
- Revenue per customer varies wildly
- Growth assumptions exceed historical without explanation
- Stated metrics don't match calculated metrics

**GTM**
- Enterprise sales with tiny team
- Consumer app with unrealistic conversion
- No clear channel strategy
- The wedge isn't compelling or differentiated

**Deal**
- Valuation disconnected from traction
- Use of funds doesn't match strategy
- Raising too little (won't hit milestones) or too much (why?)

## Technical Notes

- Use PDF skill for extraction
- Use web search for comparable companies (including failure searches)
- Stage auto-detected from deck content (can be overridden by user)
- Works standalone, but thesis alignment requires `investment-thesis.md`
- Always search for dead companies in the space—the graveyard tells you more than the survivors
