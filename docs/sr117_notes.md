# SR 11-7 Study Notes
## Sections I–III: Introduction, Purpose & Scope, Overview of Model Risk Management

**Source:** Federal Reserve / OCC - Supervisory Guidance on Model Risk Management (SR 11-7 / OCC 2011-12)
**Prepared by:** Gouri 
-----

## I. INTRODUCTION

### Why Models Matter in Banking
Banks rely heavily on **quantitative models** across virtually all areas of financial decision-making. The regulatory scope covers:
- National banks (OCC primary supervisor)
- Bank holding companies and state member banks (Federal Reserve primary supervisor)

**Key model use cases in banking:**
- Underwriting credits
- Valuing exposures, instruments, and positions
- Measuring risk
- Managing and safeguarding client assets
- Determining capital and reserve adequacy

### Growing Complexity of Model Use
In recent years, model applications have grown more ambitious - enterprise-wide risk measurement, multi-risk Basel capital frameworks (market, credit, operational risk). Two forces are driving this:
1. **Regulatory pressure** : Basel Committee capital rules (market, credit, operational risk) require quantitative modelling.
2. **Business appetite** : banks have independently been expanding data-driven, quantitative decision-making for years.

### The Model Cost-Benefit Reality
> Models improve business decisions — but they come with real costs.

| Cost Type | Description |
|---|---|
| **Direct costs** | Resources to develop and implement models properly |
| **Indirect costs** | Adverse consequences (including financial loss) from incorrect or misused models |

The indirect costs are managed through **active model risk management** this is the central subject of SR 11-7.

### Document Roadmap
| Section | Topic |
|---|---|
| II | Purpose and Scope |
| III | Overview of Model Risk Management |
| IV | Model Development, Implementation, and Use |
| V | Effective Validation Framework |
| VI | Governance, Policies, and Controls |
| VII | Conclusion |

-----

## II. PURPOSE AND SCOPE

### Purpose
SR 11-7 provides **comprehensive guidance** on model risk management, not just validation, but the full lifecycle:
- Development, implementation, and use
- Validation
- Governance and controls

### What's New vs. Prior Guidance
Previous OCC/Fed guidance (OCC 2000-16, SR 09-01) focused heavily on **model validation**. SR 11-7 **expands the scope** to cover all aspects of model risk management.

Prior publications referenced:
- OCC 2000-16 (May 2000) : model validation guidance
- SR Letter 09-01 : Market Risk Rule, validation standards, back-testing
- Fed's Trading and Capital : Markets Activities Manual
- Advanced-approaches capital rules (12 CFR 3, 208, 225) : explicit validation requirements

### Proportionality Principle
SR 11-7 is **not one-size-fits-all.** Expectations scale with:
- Size and complexity of the bank
- Number and complexity of models used
- Risk exposure and business activities

> A community bank with a few moderate-complexity models needs a much lighter-touch approach than a large bank with extensive, complex model use.

**Key takeaway:** All banks must ensure internal policies are consistent with SR 11-7 principles but the *depth* of implementation is commensurate with risk.

-----

## III. OVERVIEW OF MODEL RISK MANAGEMENT

### The SR 11-7 Definition of a Model ⭐
This is one of the most important definitions in the document.

> **A model** is a quantitative method, system, or approach that applies **statistical, economic, financial, or mathematical theories, techniques, and assumptions** to process **input data** into **quantitative estimates**.

#### The Three Components of a Model

```
[Input Component]  →  [Processing Component]  →  [Reporting Component]
  Assumptions            Transforms inputs           Translates estimates
  & data                 into estimates              into business info
```

**Important nuance:** The definition includes quantitative approaches whose *inputs* are partially qualitative or based on expert judgment — **as long as the output is quantitative.** Purely qualitative approaches fall outside SR 11-7's scope (but still need a rigorous control process - Footnote 3).

#### What Counts as a "Model" Under SR 11-7?
- Credit scoring models
- Market valuation models
- Stress testing models
- Capital adequacy models (CCAR, DFAST)
- Client asset management models
- Compliance limit monitoring tools
- Financial and regulatory reporting tools

-----

### Why Models Are Never Perfect

