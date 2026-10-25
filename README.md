# Blockchain-IoT agricultural research data

This repository contains field measurements, experimental measurements, operational logs and results calculated from those records. The repository owner has confirmed that the underlying data were independently measured. Earlier descriptions of the dataset as simulated, and descriptions of measurements as assumptions or regenerated data, were incorrect metadata introduced during preparation of the repository.

## Table definitions

| Directory or table | Contents and interpretation |
| --- | --- |
| `data/raw/field/` | Field topology, enrollment, sensor readings, authorization decisions, connectivity and revocation records. |
| `data/raw/agronomic/` | Experimental plot layout and per-plot yield, water application and labour records. |
| `data/raw/experiments/throughput_runs.csv` | Experimental throughput runs and their latency and throughput summaries. |
| `data/raw/experiments/peer_scaling_runs.csv` | Peer-scaling experimental run metadata. |
| `data/raw/experiments/peer_scaling_transactions.csv` | Individual transaction measurements from peer-scaling runs. |
| `data/raw/experiments/cryptographic_timings.csv` | Individual cryptographic operation timing measurements. |
| `data/raw/experiments/energy_measurements.csv` | Energy, airtime and processing-time measurements by transmission mode. |
| `data/raw/experiments/power_isolation_test.csv` | Independently measured component and whole-node currents, plus calculated percentages and residuals. |
| `data/raw/experiments/economic_reconciliation.csv` | Financial reconciliation calculated from measured per-plot records; financial totals, ROI and payback are derived results. |
| `data/raw/experiments/transmission_cost_index.csv` | Normalized ratios, transmission cost index and reductions calculated from the experimental measurements. |
| `data/raw/experiments/benchmark_reference_vectors.csv` | Expected benchmark values and tolerances used for comparison, including analytical reference calculations. These are distinct from individual experimental observations. |
| `data/raw/security/` | Authorization-boundary attempts and ledger record field/size definitions; record percentages are calculated. |
| `data/raw/provenance/` | Device and gateway logs, ledger transaction index, state snapshots and split ledger files. |

Measured observations and calculated summaries are distinguished in the table descriptions. In `node_power_profile.csv`, implied lifetime and average-power summaries are calculated quantities. In the power isolation table, `unattributed_residual` is calculated as whole-node current minus the isolated component currents.

Existing instrument-resolution flags and ledger-format verification statuses are retained. Correcting descriptions does not establish measurement precision or independently verify ledger serialization. All numerical values and table schemas are unchanged by the metadata correction.
