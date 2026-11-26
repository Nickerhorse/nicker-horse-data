# Data dictionary for Hoof Problem Seasonality Index

Fields below follow the public CSV schema. An ellipsis marks an abbreviated example. A dash in the unit column indicates a dimensionless or inapplicable unit.

## SEASONALITY-HOOF-2021-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `search_term` | text | — | Google Trends search term | hoof abscess |
| `period` | text | date range | Monthly observation window | 2021-11-01…2026-11-01 |
| `month_count` | integer | months | Number of monthly observations in the input series | 61 |
| `zero_month_count` | integer | months | Months reported as zero in that series | 0 |
| `data_status` | category | — | Whether the series had sufficient information for an index | sufficient |
| `index_jan` | integer | index points | January average relative to the term's overall monthly average | 81 |
| `index_feb` | integer | index points | February average relative to the term's overall monthly average | 81 |
| `index_mar` | integer | index points | March average relative to the term's overall monthly average | 93 |
| `index_apr` | integer | index points | April average relative to the term's overall monthly average | 96 |
| `index_may` | integer | index points | May average relative to the term's overall monthly average | 97 |
| `index_jun` | integer | index points | June average relative to the term's overall monthly average | 103 |
| `index_jul` | integer | index points | July average relative to the term's overall monthly average | 117 |
| `index_aug` | integer | index points | August average relative to the term's overall monthly average | 126 |
| `index_sep` | integer | index points | September average relative to the term's overall monthly average | 120 |
| `index_oct` | integer | index points | October average relative to the term's overall monthly average | 105 |
| `index_nov` | integer | index points | November average relative to the term's overall monthly average | 99 |
| `index_dec` | integer | index points | December average relative to the term's overall monthly average | 82 |
| `peak_month` | text | month label | Peak calendar month recorded for the indexed series | Aug |
| `peak_above_mean_pct` | integer | percent | Amount by which the peak exceeds the baseline | 26 |
| `trough_month` | text | month label | Low month or grouped low period | Dec–Feb |
| `trough_below_mean_pct` | integer | percent | Amount by which the low point falls below the baseline | 19 |
| `relative_series_mean` | decimal | relative Trends points | Mean of the normalized input series before calendar-month rescaling | 16.0 |

## STATE-HOOF-ABSCESS-2021-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `rank` | integer | rank | Display rank where Google Trends supplied a score | 1 |
| `state` | text | — | US state or District of Columbia | Wyoming |
| `relative_interest` | integer | relative Trends points | Relative query share with the highest-scoring state set to 100 | 100 |
| `search_term` | text | — | Search term used in the regional extract | hoof abscess |
| `scope` | text | date range and geography | Coverage of the one-term Google Trends state extract | US Google Trends regional interest for one search term, 2021-11-24 to 2026-11-24 |
| `collected_date` | date | YYYY-MM-DD | Date the regional extract was collected | 2026-11-24 |
| `score_notes` | text | — | Interpretation of the score or reason it is blank | The state with the highest share of searches for the term is scaled to 100. Scores… |
