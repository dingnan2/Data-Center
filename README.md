# Data Center Risk Assessment Framework: 12-Company Analysis

# Data Center Risk Assessment Framework

## Overview
This framework evaluates data center companies across three critical risk dimensions using qualitative flags and optional quantitative scoring. Companies with "Unknown" flags should not be penalized in final risk scoring but may be highlighted for follow-up or caution.

**Companies Evaluated:** American Tower, Applied Digital Corp,  CoreWeave, Digital Ocean Holdings, Digital Realty Trust, Digital Bridge Group Inc., Equinix, GDS Holdings, Iron Mountain, Oracle, VNET


# Data Center Company Business Model Classification

| **Company**            | **Business Model**          | **Notes**                                   | **Power Risk Assessment** |
| ---------------------- | --------------------------- | ------------------------------------------- | ------------------------- |
| Digital Realty Trust (DLR) | Operator REIT               | Owns & operates global hyperscale data centers | ✓ Include |
| Equinix (EQIX)         | Operator REIT               | Owns & operates colocation/interconnection facilities | ✓ Include |
| CoreWeave              | Operator (Private)          | Owns/operates GPU cloud infrastructure for AI/ML | ✓ Include |
| Core Scientific (CORZ) | Operator                    | Owns/operates Bitcoin mining & HPC data centers | ✓ Include |
| GDS Holdings (GDS)     | Operator                    | Owns/operates data centers primarily in China | ✓ Include |
| Applied Digital Corp (APLD) | Operator                | Owns/operates HPC & Bitcoin mining facilities | ✓ Include |
| American Tower (AMT)   | Mixed: Tower REIT + Data Center Operator | Towers (leasing) + CoreSite data centers (operator) | ✓ Include (DC segment only) |
| Iron Mountain (IRM)    | Mixed: Storage + Data Center Operator | Records storage + owns/operates data centers | ✓ Include (DC segment only) |
| VNET Group (VNET)      | Operator                    | Owns/operates data centers & managed services in China | ✓ Include |
| Digital Ocean Holdings (DOCN) | Cloud Provider (Leasing) | Cloud platform using leased data center capacity | ✗ Exclude |
| Oracle (ORCL)          | Mixed: Software + Cloud Operator | Software + owns/operates Oracle Cloud Infrastructure | ✓ Include (OCI segment only) |
| Digital Bridge Group (DBRG) | Investment Manager        | Digital infrastructure investment firm, not operator | ✗ Exclude |



---

## I. Power Risk Evaluation Framework

### 1. Power Infrastructure Resilience & Security

#### a. Grid Redundancy & Backup Systems
- **Flag Options:** Multiple Grid Connections / Comprehensive Backup / Basic Backup / Minimal
- **Purpose:** Assesses operational continuity and protection against power outages
- **Evaluation:** Multiple Grid Connections = 0 / Comprehensive Backup = 5 / Basic Backup = 15 / Minimal = 25
> - *Multiple Grid Connections*: physically diverse feeds from separate substations/utility providers (true redundancy).
> - *Comprehensive Backup*: Should include N+1 or 2N generators and long-duration on-site fuel (24–48 hours).
> - *Basic Backup*: Often just single feed + standby generators.
> - *Minimal*: Single grid feed with short-duration UPS only, or outdated diesel-only backup

#### b. Regional Power Constraint Exposure  
- **Flag Options:** No High-Risk Regions / <25% in Risk Regions / 25-50% / >50%
- **Purpose:** Identifies exposure to power-constrained regions (Northern Virginia, California, Texas grid issues)
- **Evaluation:** No High-Risk Regions = 0 / <25% in Risk Regions = 5 / 25-50% = 15 / >50% = 25
> - *High-Risk Regions*: 
>   - Northern Virginia (Dominion Energy delays)
>   - California (PG&E reliability, wildfire shutoffs)
>   - Texas (ERCOT grid instability)

> Numerator: Facilities located in “high-risk” power regions
> Denominator: Total operational facilities (owned/operated data centers)

### 2. Power Capacity Growth & Scalability 
#### a. Secured Future Power Capacity
- **Flag Options:** Multi-Year Pipeline Secured / 1-2 Years Secured / <1 Year Secured / No Clear Pipeline
- **Purpose:** Evaluates ability to scale operations without power constraints in AI/hyperscale demand environment
- **Evaluation:** Multi-Year Pipeline = 0 / 1-2 Years = 5 / <1 Year = 10 / No Clear Pipeline = 20

