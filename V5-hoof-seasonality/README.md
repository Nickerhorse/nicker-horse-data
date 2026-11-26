# Nicker Hoof Problem Seasonality Index 2026

US Google Trends summaries for hoof and leg search terms, plus a separate state ranking for the query “hoof abscess.” The monthly table lets readers compare each query against its own average.

| File | Data rows | SHA-256 |
| --- | ---: | --- |
| [`SEASONALITY-HOOF-2021-2026.csv`](data/SEASONALITY-HOOF-2021-2026.csv) | 13 | `c7674b2c9842c389b5ede6e81696b6608e0d86d361c21df2c4246ef6bfc7d572` |
| [`STATE-HOOF-ABSCESS-2021-2026.csv`](data/STATE-HOOF-ABSCESS-2021-2026.csv) | 51 | `b4e0b41c1147c71c2a7231d1386bbc4bb98c05ccae1450e11fe3f7c32b3242e4` |
| [`V5-seasonality-heatmap.svg`](data/V5-seasonality-heatmap.svg) | — | `5ad379a2c5321eeb51c091f7089f8cf4669a64f30a9ce5e851a919e4099661db` |

Row counts exclude headers. The CSV files use UTF-8 without a BOM and a comma field separator.

## Columns

- `SEASONALITY-HOOF-2021-2026.csv` (`monthly_index`, 13 rows) — `search_term`, `period`, `month_count`, `zero_month_count`, `data_status`, `index_jan`, `index_feb`, `index_mar`, `index_apr`, `index_may`, `index_jun`, `index_jul`, `index_aug`, `index_sep`, `index_oct`, `index_nov`, `index_dec`, `peak_month`, `peak_above_mean_pct`, `trough_month`, `trough_below_mean_pct`, `relative_series_mean`.
- `STATE-HOOF-ABSCESS-2021-2026.csv` (`state_interest`, 51 rows) — `rank`, `state`, `relative_interest`, `search_term`, `scope`, `collected_date`, `score_notes`.

Column definitions and examples appear in [DATA-DICTIONARY.md](DATA-DICTIONARY.md).

## Collection and limits

Group the source observations by calendar month. Monthly and state scores use different reference points. They measure relative search interest and cannot be interpreted as case counts, prevalence, or search volume. Sparse series retain their calculated values and carry a flag for filtering. A blank state score is distinct from zero interest. The monthly CSV contains 13 terms.

See the [method note](METHOD.md) for the collection rules and the [dataset page](https://nickerhorse.com/pages/horse-hoof-and-leg-health-statistics) for the accompanying analysis.

## Citation and reuse

Source: Nicker (nickerhorse.com), Hoof Problem Seasonality Index 2026, updated 2026-11-24

Use the release title, authors, and version in [CITATION.cff](CITATION.cff). The data compilation and documentation use CC BY 4.0. See [LICENSE.md](LICENSE.md) for scope.

## Citation

Cite DOI 10.5281/zenodo.24551183 (https://doi.org/10.5281/zenodo.24551183).
