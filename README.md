# SENTINEL-X: AI Early-Warning Chain

**IBM Z Datathon 2026 | IBM LinuxONE**

## Problem Statement

Cybersecurity incidents can develop through weak signals distributed across authentication, business transactions, API activity, and resource-access systems. Analyzing these events independently can make coordinated suspicious activity difficult to identify.

## Our Solution

SENTINEL-X is a prototype that analyzes synthetic cybersecurity events, assigns heuristic signal points, and correlates suspicious activity across systems using account identifiers and time windows.

It generates candidate alerts and provides evidence to help investigators understand the signals behind them.

## Key Features

- Multi-source event analysis
- Data quality validation
- Rule-based security-signal scoring
- Cross-system time-window correlation
- Candidate-alert consolidation
- Incident timelines and correlation visualizations
- Ground-truth comparison and evidence summaries

## Technology Stack

- Python
- Pandas and NumPy
- Matplotlib
- JupyterLab
- IBM LinuxONE

## Repository Contents

- `zpulse.ipynb` — analysis, correlation, evaluation, and visualizations
- CSV files — synthetic security events and incident ground truth
- `sentinel_x_results/` — exported evaluation results, if included

## Execution

The notebook was executed in JupyterLab in an IBM LinuxONE environment. Open the notebook and run its cells in order, ensuring that the CSV files are available at the expected paths.

## Limitations

This is a rule-based prototype evaluated on synthetic data. Candidate alerts and account-level coverage do not establish real-world detection accuracy. Further evaluation is needed before production use.

## Future Work

- Refine correlation rules and reduce false positives
- Perform rigorous incident-level evaluation
- Integrate and validate additional detection modules
- Explore trained machine-learning models where justified by the data
