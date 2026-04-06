# AI Governance & Model Lifecycle Architect Lab

A practical, hands-on repository for building and governing machine learning models end-to-end from data exploration and model development through to validation, monitoring, explainability, and regulatory compliance.

This lab covers the full model risk management lifecycle, grounded in real regulatory frameworks used across financial services.

-----

## What This Repository Covers

### Model Development & Validation
- Exploratory data analysis and feature engineering using Python and pandas
- Logistic regression modelling with scikit-learn
- Model validation metrics: KS statistic, Gini coefficient, Population Stability Index (PSI), ROC-AUC
- Full model validation framework aligned to SR 11-7 and SS1/23

### Explainability & Fairness
- SHAP (SHapley Additive exPlanations) for feature importance and individual prediction explanations
- Bias and fairness analysis across demographic groups
- Responsible AI principles applied to credit risk use cases

### ML Lifecycle & Monitoring
- Experiment tracking and model versioning with MLflow
- Data drift and model performance monitoring with Evidently AI
- End-to-end ML pipeline connecting data ingestion, training, evaluation, and monitoring
- Reusable Python modules in `src/` for metrics, monitoring, explainability, and fairness

### AI Governance & Regulatory Frameworks
- **SR 11-7** (Federal Reserve) : Model Risk Management
- **SS1/23** (Bank of England) : Model Risk Management
- **EU AI Act** : Risk classification, High Risk AI obligations
- **NIST AI RMF** : Govern, Map, Measure, Manage functions
- **DORA** : Digital Operational Resilience, third-party model risk
- Cross-framework regulatory comparison and policy-to-control mapping

### GenAI Governance
- LangChain fundamentals and RAG (Retrieval Augmented Generation)
- LLM risk taxonomy: hallucination, bias, prompt injection, non-determinism
- GenAI governance framework and controls

-----

## Repository Structure

```
ai-governance-architect-lab/
├── data/               ← Datasets (German Credit dataset and monitoring samples)
├── notebooks/          ← Jupyter notebooks organised by topic
├── docs/               ← Governance documents, framework notes, and model artifacts
├── src/                ← Reusable Python modules (metrics, monitoring, explainability, fairness)
└── architecture/       ← Architecture diagrams and enterprise governance design docs
```

-----

## Key Governance Artifacts

| Document | Description |
|----------|-------------|
| `docs/model_validation_framework.md` | Full model validation framework (conceptual soundness, outcome analysis, monitoring) |
| `docs/regulatory_comparison.md` | SR 11-7 vs SS1/23 vs EU AI Act vs NIST AI RMF vs DORA comparison |
| `docs/model_documentation_template.md` | Reusable model documentation template |
| `docs/governance_architecture.md` | Enterprise AI governance architecture with policy-to-control mapping |
| `docs/fairness_analysis.md` | Bias and fairness analysis across demographic groups |
| `docs/llm_governance_framework.md` | GenAI/LLM governance framework |
| `architecture/enterprise_ai_governance.md` | Enterprise-level AI governance blueprint |

-----

## Technical Stack

| Area | Tools |
|------|-------|
| Data & Modelling | Python, pandas, numpy, scikit-learn, scipy, statsmodels |
| Explainability | SHAP |
| Experiment Tracking | MLflow |
| Model Monitoring | Evidently AI |
| GenAI | LangChain |
| Version Control | Git, GitHub |
| Development | VS Code, Jupyter Lab |

-----

## Regulatory Frameworks

| Framework | Jurisdiction | Focus |
|-----------|-------------|-------|
| SR 11-7 | United States (Federal Reserve) | Model Risk Management |
| SS1/23 | United Kingdom (Bank of England) | Model Risk Management |
| EU AI Act | European Union | AI Risk Classification & Obligations |
| NIST AI RMF | United States (NIST) | AI Risk Management |
| DORA | European Union | Digital Operational Resilience |

-----

## Dataset

The primary dataset used throughout this lab is the **German Credit Dataset** (UCI Machine Learning Repository) : a widely used benchmark dataset in credit risk modelling, containing 1,000 applicants classified as good or bad credit risk across 20 features.
