# Partner Pipeline Tracking Spreadsheet
## Template for Being Human Team Collaboration

**Purpose:** Track, score, and rank all potential partners in one centralized location
**Tool:** Import into Google Sheets or Coda for team collaboration
**Owners:** Kyle (final decisions), Steve/Ram/Jaden (research and scoring)

---

## Instructions for Use

### Setup (One-Time)

1. **Create Google Sheet** - Copy structure below into new Google Sheet
2. **Share with Team** - Give edit access to Kyle, Steve, Ram, Jaden
3. **Set up Filters** - Enable filter views for sorting/filtering
4. **Create Views** - Set up different views for different workflows

### Workflow

**Adding New Partner:**
1. Team member adds row with basic info (Name, Source, Date Added)
2. Assign Primary Evaluator
3. Evaluator completes research and scoring (30-60 min)
4. Status → "Scored"
5. Team discusses in Monday sync if score 75+
6. Kyle makes final decision
7. Update Status and Action fields

**Regular Reviews:**
- **Weekly:** Update partner outreach status
- **Bi-weekly:** Discuss high-priority partners (85+ score)
- **Monthly:** Review pipeline health, reallocate budget

---

## Spreadsheet Structure

### Tab 1: Active Pipeline

| Column | Type | Purpose |
|--------|------|---------|
| ID | Auto | Unique identifier (auto-increment) |
| Name | Text | Partner name |
| Company | Text | Current company/affiliation |
| Partner Type | Dropdown | Strategic Advisor, Deal & Capital, Domain Expert, GTM, Brand, Operator |
| Primary Constraint | Dropdown | Capital Access, Deal Flow, Distribution/GTM |
| Source | Text | How they came to BH (referral, inbound, outbound) |
| Date Added | Date | When added to pipeline |
| Primary Evaluator | Dropdown | Kyle, Steve, Ram, Jaden |
| Status | Dropdown | New, Researching, Scored, Discussing, Approved, Declined, Deferred |
| --- SCORING --- | | |
| Constraint Fit | Number (0-30) | How well they solve BH constraints |
| Track Record | Number (0-25) | Past success in similar partnerships |
| Network Quality | Number (0-20) | Relevance and depth of relationships |
| Uniqueness | Number (0-15) | How unique vs. existing partners |
| Availability | Number (0-10) | Capacity to contribute |
| **TOTAL SCORE** | Formula | =SUM(Constraint:Availability) |
| **TIER** | Formula | =IF(Total>=85,"Tier 1",IF(Total>=75,"Tier 2",IF(Total>=60,"Tier 3","Pass"))) |
| --- PORTFOLIO FIT --- | | |
| Similar Partners | Text | Existing partners with overlap |
| Overlap % | Number (0-100) | Estimated network overlap with existing |
| Priority | Dropdown | High, Medium, Low (based on constraint + budget) |
| Budget Type | Dropdown | Strategic Advisor (4-6%), Deal & Capital (3-5%), Domain Expert (2-3%), GTM (3-4%), Brand (1-2%) |
| Budget Remaining | Number | % remaining in this budget category |
| --- RECOMMENDATION --- | | |
| Action | Dropdown | Pursue Aggressively, Pursue, Defer, Pass |
| Proposed Equity | Number (0-5%) | Recommended equity allocation |
| Equity Type | Dropdown | Studio, Venture (specify), Revenue Share, Cash Only |
| Rationale | Long text | 2-3 sentences explaining recommendation |
| Key Strengths | Long text | Top 3 strengths (bullets) |
| Risk Factors | Long text | Top 2 risks (bullets) |
| --- TRACKING --- | | |
| Last Contact | Date | When we last reached out or met |
| Next Step | Text | What's the next action |
| Next Step Owner | Dropdown | Who owns the next step |
| Next Step Due | Date | When next step should be completed |
| Notes | Long text | Running notes on conversations, progress |
| Evaluation Doc | URL | Link to full evaluation document (if created) |

---

## Tab 2: Cap Table Budget

Track overall equity allocation strategy:

| Partner Type | Target # | Target % | Allocated % | Remaining % | Status |
|--------------|----------|----------|-------------|-------------|--------|
| Strategic Advisors | 4-6 | 4-6% | [auto-sum from Tab 1] | [calc] | [Red/Yellow/Green] |
| Deal & Capital Partners | 3-5 | 3-5% | [auto-sum] | [calc] | [Red/Yellow/Green] |
| Domain Experts | 2-3 | 2-3% | [auto-sum] | [calc] | [Red/Yellow/Green] |
| GTM & Distribution | 2-3 | 3-4% | [auto-sum] | [calc] | [Red/Yellow/Green] |
| Brand & Storytelling | 1-2 | 1-2% | [auto-sum] | [calc] | [Red/Yellow/Green] |
| **TOTAL GROWTH POOL** | **15-20** | **15-20%** | **[auto-sum]** | **[calc]** | **[status]** |
| Reserve | - | 2-3% | 0% | 2-3% | Green |
| **GRAND TOTAL** | | **17-23%** | | | |

**Status Indicators:**
- 🟢 Green: Under budget, capacity to add more
- 🟡 Yellow: Approaching budget, be selective
- 🔴 Red: Over budget, need to deprioritize or decline

---

## Tab 3: Approved Partners

Track partners we've committed to (for reference and overlap checking):

| Name | Partner Type | Equity % | Equity Type | Date Approved | Vesting End | Status | Key Networks | Milestones |
|------|--------------|----------|-------------|---------------|-------------|--------|--------------|------------|
| [Partner Name] | [Type] | [%] | [Studio/Venture] | [Date] | [Date] | [Active/Complete] | [Networks] | [Link to agreement] |

---

## Tab 4: Declined/Deferred

Track partners we decided not to pursue (with rationale for future reference):

| Name | Partner Type | Score | Date Declined | Reason | Would Reconsider If... |
|------|--------------|-------|---------------|--------|----------------------|
| [Name] | [Type] | [Score] | [Date] | [Why we passed] | [What would change our mind] |

---

## Sample Data (Example Rows)

### Tab 1: Active Pipeline (Example)

| ID | Name | Company | Partner Type | Constraint | Source | Date Added | Evaluator | Status | C.Fit | Track | Network | Unique | Avail | TOTAL | TIER | Action | Proposed Equity |
|----|------|---------|--------------|-----------|--------|------------|-----------|--------|-------|-------|---------|--------|-------|-------|------|--------|----------------|
| 1 | Jocelyn Little | Beach House Pictures | Strategic Advisor | Distribution + Deal Flow | Inbound | 2026-01-15 | Kyle | Scored | 23 | 20 | 16 | 8 | 7 | 74 | Tier 3 | Pursue (Modified) | 0.4% studio |
| 2 | Donovan Chan | Beach House Pictures | Brand & Storytelling | Distribution | Inbound | 2026-01-15 | Kyle | Scored | 21 | 21 | 14 | 6 | 7 | 69 | Tier 3 | Defer | 0% studio, 1% WonderCast |
| 3 | Beach House Pictures | Fremantle | GTM & Distribution | Distribution | Inbound | 2026-01-15 | Kyle | Scored | 24 | 22 | 17 | 12 | 7 | 82 | Tier 2 | Pursue | 2.5% studio (services) |
| 4 | Gay Chee Cheong | Individual | Deal & Capital | Capital Access | Referral | 2025-12-01 | Kyle | Approved | 25 | 18 | 15 | 10 | 8 | 76 | Tier 2 | Approved | 0.5-1.0% (pending) |
| 5 | [Hypothetical Tech Advisor] | [AI Startup] | Strategic Advisor | Capital + Deal Flow | Outbound | 2026-02-01 | Steve | Researching | - | - | - | - | - | - | - | TBD | TBD |

---

## Formulas for Google Sheets

### TOTAL SCORE (Column N)
```
=SUM(J2:N2)
```
Where J=Constraint Fit, K=Track Record, L=Network Quality, M=Uniqueness, N=Availability