#### b. Power Procurement Strategy
- **Flag Options:** Diversified Long-term Contracts / Some Long-term / Mostly Spot Market / Unknown/Ad-hoc
- **Purpose:** Measures strategic approach to securing reliable power supply for growth
- **Evaluation:** Diversified Long-term = 0 / Some Long-term = 5 / Mostly Spot = 10 / Unknown/Ad-hoc = 15

### 3. Energy Cost Management & Volatility 

#### a. Power Cost Hedging/Stabilization Strategy
- **Flag Options:** Comprehensive Hedging / Partial Hedging / Limited Hedging / No Hedging Strategy
- **Purpose:** Measures protection against energy price volatility and margin stability
- **Evaluation:** Comprehensive Hedging = 0 / Partial Hedging = 5 / Limited Hedging = 10 / No Hedging = 20

#### b. Energy Cost Transparency & Management
- **Flag Options:** Detailed Cost Breakdown / Basic Disclosure / Minimal Disclosure / No Disclosure
- **Purpose:** Assesses management's control and transparency over energy cost structure
- **Evaluation:** Detailed Breakdown = 0 / Basic Disclosure = 3 / Minimal = 7 / No Disclosure = 10


### 4. Operational Energy Efficiency 

#### a. Power Usage Effectiveness (PUE)
- **Flag Options:** ≤1.25 / 1.25-1.4 / 1.4-1.6 / >1.6 or Unknown
- **Purpose:** Measures operational efficiency and competitive positioning in energy utilization
- **Evaluation:** ≤1.25 = 0 / 1.25-1.4 = 5 / 1.4-1.6 = 10 / >1.6 or Unknown = 15

#### b. Efficiency Improvement Trajectory
- **Flag Options:** Improving Trend / Stable Performance / Declining Trend / No Historical Data
- **Purpose:** Indicates management's operational excellence and forward-looking efficiency gains
- **Evaluation:** Improving Trend = 0 / Stable Performance = 3 / Declining Trend = 7 / No Data = 10


### 5. Sustainability & Regulatory Risk

#### a. Renewable Energy Integration
- **Flag Options:** >75% Renewable / 50–75% Renewable / 25–50% Renewable / <25% or Unknown
- **Purpose:** Captures long-term regulatory compliance risk and ESG-related constraints tied to renewable adoption
- **Evaluation:** >75% = 0 / 50–75% = 5 / 25–50% = 10 / <25% or Unknown = 15
#### b. ESG/Climate Regulatory Preparedness
- **Flag Options:** Comprehensive Strategy / Basic Strategy / Minimal Planning / No Clear Strategy
- **Purpose:** Assesses readiness for evolving environmental regulations and carbon pricing mechanisms
- **Evaluation:** Comprehensive Strategy = 0 / Basic Strategy = 3 / Minimal Planning = 7 / No Strategy = 10


---


### Total Power Risk Score Calculation:
**Total Score = Σ(Individual Metric Score)**

### Risk Categories:
- **Low Risk:** 0-25 points
- **Moderate Risk:** 26-50 points  
- **High Risk:** 51-75 points
- **Very High Risk:** 76-100 points

---


## II. Geographic Risk Evaluation Framework

### 1. Asset Geographic Concentration Risk
- **Flag Options:** Highly Concentrated / Moderately Concentrated / Well Diversified
- **Purpose:** Measures physical infrastructure concentration to assess operational continuity risk from localized disruptions
- **Evaluation:** Highly Concentrated = 20 / Moderately Concentrated = 10 / Well Diversified = 0

**Assessment Criteria:**
- *Highly Concentrated*: >60% of assets/capacity in single country or >40% in single metro area
- *Moderately Concentrated*: 25-40% in single metro area OR limited regional diversity within country  
- *Well Diversified*: <40% in single country and <25% in single metro area


---

### 2. Revenue Geographic Concentration Risk  
- **Flag Options:** Highly Concentrated / Moderately Concentrated / Well Diversified
- **Purpose:** Evaluates market dependency risk from localized revenue concentration that creates economic vulnerability
- **Evaluation:** Highly Concentrated = 15 / Moderately Concentrated = 8 / Well Diversified = 0

**Assessment Criteria:**
- *Highly Concentrated*: >40% revenue from single metro area OR >25% from single facility/campus
- *Moderately Concentrated*: 25-40% revenue from single metro area OR 15-25% from single facility/campus
- *Well Diversified*: <25% revenue from single metro area AND <15% from single facility/campus

**Geographic Risk Hierarchy (Highest to Lowest Risk):**
- Single facility/campus dominance (>25% revenue)
- Single metro concentration (>40% revenue)
- Single region within large country (acceptable if diversified across metros)
- Single country with multi-metro distribution (low risk)
- Multi-country operations (lowest risk)
> **Note:** For companies with limited metro-level disclosure, use the most granular geographic breakdown available (state/province level for large countries). Single-country concentration is acceptable if revenue is distributed across multiple metropolitan areas.

