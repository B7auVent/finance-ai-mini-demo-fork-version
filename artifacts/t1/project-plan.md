# T1 Project Plan

## Project Goal

Develop a clear and reproducible research workflow for comparing three familiar asset classes:

- `SPY` — US equities
- `TLT` — long-term US Treasury bonds
- `GLD` — gold

The comparison is based on an illustrative, fixed ETF dataset so the work can focus on project versioning, AI-assisted analysis, verification, and agent collaboration rather than data collection.

## Available Data

`data/etf_snapshot.csv` is a small, fixed dataset with one row per ETF. The dataset is synthetic teaching data, not live or historical market observations. Each row contains:

| Column | Meaning |
|---|---|
| `ticker` | Short identifier for the illustrative ETF |
| `asset_class` | Broad type of asset represented by the ETF |
| `expected_return_pct` | Illustrative annual return assumption (%) |
| `volatility_pct` | Illustrative annual variability assumption (%) |
| `max_drawdown_pct` | Illustrative largest peak-to-trough loss (%); negative values represent losses |
| `expense_ratio_pct` | Illustrative annual fund fee (% of invested assets) |

## Expected Final Deliverable

A reproducible analysis workflow that compares the three ETFs on risk, return, and cost using the synthetic snapshot data. The final deliverable is planned to include a written summary of findings, supporting tables or figures, and the steps needed to reproduce the analysis.

## Three Project Milestones

1. **T1 — Project setup**: Review the repository and data dictionary, and create this initial project plan.
2. **T2 — Analysis design**: Define a bounded analysis task (planned work) using the snapshot data, including which metrics to compute and how to compare the three ETFs.
3. **T3 — Agent workflow**: Organize a verifiable agent workflow (planned work) that executes the analysis, verifies results, and produces the final deliverable.

## One Data Limitation

All numeric values in `data/etf_snapshot.csv` are synthetic teaching assumptions. They are not current quotations, verified historical estimates, or forecasts, and the dataset omits correlations, taxes, transaction costs, liquidity, currency exposure, and investor-specific constraints. The dataset must not be used as investment advice or as the basis for a real investment decision.

## Next Action

Review this project plan and save it with Git as part of the T1 deliverable. The next tutorial step will be to design the bounded analysis task on top of this repository.
