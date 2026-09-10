# Mistral-7B-v0.3 results

Evaluation of CORE-FV against the AIE baseline on `mistralai/Mistral-7B-v0.3`.
Each method was run with three seeds (42, 43, 44).

## Aggregated results (mean ± std over seeds)

| Model | Method | Antonymy | Capitalize | Present-Past | Singular-Plural | Country-Capital | English-French | Avg. |
|---|---|---|---|---|---|---|---|---|
| Mistral-7B-v0.3 | AIE | 84.92 ± 1.68 | 100.00 ± 0.00 | 95.44 ± 2.64 | 99.17 ± 1.44 | 92.50 ± 6.00 | 85.95 ± 0.24 | 93.00 ± 0.23 |
| Mistral-7B-v0.3 | CORE-FV | 83.05 ± 2.45 | 98.98 ± 1.27 | 96.59 ± 1.70 | 95.89 ± 3.74 | 97.06 ± 2.94 | 87.96 ± 1.38 | 93.25 ± 1.24 |

Per-seed numbers are in [`results-summary.txt`](results-summary.txt); the formatted
table is in [`results-table.txt`](results-table.txt).

## Contents

| Path | Description |
|---|---|
| `results-summary.txt` | Per-seed accuracy per task, both methods |
| `results-table.txt` | Formatted mean ± std comparison table |
| `CoreFV_outputs/seed_42.ipynb`, `seed_43.ipynb` | CORE-FV run notebooks (seeds 42, 43) |
| `CoreFV_outputs/seed_44.zip` | CORE-FV seed 44: notebook, run log, and `outputs/` (function vectors, plots) |
| `AIE_outputs/seed_42.zip`, `seed_43.zip`, `seed_44.zip` | AIE baseline runs: notebook/log and `outputs/` per seed |

The numbers in the file names are the computation seeds.