---

### 3. High-Risk Geographic Exposure
- **Flag Options:** High Exposure / Moderate Exposure / Low Exposure  
- **Purpose:** Quantifies exposure to regions with known infrastructure, regulatory, or operational challenges
- **Evaluation:** High Exposure = 15 / Moderate Exposure = 8 / Low Exposure = 0

**High-Risk Regions Defined:**
- **Regulatory/Political Risk:** China (GDS, VNET), European markets with strict data sovereignty laws
- **Power Grid Risk:** Northern Virginia (Dominion Energy constraints), California (PG&E reliability), Texas (ERCOT instability)
- **Infrastructure Risk:** Emerging markets with unstable power/telecom infrastructure

**Assessment Criteria:**
- *High Exposure*: >40% of assets/revenue in high-risk regions
- *Moderate Exposure*: 20-40% of assets/revenue in high-risk regions  
- *Low Exposure*: <20% of assets/revenue in high-risk regions

---

### 4. Natural Disaster & Climate Risk Exposure
- **Flag Options:** High Risk / Moderate Risk / Low Risk
- **Purpose:** Assesses physical asset vulnerability to climate events that could disrupt operations or require costly infrastructure hardening
- **Evaluation:** High Risk = 10 / Moderate Risk = 5 / Low Risk = 0

**Risk Zones:**
- *High Risk*: Hurricane zones (Southeast US, Caribbean), Wildfire zones (California), Seismic zones (California, Japan), Flood-prone areas
- *Moderate Risk*: Areas with occasional severe weather but lower frequency/intensity
- *Low Risk*: Geographically stable regions with minimal natural disaster history

**Assessment Criteria:**
- *High Risk*: >50% of critical assets in high-risk natural disaster zones
- *Moderate Risk*: 25-50% of critical assets in high-risk zones
- *Low Risk*: <25% of critical assets in high-risk zones

---

### 5. Market Saturation & Competition Risk  
- **Flag Options:** High Saturation / Moderate Saturation / Low Saturation
- **Purpose:** Evaluates competitive intensity in primary markets - saturated markets typically have pricing pressure and limited expansion opportunities
- **Evaluation:** High Saturation = 8 / Moderate Saturation = 4 / Low Saturation = 0

**Market Assessment:**
- *High Saturation*: Concentrated in mature markets (Northern Virginia, Silicon Valley, London, Frankfurt) with intense competition
- *Moderate Saturation*: Mix of mature and emerging markets, or secondary markets with moderate competition
- *Low Saturation*: Significant presence in emerging/underserved markets with growth potential

---

## Geographic Risk Scoring Summary

| Sub-Metric | Score Range | Weight |
|------------|-------------|---------|
| Asset Geographic Concentration | 0-20 | 30% |
| Revenue Geographic Concentration | 0-15 | 25% |
| High-Risk Geographic Exposure | 0-15 | 25% |
| Natural Disaster & Climate Risk | 0-10 | 15% |
| Market Saturation & Competition | 0-8 | 5% |

**Total Geographic Risk Score = Σ(Individual Metric Score × Weight)**

### Risk Categories:
- **Low Risk:** 0-5 points
- **Moderate Risk:** 6-10 points  
- **High Risk:** 11-15 points
- **Very High Risk:** 16+ points

---

## III. Customer Concentration Risk 

### 1. Single Customer Dependency Risk
- **Flag Options:** Low Dependency / Moderate Dependency / High Dependency / Unknown
- **Purpose:** Measures reliance on largest single customer - critical for assessing revenue stability and negotiation leverage
- **Evaluation:** Low Dependency = 0 / Moderate Dependency = 8 / High Dependency = 20 / Unknown = 12

**Assessment Criteria:**
- *Low Dependency*: Largest customer <10% of total revenue
- *Moderate Dependency*: Largest customer 10-25% of total revenue  
- *High Dependency*: Largest customer >25% of total revenue
- *Unknown*: No disclosure of customer concentration metrics

> **Data Sources:** 10-K "Concentration of Credit Risk" sections, revenue footnotes, management discussion

---

### 2. Top Customer Portfolio Concentration
- **Flag Options:** Well Diversified / Moderately Concentrated / Highly Concentrated / Unknown
- **Purpose:** Evaluates broader customer concentration beyond single largest customer - captures oligopoly risk
- **Evaluation:** Well Diversified = 0 / Moderately Concentrated = 5 / Highly Concentrated = 15 / Unknown = 8