Models are **simplified representations** of real-world relationships. Simplification is:
- **Inevitable** — real-world relationships are inherently complex
- **Intentional** — focus is placed on what matters most for a given use case

#### Model Quality Metrics (context-dependent)
| Metric | When It Applies |
|---|---|
| Precision & Accuracy | Models that forecast future values |
| Discriminatory Power | Models that rank-order risks (e.g., credit scorecards) |
| Robustness & Stability | Stress testing, capital models |
| Reliability | Production/ongoing use models |

-----

### What Is Model Risk?

> **Model risk** = the potential for adverse consequences from decisions based on **incorrect or misused** model outputs and reports.

Consequences include:
- Financial loss
- Poor business and strategic decision making
- Damage to a bank's reputation

#### Two Root Causes of Model Risk

**Cause 1: Fundamental Model Errors**
Errors can occur at any point in the model development lifecycle:
- Theory application
- Sample design and numerical routines
- Input selection and estimation
- Information systems implementation
- Shortcuts/simplifications that compromise integrity
- Poor-quality input data or incorrect assumptions

**Cause 2: Incorrect or Inappropriate Use**
Even a technically sound model carries high risk if misapplied:
- Used outside the environment it was designed for
- Applied to new products or markets it wasn't built for
- Market conditions or customer behaviour change around it
- Decision makers don't understand its limitations

> This is a critical insight for governance: **model fitness for purpose** is as important as technical correctness.

-----

### Managing Model Risk

#### Assessing the Magnitude
Model risk increases with:
- Greater model complexity
- Higher uncertainty about inputs and assumptions
- Broader scope of use
- Larger potential impact on the bank

Banks must consider risk at two levels:
1. **Individual model level** : each model's own errors and limitations
2. **Aggregate level** : interaction/dependencies between models, shared assumptions or data, common methodologies

#### The Guiding Principle: Effective Challenge ⭐
> **Effective challenge** = critical analysis by **objective, informed parties** who can identify model limitations and assumptions and produce appropriate changes.

Three pillars of effective challenge:

| Pillar | What It Means |
|---|---|
| **Incentives** | Separation from model development process; well-designed compensation practices and corporate culture |
| **Competence** | Technical knowledge and modelling skills to conduct rigorous analysis and critique |
| **Influence** | Explicit authority, organisational stature, and management commitment to act on findings |

#### Tools Beyond Validation
Even with robust validation, model risk can't be fully eliminated. Additional tools:
- Establishing **limits on model use**
- **Monitoring model performance** over time
- **Adjusting or revising models** as conditions change
- **Supplementing model results** with other analysis and information
- **Informed conservatism** — in inputs, design, or output adjustments (not an excuse to avoid fixing models)

#### Materiality Matters
- Where model use is limited and impact is low --> lighter MRM framework may meet supervisory expectations
- Where model output **materially affects** business decisions, risk management, capital/liquidity planning, and model failure would be **particularly harmful** --> framework must be more extensive and rigorous

-----

### The Three Pillars of Model Risk Management

```
┌─────────────────────────────────────────────────────────────┐
│              MODEL RISK MANAGEMENT (SR 11-7)                │
├─────────────────┬────────────────────┬──────────────────────┤
│   DEVELOPMENT   │    VALIDATION      │     GOVERNANCE       │
│ Implementation  │                    │                      │
│   & Use         │  Independent       │  Roles &             │
│                 │  challenge of      │  responsibilities    │
│  Robust, fit-   │  model soundness   │  Communication of    │
│  for-purpose    │  and appropriate   │  limitations         │
│  model build    │  application       │  Authority to        │
│                 │                    │  restrict usage      │
└─────────────────┴────────────────────┴──────────────────────┘
```

-----

## Key Concepts to Remember

| Concept | SR 11-7 Position |
|---|---|
| Model definition | 3-component quantitative system (input --> processing --> reporting) |
| Model risk | Risk from incorrect outputs OR misuse of correct outputs |
| Effective challenge | Objective, competent, influential independent review |
| Proportionality | MRM depth scales with bank size, model complexity, and materiality |
| Aggregate risk | Models don't just have individual risk — shared assumptions create systemic vulnerability |
| Informed conservatism | Acceptable tool, but not a substitute for fixing models |

-----
