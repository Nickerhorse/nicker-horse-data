# Data dictionary for Hoof & Leg Problem Stats

Fields below follow the public CSV schema. An ellipsis marks an abbreviated example. A dash in the unit column indicates a dimensionless or inapplicable unit.

## STATS-HOOF-LEG-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `record_id` | text | — | Stable statistic record identifier | S001 |
| `topic` | category | — | Hoof or leg topic of the observation | abscess |
| `value` | text | see unit | Reported or calculated value with any qualifier | 160 |
| `unit` | text | row-specific | Meaning and units of the value | cases |
| `population_scope` | text | — | Geography, population, denominator, and time window when available | Retrospective cohort of subsolar abscess patients from Penn New Bolton Center Field… |
| `source` | text | — | Research publication, report, or calculation source | Cole et al. Vet Rec PubMed 30514742 |
| `source_year` | text | as recorded | Year attached to the underlying data or source | 2019 |
| `publication_year` | text | as recorded | Publication year or publication date | 2019 |
| `evidence_type` | category | — | Distinguishes sourced findings, calculations, and scoped absence records | source_reported |
| `source_material` | text | — | Primary material or portion of the source inspected | PubMed abstract (E-utilities) |
| `checked_date` | text | ISO dates | Date or dates on which the source was checked | 2026-11-24 |
| `source_excerpt` | text | — | Evidence excerpt or calculation trail | Descriptive statistics were performed on data collected from 160 cases of equine… |
| `scope_notes` | text | — | Limits, denominators, or qualifications recorded with the observation | One clinic population. |
