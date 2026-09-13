# Qwen2.5-7B results

Evaluation of CORE-FV against the AIE baseline on `Qwen/Qwen2.5-7B`.
Each method was run with three seeds (42, 43, 44).

## Aggregated results (mean ± std over seeds)

| Model | Method | Antonymy | Capitalize | Present-Past | Singular-Plural | Country-Capital | English-French | Avg. |
|---|---|---|---|---|---|---|---|---|
| Qwen2.5-7B | AIE | 83.67 ± 1.63 | 99.80 ± 0.35 | 98.86 ± 0.98 | 97.54 ± 2.44 | 92.67 ± 4.07 | 21.39 ± 22.32 | 82.32 ± 3.55 |
| Qwen2.5-7B | CORE-FV | 83.54 ± 2.56 | 100.00 ± 0.00 | 99.43 ± 0.99 | 97.54 ± 2.44 | 94.44 ± 0.15 | 88.15 ± 0.15 | 93.85 ± 0.61 |

AIE's English→French accuracy is unstable across seeds (7.65 / 9.38 / 47.15), while
CORE-FV stays consistent (88.04–88.32). Per-seed numbers are in
[`results-summary.txt`](results-summary.txt); the formatted table is in
[`results-table.txt`](results-table.txt).

## Contents

| Path | Description |
|---|---|
| `results-summary.txt` | Per-seed accuracy per task, both methods |
| `results-table.txt` | Formatted mean ± std comparison table |
| `CoreFV_outputs/seed_42.zip`, `seed_43.zip`, `seed_44.zip` | CORE-FV runs: results JSON, cache (function vectors, mean displacements), logs, and plots per seed |
| `AIE_outputs/seed_42.zip`, `seed_43.zip`, `seed_44.zip` | AIE baseline runs: results JSON, cache (function vectors, mean activations), logs, and plots per seed |

The numbers in the file names are the computation seeds.
