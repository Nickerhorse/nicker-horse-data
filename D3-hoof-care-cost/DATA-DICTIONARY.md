# Data dictionary for US Hoof Care Cost

Fields below follow the public CSV schema. An ellipsis marks an abbreviated example. A dash in the unit column indicates a dimensionless or inapplicable unit.

## COST-HOOF-CARE-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `record_id` | text | — | Stable cost or assumption identifier | C001 |
| `item` | text | — | Care item, fee, or modeled scenario | Four-hoof trim |
| `value` | text | see unit | Amount, range, schedule assumption, or descriptive result | 61 |
| `unit` | text | row-specific | Currency and billing basis or other row unit | USD / visit |
| `scope` | text | — | Applicable service, geography, sample, or scenario assumptions | US survey of full-time farriers, 2026 AFJ survey (604 responses from 8,991 emails,… |
| `source` | text | — | Identifies the source or component records | AFJ, 'Farrier Business Trends Reveal Shifting Priorities', M. Krueger, June 18,… |
| `data_year` | text | as recorded | Underlying data year when supplied | 2026 |
| `evidence_type` | category | — | Distinguishes attributed observations and calculations | source_reported |
| `source_excerpt` | text | — | Supporting excerpt or calculation expression | A trim costs a client $61, a trim and four keg shoes $184 and a trim and a full… |
| `scope_notes` | text | — | Scope qualifications and interpretation notes | National average. Far West $75 and Central $54 (AFJ What Farriers Are Charging,… |

## cost-inputs.json

| Field | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `source` | string | — | CSV supplying the modeled parameters | COST-HOOF-CARE-2026.csv |
| `updated` | date | YYYY-MM-DD | Parameter snapshot date | 2026-11-24 |
| `trim_usd` | integer | USD per visit | Routine trim input | 61 |
| `trim_4keg_usd` | integer | USD per visit | Trim with four keg shoes input | 184 |
| `trim_reset_usd` | integer | USD per visit | Trim with full reset input | 178 |
| `region` | object | — | Regional values keyed by far_west and central | far_west |
| `region.*.trim` | integer | USD per visit | Regional trim input | 75 |
| `region.*.trim_4keg` | integer | USD per visit | Regional trim with four keg shoes input | 197 |
| `interval_weeks` | object | — | Interval bounds keyed by hoof-care scenario | barefoot |
| `interval_weeks.barefoot` | two integers | weeks | Minimum and maximum barefoot trim intervals | [6, 8] |
| `interval_weeks.shod` | two integers | weeks | Minimum and maximum shoeing intervals | [4, 6] |
| `source_text` | string | — | Source names supporting the parameters | AFJ 2026 Farrier Business Practices survey… |