### TIER (Column O)
```
=IF(N2>=85,"Tier 1",IF(N2>=75,"Tier 2",IF(N2>=60,"Tier 3","Pass")))
```

### Budget Remaining (Tab 2)
```
=MAX(0, [Target %] - [Allocated %])
```

### Status Indicator (Tab 2)
```
=IF([Allocated %]>[Target %],"🔴 Over Budget",IF([Allocated %]>([Target %]*0.8),"🟡 Approaching Limit","🟢 Capacity Available"))
```

---

## Filter Views (Pre-Configured)

### View 1: "High Priority (85+ Score)"
- Filter: Score >= 85
- Sort: Score DESC
- Purpose: Focus on top-tier opportunities

### View 2: "Needs Decision (Scored, Not Approved)"
- Filter: Status = "Scored" OR "Discussing"
- Sort: Score DESC
- Purpose: Partners awaiting team decision

### View 3: "By Partner Type"
- Group by: Partner Type
- Sort: Type, then Score DESC
- Purpose: See distribution across types

### View 4: "Capital Access Priority"
- Filter: Primary Constraint = "Capital Access"
- Sort: Score DESC
- Purpose: Focus on solving #1 constraint

### View 5: "This Month's Additions"
- Filter: Date Added >= [First day of current month]
- Sort: Date Added DESC
- Purpose: Track new inbound

---

## Automated Workflows (Optional - Zapier/Make)

**Workflow 1: New Partner Added**
- Trigger: New row added to Tab 1
- Action: Send Slack message to #partners channel
- Content: "[Name] added to pipeline by [Source]. Assigned to [Evaluator]."

**Workflow 2: High Score Achieved**
- Trigger: Total Score >= 85 (calculated field changes)
- Action: Send Slack message to Kyle + team
- Content: "🎯 High priority partner: [Name] scored [Score]. Review ASAP."

**Workflow 3: Budget Warning**
- Trigger: Allocated % exceeds 80% of Target % (Tab 2)
- Action: Send Slack warning to Kyle
- Content: "⚠️ [Partner Type] budget at 80%. Remaining: [X]%."

**Workflow 4: Stale Pipeline**
- Trigger: Status = "Researching" for >7 days OR "Discussing" for >14 days
- Action: Send reminder to assigned evaluator
- Content: "[Name] has been in [Status] for [X] days. Next step?"

---

## How to Import This Template

### Option 1: Google Sheets

1. Create new Google Sheet
2. Copy column headers from "Spreadsheet Structure" above
3. Set up formulas for calculated fields (Total Score, Tier)
4. Configure dropdowns:
   - Partner Type: Strategic Advisor, Deal & Capital Partner, Domain Expert, Venture Operator, GTM & Distribution, Brand & Storytelling
   - Primary Constraint: Capital Access, Deal Flow, Distribution/GTM
   - Status: New, Researching, Scored, Discussing, Approved, Declined, Deferred
   - Action: Pursue Aggressively, Pursue, Defer, Pass
   - Priority: High, Medium, Low
5. Share with team (edit access)

### Option 2: Coda

1. Create new Coda doc
2. Add table with columns above
3. Use Coda's calculation and filtering features
4. Embed in BH's main Coda workspace

### Option 3: Airtable

1. Create new Airtable base
2. Import CSV with column structure
3. Configure field types (dropdowns, formulas, dates)
4. Set up views (filters, sorts, groupings)
5. Invite team members

---

## Dashboard Metrics (Add to Tab 1 Summary)

Track pipeline health with these KPIs:

| Metric | Formula | Target | Current | Status |
|--------|---------|--------|---------|--------|
| **Total Partners in Pipeline** | COUNT(Status != "Approved" AND != "Declined") | 15-25 | [auto] | [indicator] |
| **Avg Score (Active Pipeline)** | AVERAGE(Score WHERE Status = Active) | 70+ | [auto] | [indicator] |
| **% High Priority (85+)** | COUNT(Score>=85) / COUNT(All) | 20-30% | [auto] | [indicator] |
| **% Approved & Pending** | COUNT(Status="Approved") / COUNT(All) | 10-20% | [auto] | [indicator] |
| **Total Equity Allocated** | SUM(Approved Partners Equity %) | <20% | [auto] | [indicator] |
| **Strategic Advisors (Approved)** | COUNT(Type="Strategic Advisor" AND Status="Approved") | 4-6 | [auto] | [indicator] |
| **Capital Partners (Approved)** | COUNT(Type="Deal & Capital" AND Status="Approved") | 3-5 | [auto] | [indicator] |
| **Days Since Last Addition** | TODAY() - MAX(Date Added) | <7 days | [auto] | [indicator] |

---

## Meeting Agenda Template (Monday Partner Sync)

Use spreadsheet as source of truth for weekly partner discussions:

**15-Minute Partner Review (Weekly)**

1. **New Additions (2 min)**
   - Review partners added this week
   - Assign evaluators
   - Set research deadlines

2. **High Priority (5 min)**
   - Discuss any partners scoring 85+
   - Make pursue/defer decisions
   - Assign next steps

3. **Pending Decisions (5 min)**
   - Review partners in "Scored" or "Discussing" status
   - Make approve/decline/defer decisions
   - Update budget tracking

4. **Pipeline Health (3 min)**
   - Review dashboard metrics
   - Identify gaps (e.g., need more capital partners)
   - Outreach planning for next week

---

## Sample Export (CSV Format)

```csv
ID,Name,Company,Partner Type,Primary Constraint,Source,Date Added,Primary Evaluator,Status,Constraint Fit,Track Record,Network Quality,Uniqueness,Availability,TOTAL,TIER,Action,Proposed Equity,Equity Type
1,Jocelyn Little,Beach House Pictures,Strategic Advisor,Distribution + Deal Flow,Inbound,2026-01-15,Kyle,Scored,23,20,16,8,7,74,Tier 3,Pursue (Modified),0.4%,Studio
2,Donovan Chan,Beach House Pictures,Brand & Storytelling,Distribution,Inbound,2026-01-15,Kyle,Scored,21,21,14,6,7,69,Tier 3,Defer,0%,Studio
3,Beach House Pictures,Fremantle,GTM & Distribution,Distribution,Inbound,2026-01-15,Kyle,Scored,24,22,17,12,7,82,Tier 2,Pursue,2.5%,Studio (services)
4,Gay Chee Cheong,Individual,Deal & Capital,Capital Access,Referral,2025-12-01,Kyle,Approved,25,18,15,10,8,76,Tier 2,Approved,0.5-1.0%,Studio (pending)
```

---

## Quick Actions Checklist

**When evaluating a new partner:**
- [ ] Add row to spreadsheet with basic info
- [ ] Assign primary evaluator
- [ ] Complete research (30-60 min)
- [ ] Score on 5 dimensions
- [ ] Check for overlap with existing partners
- [ ] Verify budget available in their category
- [ ] Make pursue/defer recommendation
- [ ] Share with team for input
- [ ] Discuss in Monday sync if 75+
- [ ] Kyle makes final decision
- [ ] Update Status and Action
- [ ] Schedule next step if pursuing

**When approving a partner:**
- [ ] Move to "Approved Partners" tab
- [ ] Update budget allocation (Tab 2)
- [ ] Create evaluation document (full write-up)
- [ ] Draft term sheet or agreement
- [ ] Assign owner for partnership management
- [ ] Set milestone schedule
- [ ] Add to BH partner communications

---

This spreadsheet becomes the single source of truth for BH's partner pipeline, enabling the team to collaborate efficiently and make data-driven decisions about equity allocation.

**Setup Time:** 30-45 minutes to configure in Google Sheets/Coda
**Maintenance:** 15 minutes weekly (update during Monday sync)
**Value:** Clear visibility into partner pipeline, consistent evaluation, strategic cap table management

---

**Prepared by:** Claude + Kyle Jackson
**Date:** February 1, 2026
**Status:** Template Ready for Implementation