**Assessment Criteria:**
- *Well Diversified*: Top 5 customers <40% of revenue OR Top 10 customers <50% of revenue
- *Moderately Concentrated*: Top 5 customers 40-60% OR Top 10 customers 50-70%
- *Highly Concentrated*: Top 5 customers >60% OR Top 10 customers >70%
- *Unknown*: Limited disclosure beyond largest customer

---

### 3. Customer Type & Pricing Power Risk
- **Flag Options:** Favorable Mix / Moderate Risk / High Risk / Unknown
- **Purpose:** Assesses customer quality, negotiation dynamics, and revenue predictability based on customer segment characteristics
- **Evaluation:** Favorable Mix = 0 / Moderate Risk = 6 / High Risk = 12 / Unknown = 6

**Customer Segments Defined:**
- **Enterprise/SMB:** Higher pricing power, stickier relationships, longer decision cycles
- **Hyperscalers (AWS, Azure, GCP):** Volume pricing pressure, sophisticated procurement, high switching capability
- **Government:** Stable but bureaucratic, security requirements, budget-dependent
- **Cryptocurrency/Speculative:** Volatile demand, price-sensitive, regulatory risk

**Assessment Criteria:**
- *Favorable Mix*: >60% enterprise/government, minimal hyperscaler exposure
- *Moderate Risk*: Balanced mix or moderate hyperscaler exposure (20-50%)
- *High Risk*: >50% hyperscaler/crypto exposure or single sector dominance
- *Unknown*: No meaningful customer segmentation disclosure

---

### 4. Contract Duration & Revenue Stability
- **Flag Options:** Strong Protection / Moderate Protection / Weak Protection / Unknown
- **Purpose:** Measures contractual revenue protection and customer switching costs - longer terms reduce concentration risk impact
- **Evaluation:** Strong Protection = 0 / Moderate Protection = 4 / Weak Protection = 10 / Unknown = 6

**Contract Assessment:**
- *Strong Protection*: Average contract >3 years, majority take-or-pay terms, high early termination costs
- *Moderate Protection*: Mix of long/short terms (1-3 years average), some committed capacity
- *Weak Protection*: Month-to-month or <1 year terms, minimal commitment requirements
- *Unknown*: Limited contract term disclosure

**Key Indicators:**
- Take-or-pay provisions
- Early termination penalties  
- Automatic renewal clauses
- Committed vs. on-demand pricing

---

### 5. Customer Financial Quality & Credit Risk
- **Flag Options:** High Quality / Mixed Quality / Concerning Quality / Unknown
- **Purpose:** Evaluates customer financial stability and payment risk - financially weak customers amplify concentration risk
- **Evaluation:** High Quality = 0 / Mixed Quality = 3 / Concerning Quality = 8 / Unknown = 4

**Quality Assessment:**
- *High Quality*: Majority investment-grade customers, Fortune 500 enterprises, major cloud providers
- *Mixed Quality*: Combination of established and emerging companies, some non-rated entities
- *Concerning Quality*: High exposure to startups, financially distressed companies, or high-risk sectors
- *Unknown*: No meaningful customer quality disclosure

**Risk Indicators:**
- Customer payment history/bad debt provisions
- Industry sectors served (tech vs. traditional enterprise)
- Customer lifecycle stage (startup vs. established)
- Geographic customer risk (emerging vs. developed markets)

---

## Customer Concentration Risk Scoring Summary

| Sub-Metric | Score Range | Weight | Rationale |
|------------|-------------|---------|-----------|
| Single Customer Dependency | 0-20 | 35% | Highest impact risk factor |
| Top Customer Portfolio Concentration | 0-15 | 25% | Captures oligopoly effects |
| Customer Type & Pricing Power | 0-12 | 20% | Affects negotiation dynamics |
| Contract Duration & Stability | 0-10 | 15% | Mitigates concentration impact |
| Customer Financial Quality | 0-8 | 5% | Credit risk amplifier |

**Total Customer Concentration Risk Score = Σ(Individual Metric Score × Weight)**

### Risk Categories:
- **Low Risk:** 0-6 points
- **Moderate Risk:** 7-12 points  
- **High Risk:** 13-18 points
- **Very High Risk:** 19+ points


---

## Implementation Guidelines

1. **Consistency:** All evaluators should use the same methodology to avoid bias
2. **Documentation:** Record specific evidence and SEC filing references for each flag assignment
3. **Unknown Handling:** Companies with "Unknown" flags should be highlighted for follow-up rather than penalized
4. **Weighting:** Consider applying weights based on strategic importance of each risk dimension
