# Beach House Pictures - Deal Calculator
## Dynamic Formula Reference for Negotiations

**Purpose:** Calculate equity allocations based on variable service values and valuations
**Date:** February 1, 2026

---

## Core Formulas

### Formula 1: Net Service Value Differential

```
Net_Differential = BHP_Service_Value - BH_Service_Value
```

**Where:**
- `BHP_Service_Value` = Dollar value of Beach House storytelling services
- `BH_Service_Value` = Dollar value of Being Human AI consultation services

**Example:**
- BHP Services: $150,000
- BH Services: $50,000
- **Net Differential: $100,000**

---

### Formula 2: Corporate Equity Allocation (Service Swap)

```
BHP_Corporate_Equity_% = (Net_Differential / BH_Valuation_Cap) × 100
```

**Where:**
- `Net_Differential` = From Formula 1
- `BH_Valuation_Cap` = Being Human valuation cap (from SAFE terms)

**Example:**
- Net Differential: $100,000
- BH Valuation: $12,000,000
- **BHP Corporate Equity: 0.83%**

---

### Formula 3: Total Studio Dilution

```
Total_Studio_Dilution_% = BHP_Corporate_% + Jocelyn_Personal_% + Donovan_Personal_%
```

**Example:**
- BHP Corporate: 0.83%
- Jocelyn Personal: 0.75%
- Donovan Personal: 0.5%
- **Total Studio Dilution: 2.08%**

---

### Formula 4: Remaining Growth Pool Capacity

```
Remaining_Growth_Pool_% = Growth_Pool_Budget_% - Total_Allocated_%
```

