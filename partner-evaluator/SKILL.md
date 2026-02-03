---
name: partner-evaluator
description: Evaluate potential Being Human partners and advisors. Use when assessing any potential partner, advisor, investor, domain expert, operator, or strategic relationship for BH. Triggers on requests like "evaluate this partner", "assess [name] as an advisor", "should we work with [company]", "score this partnership opportunity", or "run partner evaluation on [name]". Produces comprehensive evaluation with scoring, tier recommendation, equity structure, and milestone schedule.
---

# BH Partner Evaluator

Evaluate any potential partner against Being Human's strategic framework. Produces a scored assessment with actionable recommendations.

## Evaluation Workflow

1. **Gather partner information** - Research and collect context
2. **Determine partner type** - Classify the partnership opportunity
3. **Assess constraint fit** - Map to BH's three core constraints
4. **Score across dimensions** - Apply 5-dimension scoring model
5. **Generate recommendations** - Tier, equity, milestones
6. **Produce evaluation report** - Standardized output format

## Step 1: Gather Partner Information

Before scoring, collect comprehensive context on the partner:

**Required Information:**
- Full name and current role/company
- Professional background (last 10 years)
- Relevant network and relationships
- Previous partnerships or advisory roles
- Any existing relationship with BH team

**Research Methods:**
- LinkedIn profile review
- Web search for recent news/activity
- Company information if applicable
- Any provided documents or context from user

If information is incomplete, note gaps and adjust confidence level in final score.

## Step 2: Determine Partner Type

Classify into one of six categories:

| Type | Indicators |
|------|------------|
| **Strategic Advisor** | Senior exec, board experience, broad network, guidance-focused |
| **Deal & Capital Partner** | Investor, LP, fund manager, deal sourcing background |
| **Domain Expert** | Deep vertical expertise, industry operator, customer connections |
| **Venture Operator** | Execution-focused, GM/CEO experience, team builder |
| **GTM & Distribution Partner** | Channel owner, customer relationships, sales/marketing leader |
| **Brand & Storytelling Partner** | Creative, marketing, content, brand-building background |

Partners may span multiple types. Identify primary and secondary classifications.

## Step 3: Assess Constraint Fit

BH's three core constraints (in priority order):

1. **Capital Access** - Funding, investors, LP relationships
2. **Deal Flow** - Venture opportunities, partnership leads
3. **Distribution/GTM** - Customer access, market channels

For each constraint, assess:
- **Direct fit**: Partner has proven ability to deliver on this constraint
- **Indirect fit**: Partner could contribute but mechanism unclear
- **No fit**: Partner doesn't address this constraint

A partner must directly fit at least one constraint to proceed.

## Step 4: Score Across Dimensions

See [references/scoring-guide.md](references/scoring-guide.md) for detailed criteria.

### Scoring Summary

| Dimension | Weight | Range |
|-----------|--------|-------|
| Constraint Fit | 30% | 0-30 |
| Track Record | 25% | 0-25 |
| Network Quality | 20% | 0-20 |
| Alignment | 15% | 0-15 |
| Availability | 10% | 0-10 |
| **Total** | 100% | 0-100 |

### Quick Scoring Guide

**Constraint Fit (0-30)**
- 25-30: Directly solves primary constraint, proven mechanism
- 18-24: Solves constraint, mechanism less proven
- 10-17: Partial fit, secondary benefit
- 0-9: No clear constraint fit

**Track Record (0-25)**
- 20-25: Documented success, measurable outcomes
- 14-19: Some experience, unclear results
- 7-13: Limited track record
- 0-6: No experience or negative signals

**Network Quality (0-20)**
- 16-20: Deep, relevant relationships
- 11-15: Good network, some gaps
- 6-10: Network relevance unclear
- 0-5: Limited/irrelevant network

**Alignment (0-15)**
- 12-15: Strong cultural fit, long-term oriented
- 8-11: Generally aligned
- 4-7: Some concerns
- 0-3: Significant risks

**Availability (0-10)**
- 8-10: Clear capacity, prioritizes BH
- 5-7: Available with competing commitments
- 2-4: Limited availability
- 0-1: Overcommitted

