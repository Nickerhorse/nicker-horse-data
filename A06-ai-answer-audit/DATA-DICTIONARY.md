# Data dictionary for AI Answer Audit

Fields below follow the public CSV schema. An ellipsis marks an abbreviated example. A dash in the unit column indicates a dimensionless or inapplicable unit.

## AI-AUDIT-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `date_utc` | date | YYYY-MM-DD UTC | UTC date of the recorded run | 2026-11-23 |
| `question_id` | identifier | — | Shared question identifier across repeats | D2-G01 |
| `question` | text | — | Released question text, with editorial shortening marked where applicable | What is the best red light wrap for an older horse with stiff hocks on cold winter… |
| `question_group` | category | — | Dominant question topic or designated publisher probe group | lower_leg_and_rehab |
| `run` | identifier | — | Unique answer run with repeat suffix | D2-G01#1 |
| `model` | category | — | ChatGPT model recorded for the run | gpt-6-mini |
| `nicker_unprompted` | indicator | 0 or 1 | Whether the prompt omitted the publisher name and address | 1 |
| `cited_domains` | list of domains | pipe-delimited | Resolved cited domains, deduplicated within an answer | csuveterinaryhealth.org&#124;equusmagazine.com&#124;esc.rutgers.edu&#124;k8s-msu-msuprod2-d4425984b… |
| `recommendation_order` | category | — | Code describing whether the answer prioritized routine hoof care or made order conditional | no_explicit_priority |
| `light_device_mentioned` | indicator | 0 or 1 | Whether a light device met the mention criterion | 1 |
| `pubmed_or_pmc_cited` | indicator | 0 or 1 | Whether the run cited a recorded PubMed or PMC domain | 0 |
| `nicker_search_listed` | indicator | 0 or 1 | Whether the publisher appeared in the recorded search listing | 0 |
| `unresolved_citation_marker` | indicator | 0 or 1 | Whether an unresolved citation marker was recorded in the run | 0 |
