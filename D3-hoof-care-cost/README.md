# Nicker US Hoof Care Cost 2026

A US hoof-care cost table combining survey figures, published clinic fees, selected retail observations, and calculations. The companion JSON carries routine farrier budgeting inputs.

| File | Data rows | SHA-256 |
| --- | ---: | --- |
| [`COST-HOOF-CARE-2026.csv`](data/COST-HOOF-CARE-2026.csv) | 31 | `200a723630fbdd8a546cbeee4ebc4faf0f3bd47e2f9602143f486d2f595e723e` |
| [`cost-inputs.json`](data/cost-inputs.json) | — | `6f2233185abfd13bbc6aa46393a995d110ee803ebdf30cdd6d40a2dab9cc8c2c` |

Row counts exclude headers. The CSV files use UTF-8 without a BOM and a comma field separator.

## Columns

- `COST-HOOF-CARE-2026.csv` (`cost_observations`, 31 rows) — `record_id`, `item`, `value`, `unit`, `scope`, `source`, `data_year`, `evidence_type`, `source_excerpt`, `scope_notes`.

Column definitions and examples appear in [DATA-DICTIONARY.md](DATA-DICTIONARY.md).

## Collection and limits

Keep each observation with its service definition, billing unit, and scope. Routine-care scenarios depend on the chosen interval and service. Clinic and retail observations come from selected sources and can change. The clinic component examples do not estimate a complete hoof abscess episode or a US average. The JSON was dated November 24 and concerns recurring farrier inputs.

See the [method note](METHOD.md) for the collection rules and the [dataset page](https://nickerhorse.com/pages/cost-of-horse-leg-and-hoof-care-per-year) for the accompanying analysis.

## Citation and reuse

Source: Nicker (nickerhorse.com), US Hoof Care Cost 2026, updated 2026-11-25

Use the release title, authors, and version in [CITATION.cff](CITATION.cff). The data compilation and documentation use CC BY 4.0. See [LICENSE.md](LICENSE.md) for scope.

## Citation

Cite DOI 10.5281/zenodo.24550912 (https://doi.org/10.5281/zenodo.24550912).