## Step 5: Generate Recommendations

### Score Interpretation

| Score | Recommendation |
|-------|----------------|
| 85-100 | **Pursue Aggressively** - Offer favorable terms |
| 75-84 | **Strong Candidate** - Standard terms |
| 60-74 | **Qualified** - Proceed with caution |
| 40-59 | **Watchlist** - Revisit later |
| 0-39 | **Pass** - Does not meet threshold |

### Tier Assignment

| Tier | Criteria | Engagement Level |
|------|----------|------------------|
| **Tier 1: Strategic** | Score 85+ AND $1M+ potential | Kyle direct, top equity |
| **Tier 2: Growth** | Score 75-84 AND $250K+ potential | Active management |
| **Tier 3: Network** | Score 60-74 | Light touch |

### Equity Structure

Based on partner type, recommend equity range and structure. See [references/milestone-templates.md](references/milestone-templates.md) for specific milestones by partner type.

**Studio Equity** - For horizontal value across portfolio:
- Strategic Advisors: 0.25% - 2.0%
- Deal & Capital Partners: 0.5% - 1.5%

**Venture Equity** - For vertical value in specific ventures:
- Domain Experts: 0.5% - 15% (advisor vs co-founder)
- Venture Operators: 2% - 15%
- GTM & Distribution: 2% - 20%
- Brand & Storytelling: 0.25% - 3%

## Step 6: Produce Evaluation Report

### Report Template

```markdown
# Partner Evaluation: [Name]

## Summary
| Field | Value |
|-------|-------|
| **Partner** | [Name, Title, Company] |
| **Type** | [Primary type] / [Secondary if applicable] |
| **Evaluation Date** | [Date] |
| **Evaluator** | Claude + [BH team member] |

## Recommendation
**Score: [X]/100** | **Tier: [1/2/3]** | **Action: [Pursue/Qualified/Watchlist/Pass]**

[2-3 sentence summary of recommendation and rationale]

## Constraint Analysis

| Constraint | Fit Level | Evidence |
|------------|-----------|----------|
| Capital Access | [Direct/Indirect/None] | [Brief evidence] |
| Deal Flow | [Direct/Indirect/None] | [Brief evidence] |
| Distribution/GTM | [Direct/Indirect/None] | [Brief evidence] |

## Scoring Breakdown

| Dimension | Score | Notes |
|-----------|-------|-------|
| Constraint Fit | [X]/30 | [Key factors] |
| Track Record | [X]/25 | [Key factors] |
| Network Quality | [X]/20 | [Key factors] |
| Alignment | [X]/15 | [Key factors] |
| Availability | [X]/10 | [Key factors] |
| **TOTAL** | **[X]/100** | |

## Recommended Structure

**Equity Type:** [Studio / Venture: specify which]
**Equity Range:** [X% - Y%]
**Recommended Allocation:** [X%]

### Milestone Schedule

| Tranche | % | Trigger | Target |
|---------|---|---------|--------|
| Cliff | 25% | [Specific milestone] | [+X months] |
| T2 | 25% | [Specific milestone] | [+X months] |
| T3 | 25% | [Specific milestone] | [+X months] |
| T4 | 25% | [Specific milestone] | [+X months] |

**Acceleration Triggers:**
- [Condition] → [Effect]

## Key Strengths
1. [Strength 1]
2. [Strength 2]
3. [Strength 3]

## Risk Factors
1. [Risk 1 + mitigation]
2. [Risk 2 + mitigation]

## Research Notes

### Background
[Professional history, relevant experience]

### Network Analysis
[Key relationships relevant to BH]

### Recent Activity
[Any recent news, deals, or developments]

## Next Steps
1. [Recommended action 1]
2. [Recommended action 2]
3. [Recommended action 3]

---
*Evaluation Confidence: [High/Medium/Low]*
*Information Gaps: [List any missing information]*
```

## Usage Notes

- Always disclose when information is incomplete
- Adjust confidence level based on research depth
- Flag any conflicts of interest discovered
- For borderline scores (within 5 points of threshold), recommend additional diligence
- Update evaluations when new information becomes available