**Where:**
- `Growth_Pool_Budget_%` = 15-20% (BH's total partner allocation budget)
- `Total_Allocated_%` = Sum of all approved/proposed partner equity

**Example:**
- Growth Pool Budget: 15-20%
- Total Allocated: 2.08% (Beach House) + 0.5% (Gay Chee Cheong) = 2.58%
- **Remaining: 12.42% - 17.42%**

---

### Formula 5: Growth Pool % Consumed

```
Growth_Pool_Consumed_% = (Total_Allocated_% / Growth_Pool_Budget_%) × 100
```

**Example:**
- Total Allocated: 5.83% (if BHP gets 5% personal + 0.83% corporate)
- Growth Pool Budget: 15% (conservative end)
- **Growth Pool Consumed: 38.9%**

---

## Quick Calculation Table

### Scenario Analysis: Corporate Service Swap Only

| BHP Services | BH Services | Net Diff | @$12M Cap | @$10M Cap | @$15M Cap |
|--------------|-------------|----------|-----------|-----------|-----------|
| $150,000 | $50,000 | $100,000 | **0.83%** | 1.00% | 0.67% |
| $200,000 | $50,000 | $150,000 | **1.25%** | 1.50% | 1.00% |
| $150,000 | $75,000 | $75,000 | **0.625%** | 0.75% | 0.50% |
| $200,000 | $100,000 | $100,000 | **0.83%** | 1.00% | 0.67% |
| $300,000 | $100,000 | $200,000 | **1.67%** | 2.00% | 1.33% |

---

## Scenario Modeling: Total Dilution Impact

### Scenario A: Accept Full Request (5% Personal)

**Inputs:**
- BHP Services: $150,000
- BH Services: $50,000
- BH Valuation: $12,000,000
- Jocelyn Personal: 2.5%
- Donovan Personal: 2.5%

**Calculations:**
```
Corporate_Equity = ($150K - $50K) / $12M = 0.83%
Personal_Equity = 2.5% + 2.5% = 5.0%
Total_Dilution = 0.83% + 5.0% = 5.83%
Growth_Pool_Consumed = 5.83% / 15% = 38.9%
```

**Impact:**
- ❌ High Growth Pool consumption (39%)
- ❌ Only 9.17% remaining for all other partners
- ❌ Limits strategic advisor and capital partner capacity

---

### Scenario B: Counter-Offer (1.25% Personal)

**Inputs:**
- BHP Services: $150,000
- BH Services: $50,000
- BH Valuation: $12,000,000
- Jocelyn Personal: 0.75%
- Donovan Personal: 0.5%

**Calculations:**
```
Corporate_Equity = ($150K - $50K) / $12M = 0.83%
Personal_Equity = 0.75% + 0.5% = 1.25%
Total_Dilution = 0.83% + 1.25% = 2.08%
Growth_Pool_Consumed = 2.08% / 15% = 13.9%
```

**Impact:**
- ✅ Low Growth Pool consumption (14%)
- ✅ 12.92% remaining for other partners
- ✅ Room for tech advisors, capital partners, domain experts

---

### Scenario C: Increase Services, Lower Personal

**Inputs:**
- BHP Services: $200,000 (increased scope)
- BH Services: $50,000
- BH Valuation: $12,000,000
- Jocelyn Personal: 0.5%
- Donovan Personal: 0.25%

**Calculations:**
```
Corporate_Equity = ($200K - $50K) / $12M = 1.25%
Personal_Equity = 0.5% + 0.25% = 0.75%
Total_Dilution = 1.25% + 0.75% = 2.0%
Growth_Pool_Consumed = 2.0% / 15% = 13.3%
```

**Strategy:** Get more storytelling services, pay with equity, reduce personal advisory equity

---

### Scenario D: Decrease Services, Increase Personal (Compromise)

**Inputs:**
- BHP Services: $100,000 (reduced scope)
- BH Services: $50,000
- BH Valuation: $12,000,000
- Jocelyn Personal: 1.25%
- Donovan Personal: 1.0%

**Calculations:**
```
Corporate_Equity = ($100K - $50K) / $12M = 0.42%
Personal_Equity = 1.25% + 1.0% = 2.25%
Total_Dilution = 0.42% + 2.25% = 2.67%
Growth_Pool_Consumed = 2.67% / 15% = 17.8%
```

**Strategy:** Get less corporate services, give more personal equity (still below 5% request)

---

## Dynamic Calculator (Spreadsheet Formula)

### Google Sheets Implementation

**Setup:**
```
A1: "BHP Service Value"              B1: [Input: $150,000]
A2: "BH Service Value"               B2: [Input: $50,000]
A3: "Net Differential"               B3: =B1-B2
A4: "BH Valuation Cap"               B4: [Input: $12,000,000]
A5: "Corporate Equity %"             B5: =(B3/B4)*100
A6: "Jocelyn Personal %"             B6: [Input: 0.75]
A7: "Donovan Personal %"             B7: [Input: 0.5]
A8: "Total Studio Dilution %"        B8: =B5+B6+B7
A9: "Growth Pool Budget %"           B9: [Input: 15]
A10: "Other Allocated %"             B10: [Input: 0.5]
A11: "Total Allocated %"             B11: =B8+B10
A12: "Remaining Growth Pool %"       B12: =B9-B11
A13: "Growth Pool Consumed %"        B13: =(B11/B9)*100
```

**Result:**
- Change any input (B1, B2, B4, B6, B7, B9, B10)
- All calculations update automatically
- See real-time impact on total dilution and remaining capacity

---

## Negotiation Levers (What You Can Adjust)

### Lever 1: Service Scope & Value

**Beach House Services (BHP_Service_Value):**
- **Increase** ($150K → $200K+): More content, more ventures, ongoing support
- **Decrease** ($150K → $100K): Limited to WonderCast launch only, no ongoing

**Being Human Services (BH_Service_Value):**
- **Increase** ($50K → $100K): Deeper AI playground involvement, hands-on implementation
- **Decrease** ($50K → $25K): Strategy consultation only, no implementation

**Impact on Corporate Equity:**
- Wider gap = More equity to BHP
- Narrower gap = Less equity to BHP

**Example:**
- $200K BHP / $50K BH = $150K diff = **1.25% equity**
- $150K BHP / $100K BH = $50K diff = **0.42% equity**

---

### Lever 2: Valuation Cap

**BH Valuation Cap (BH_Valuation_Cap):**
- **Lower cap** ($12M → $10M): Higher equity % for same dollar value
- **Higher cap** ($12M → $15M): Lower equity % for same dollar value

**Impact on Corporate Equity:**

| Net Diff | @$10M | @$12M | @$15M |
|----------|-------|-------|-------|
| $100K | 1.00% | 0.83% | 0.67% |
| $150K | 1.50% | 1.25% | 1.00% |

**When to use:**
- If BH raises money at higher valuation, can offer lower equity %
- If negotiating with investor, lower cap = better for them, higher corporate equity

---

### Lever 3: Personal Advisory Equity Split

**Total Personal Equity:**
- Can allocate any % between Jocelyn and Donovan
- Doesn't affect total dilution, just the split

**Possible Splits:**

| Total | Jocelyn | Donovan | Rationale |
|-------|---------|---------|-----------|
| 1.25% | 0.75% | 0.5% | Jocelyn business dev focus = higher |
| 1.25% | 0.625% | 0.625% | Equal split |
| 2.0% | 1.0% | 1.0% | Equal split, higher total |
| 2.5% | 1.5% | 1.0% | Jocelyn higher for MD role |

**Plus Donovan Venture-Specific:**
- Add 1.0-1.5% WonderCast (doesn't affect studio equity)
- Add 1.0-1.5% Luminary (doesn't affect studio equity)

---

### Lever 4: Studio vs. Venture Equity Mix

**For Donovan Specifically:**

| Structure | Studio % | WonderCast % | Luminary % | Total Value Potential |
|-----------|----------|--------------|------------|----------------------|
| **High Studio** | 1.0% | 0.5% | 0.5% | Broad exposure, lower venture upside |
| **Balanced** | 0.5% | 1.0% | 1.25% | Recommended - aligns with creative impact |
| **Venture-Heavy** | 0.25% | 1.5% | 1.5% | Concentrated upside if ventures succeed |
| **Venture-Only** | 0% | 2.0% | 2.0% | Maximum venture exposure, no studio |

**Trade-off:**
- More studio % = Broader exposure to all BH ventures (winners + losers)
- More venture % = Concentrated upside in ventures where Donovan has most impact

---

## Threshold Analysis: What Equity Levels Allow

### If Total BHP Dilution ≤ 2.5%

**Remaining Capacity:** 12.5% - 17.5%

**Can Afford:**
- ✅ 4-6 strategic advisors (4-6%)
- ✅ 3-5 capital partners (3-5%)
- ✅ 2-3 domain experts (2-3%)
- ✅ 1-2 additional GTM partners (1-2%)
- ✅ Complete partner portfolio

---

### If Total BHP Dilution = 3.5% - 4.5%

**Remaining Capacity:** 10.5% - 16.5%

**Can Afford:**
- ✅ 3-4 strategic advisors (3-4%)
- ✅ 2-4 capital partners (2-4%)
- ⚠️ 1-2 domain experts (limited budget)
- ⚠️ 1 additional GTM partner (limited budget)
- ⚠️ Must prioritize carefully

---

### If Total BHP Dilution ≥ 5.5%

**Remaining Capacity:** 9.5% - 14.5%

**Can Afford:**
- ⚠️ 2-3 strategic advisors (forced choice on which types)
- ⚠️ 2-3 capital partners (limited to smaller checks)
- ❌ Limited domain expert budget
- ❌ No additional GTM partners
- ❌ Cannot build complete portfolio

**Critical Constraints:**
- Must choose between tech advisors OR capital partners (can't afford both well)
- Beach House becomes 37-39% of total Growth Pool
- Severely limits future flexibility

---

## Decision Matrix: Given Total Dilution, What to Prioritize

### If BHP Total = 2.0-2.5% (Recommended Range)

**Remaining:** ~13-17%

**Priority Allocation:**
1. Tech/AI Strategic Advisor (1.0%) - Capital access via investor networks
2. Capital Partner #1 (1.25%) - $250K+ anchor investor
3. Capital Partner #2 (1.0%) - $100-250K strategic investor
4. Strategic Advisor - Capital Focus (0.75%) - LP relationships
5. Enterprise GTM Partner (1.25%) - B2B distribution for Kavlo
6. Domain Expert - Education (0.75%) - Luminary/WonderCast validation

**Total Additional:** ~6.0%
**Total with BHP:** ~8.5%
**Reserve:** 6.5-11.5% for future opportunities

---

### If BHP Total = 5.5-6.0% (Their Request)

**Remaining:** ~9-14%

**Forced Choices:**
- Choose: Tech advisor (1.0%) OR Capital partner #1 (1.25%)? Can't afford both well.
- Choose: 2nd capital partner OR enterprise GTM? Not both.
- Domain experts likely cut entirely
- Only 1-2 additional strategic advisors possible (vs. target of 4-6)

**Result:** Incomplete partner portfolio, #1 constraint (Capital Access) under-solved

---

## Recommended Negotiation Ranges

### Corporate Service Swap (Accept as Calculated)

**Formula:** `Corporate_% = (BHP_Services - BH_Services) / BH_Valuation`

**Recommended Service Ranges:**
- BHP Services: $100K - $200K
- BH Services: $25K - $100K
- Net Differential: $50K - $150K

**Resulting Equity Range:**
- At $12M cap: **0.42% - 1.25%**
- At $10M cap: **0.50% - 1.50%**
- At $15M cap: **0.33% - 1.00%**

**Recommendation:** Accept whatever the formula yields based on actual service scopes

---

### Personal Advisory (Counter-Offer Range)

**Formula:** `Personal_% = Jocelyn_% + Donovan_%`

**Recommended Ranges:**

| Scenario | Jocelyn | Donovan | Total | When to Use |
|----------|---------|---------|-------|-------------|
| **Minimum** | 0.5% | 0.25% | 0.75% | If service swap is high (1.25%+) |
| **Base** | 0.75% | 0.5% | 1.25% | Recommended starting point |
| **Compromise** | 1.0% | 1.0% | 2.0% | If they won't budge below 5% |
| **Maximum** | 1.5% | 1.5% | 3.0% | Absolute ceiling before walking away |

**Plus Donovan Venture-Specific:**
- WonderCast: 0.5% - 1.5%
- Luminary: 0.75% - 1.5%

---

## Walk-Away Threshold

### When to Walk Away from Personal Advisory

**If Total Studio Dilution > 4.0%:**

```
If (BHP_Corporate_% + Jocelyn_% + Donovan_%) > 4.0%:
    Consider: Corporate only (BHP service swap)
    Defer: Personal advisory to future date
    Rationale: Preserves Growth Pool for higher-priority constraints
```

**Example:**
- Corporate: 0.83%
- Personal requested: 5.0%
- Total: 5.83%
- **Decision: Accept corporate (0.83%), defer personal advisory**

---

## Quick Reference: Formula Summary

```python
# Corporate Equity (Service Swap)
Corporate_Equity_% = ((BHP_Services - BH_Services) / BH_Valuation) * 100

# Total Studio Dilution
Total_Dilution_% = Corporate_% + Jocelyn_% + Donovan_%

# Remaining Growth Pool
Remaining_% = Growth_Pool_Budget_% - Total_Allocated_%

# Growth Pool Consumed
Consumed_% = (Total_Allocated_% / Growth_Pool_Budget_%) * 100

# Walk-Away Threshold
If Total_Dilution_% > 4.0%: Consider walking away from personal advisory
```

---

**Usage:** Input your actual negotiated numbers into these formulas to calculate real-time equity allocations and cap table impact.

**Prepared by:** Claude + Kyle Jackson
**Date:** February 1, 2026
**Status:** Dynamic Calculator - Ready for Negotiations
