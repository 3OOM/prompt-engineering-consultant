# Business Consultation Prompt Collection

A comprehensive repository of production-grade prompt templates implementing advanced reasoning frameworks: Chain-of-Thought (CoT), Tree-of-Thoughts (ToT), Self-Consistency Validation, Weighted Decision Scoring, and Planning Prompting.

---

## Framework Architecture (The APEX Consulting Model)

```
        ┌────────────────────────────────────────────────────────┐
        │                 A - ASSESS                             │
        │   Chain-of-Thought (CoT) Diagnostic SWOT Analysis      │
        └───────────────────────────┬────────────────────────────┘
                                    │
                                    ▼
        ┌────────────────────────────────────────────────────────┐
        │                 P - PINPOINT                           │
        │   Root-Cause Bottleneck Isolation & Gap Analysis       │
        └───────────────────────────┬────────────────────────────┘
                                    │
                                    ▼
        ┌────────────────────────────────────────────────────────┐
        │                 E - EVALUATE                           │
        │   Tree-of-Thoughts (ToT) Multi-Branch Scoring          │
        │   Self-Consistency Validation & Weighted Matrix        │
        └───────────────────────────┬────────────────────────────┘
                                    │
                                    ▼
        ┌────────────────────────────────────────────────────────┐
        │                 X - eXECUTE                            │
        │   Two-Stage Planning Prompting (12-Month Roadmap)      │
        │   Risk Mitigation Registry                             │
        └────────────────────────────────────────────────────────┘
```

---

## Template 1: Diagnostic Assessment & SWOT Analysis (CoT + Persona)

- **Framework:** Persona Conditioning + Zero-Shot Chain-of-Thought (CoT)
- **Objective:** Establish the consulting persona, ingest client baseline dossier metrics, and systematically generate a structured SWOT analysis.

### Prompt Template
```markdown
Act as a Senior Management Consultant specializing in retail supply chain turnaround and omnichannel e-commerce strategy.

We are conducting the ASSESS stage of a strategic turnaround engagement for our client: [Insert Client Name].

[CLIENT DOSSIER & METRICS]:
- Physical Footprint: [Insert Store Count & Geography]
- Top-Line Financials: [Insert Annual Revenue & Margin Trends]
- Channel Performance: [Insert Foot Traffic Trends]
- Digital Metrics: [Insert E-Commerce Conversion Rate & Cart Abandonment Rate]
- Operational Bottlenecks: [Insert Warehousing, Logistics & Inventory Tracking Systems]

Let's think step-by-step to diagnose this client's current operating health:
1. Break down the internal strengths and weaknesses based strictly on the provided performance metrics.
2. Identify external market opportunities and threats relevant to modern apparel consumer behavior.
3. Synthesize findings into a formal 4-quadrant SWOT Analysis in Markdown table format.
4. Conclude with a 2-sentence executive summary defining the firm's strategic posture.
```

---

## Template 2: Root-Cause Bottleneck & Strategic Gap Analysis (CoT)

- **Framework:** Sequential Chain-of-Thought Root-Cause Isolation
- **Objective:** Prevent symptom-treating by isolating the fundamental operational failure causing margin compression, followed by a formal Current vs. Desired State gap analysis.

### Prompt Template
```markdown
Act as a Principal Business Systems Analyst. 

Using the client metrics and SWOT analysis established for [Insert Client Name], let's think step-by-step to execute the PINPOINT stage of our engagement:

Step 1 - Causal Logic Chain:
Trace the causal chain explaining exactly why operating margins have compressed by [Insert Margin Decline %]. Show how warehouse operations, inventory tracking, and e-commerce friction interlink.

Step 2 - Root-Cause Identification:
Pinpoint the single most critical root-cause bottleneck. Explain why this bottleneck is the primary driver rather than a secondary symptom.

Step 3 - Strategic Gap Analysis:
Construct a Markdown table comparing the client's Current State (Baseline) against the Desired Optimized State across four core operational dimensions:
1. Inventory Visibility & Tracking
2. Fulfillment Velocity & Logistics
3. E-Commerce Conversion & Funnel Friction
4. Cost Structure & Working Capital

Output the step-by-step diagnostic reasoning followed by the finalized Gap Analysis table.
```

---

## Template 3: Tree of Thoughts (ToT) Multi-Branch Evaluation

- **Framework:** Tree-of-Thoughts (ToT) Parallel Exploration & Pruning
- **Objective:** Generate and evaluate three competing strategic alternatives across margin impact, CapEx requirements, and execution risk, scoring each out of 10.

### Prompt Template
```markdown
Act as an Executive Strategy Director. We need to execute the EVALUATE stage for [Insert Client Name].

Generate three distinct, mutually exclusive strategic solution branches designed to restore profitability:
- Branch A: [Insert Branch A Name - e.g., E-Commerce & Logistics Overhaul]
- Branch B: [Insert Branch B Name - e.g., Retail Footprint Downsizing]
- Branch C: [Insert Branch C Name - e.g., Hybrid B2B Licensing & Franchising]

Evaluate each strategic branch in parallel. For each option, systematically analyze:
1. Estimated Impact on Margins (High / Med / Low with strategic justification).
2. Capital Expenditure (CapEx) Required (High / Med / Low with cost drivers).
3. Execution Risk (Primary organizational, technical, or legal failure modes).

Let's think step-by-step through the trade-offs of each branch.
Assign an overall strategic score from 1.0 to 10.0 for each branch, state the winning recommendation, and explain why the other two branches were pruned.
```

---

## Template 4: Self-Consistency Validation Protocol

- **Framework:** Self-Consistency Sampling & Deterministic Validation
- **Objective:** Run the ToT prompt across multiple distinct chat threads to verify whether the model converges deterministically on the winning branch.

### Prompt Template
```markdown
Act as an Independent Management Auditor. 

Review the strategic problem facing [Insert Client Name] with the following operational constraints:
- Margins eroding due to inventory carry costs.
- Store foot traffic down 25%.
- E-commerce cart abandonment at 82% with 5-7 days fulfillment latency.

Without referencing prior conversation context, independently evaluate whether the organization should:
Option A: Overhaul E-commerce, automated inventory, and switch to 3PL logistics.
Option B: Downsize the physical retail store footprint by closing 15 unprofitable stores.
Option C: Convert physical stores to franchise licenses and shift to wholesale.

Rank the three options in order of strategic viability (1st, 2nd, 3rd) and provide a 3-bullet justification for your top choice.
```

---

## Template 5: Weighted Decision Matrix Calculation

- **Framework:** Quantitative Multi-Criteria Decision Analysis (MCDA)
- **Objective:** Compute a mathematically rigorous weighted decision matrix where criteria weights sum to exactly 1.00 (100%), applying the formula `Weighted Score = Raw Score × Weight`.

### Prompt Template
```markdown
Act as a Quantitative Management Analyst. Create a mathematically verified Weighted Decision Matrix comparing the three strategic candidates:
- Branch A: E-Commerce & Logistics Overhaul
- Branch B: Retail Footprint Downsizing
- Branch C: Hybrid B2B Licensing

Evaluate each branch across the following four criteria with explicit weights (weights must sum to exactly 100% / 1.00):
1. Return on Investment (ROI): 30% weight (0.30)
2. Resource & Capability Alignment: 30% weight (0.30)
3. Low Execution Risk: 20% weight (0.20)
4. Implementation Speed: 20% weight (0.20)

For each option, assign a Raw Score from 1 (unacceptable) to 10 (exceptional) for each criterion.
Calculate the exact Weighted Score using the formula: Weighted Score = Raw Score × Weight.

Output the results in a Markdown table with the following column headers:
| Solution | Criterion | Weight | Score (1-10) | Weighted Score |

At the bottom of the table, provide the total summed score out of 10.0 for each candidate and declare the mathematical winner.
```

---

## Template 6: Phased Roadmap Planning Prompt (Two-Stage Planning Prompting)

- **Framework:** Two-Stage Planning Prompting (Outline → Expansion) to eliminate token truncation.
- **Objective:** Structure a 12-month implementation roadmap for the selected strategy across three distinct phases with milestones and RACI accountability.

### Prompt Template (Stage 1: Outline Phase)
```markdown
We have selected Branch A (E-Commerce & Logistics Overhaul) as the winning strategy for [Insert Client Name]. 
Act as a Senior Engagement Project Manager.

First, outline three distinct implementation phases covering a 12-month project lifecycle.
Pause and output ONLY the phase names, objective statements, and duration windows (e.g., Months 1–3). 
Do NOT generate detailed activities or tables yet. 
Wait for my explicit command: "Execute".
```

### Prompt Template (Stage 2: Detailed RACI Expansion)
```markdown
Execute. 

Now, for each of the three defined phases, output:
1. Detailed Core Activities & Deliverables.
2. Phase Milestone Gate Criteria.
3. A complete RACI Matrix (Responsible, Accountable, Consulted, Informed) identifying roles across Executive Sponsor, VP of Supply Chain, Head of E-Commerce, 3PL Partner, and Lead Systems Integrator.
```

---

## Template 7: Risk Mitigation Registry (4-Column Matrix)

- **Framework:** Formal Risk Registry & Failure Mode Mitigation
- **Objective:** Identify the top 3 mission-critical implementation risks and structure them into a standardized 4-column risk registry.

### Prompt Template
```markdown
Act as a Risk Management Director for enterprise supply chain transformations.

For the selected E-Commerce & Logistics Overhaul implementation, identify the three most critical operational and technical risks that could derail project delivery.

Format the output strictly as a Markdown table with the following four columns:
| Risk Event | Probability (Low/Med/High) | Impact (Low/Med/High) | Mitigation Strategy |

Ensure each mitigation strategy is actionable, preventative, and specifies operational controls (e.g., buffer stock protocols, automated failovers, parallel legacy run periods).
```
