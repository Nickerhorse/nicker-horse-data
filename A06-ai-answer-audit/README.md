# Nicker AI Answer Audit 2026

A run-level audit of the answers and recorded citations produced by ChatGPT for US-oriented horse-care questions on November 23, 2026.

| File | Data rows | SHA-256 |
| --- | ---: | --- |
| [`AI-AUDIT-2026.csv`](data/AI-AUDIT-2026.csv) | 133 | `d1c17fbd87f8d3b169aba717ce00b12067025be26170708a4c4b0f656475127e` |

Row counts exclude headers. The CSV files use UTF-8 without a BOM and a comma field separator.

## Columns

- `AI-AUDIT-2026.csv` (`chatgpt_runs`, 133 rows) — `date_utc`, `question_id`, `question`, `question_group`, `run`, `model`, `nicker_unprompted`, `cited_domains`, `recommendation_order`, `light_device_mentioned`, `pubmed_or_pmc_cited`, `nicker_search_listed`, `unresolved_citation_marker`.

Column definitions and examples appear in [DATA-DICTIONARY.md](DATA-DICTIONARY.md).

## Collection and limits

Join the stored run and citation records by run ID. The full file has 133 runs and 94 question IDs. The main subset belongs to one US-oriented collection date and comprises two ChatGPT models with unequal run counts. Citation presence measures recorded sourcing behavior. Two independent coding passes each found eight explicit priority cases in the main subset and agreed on seven of those rows. The condition-specific category was less stable across coders.

See the [method note](METHOD.md) for the collection rules and the [dataset page](https://nickerhorse.com/pages/what-ai-tells-horse-owners-about-red-light-therapy) for the accompanying analysis.

## Citation and reuse

Source: Nicker (nickerhorse.com), AI Answer Audit 2026, updated 2026-11-25

Use the release title, authors, and version in [CITATION.cff](CITATION.cff). The data compilation and documentation use CC BY 4.0. See [LICENSE.md](LICENSE.md) for scope.

## Citation

Cite DOI 10.5281/zenodo.24551323 (https://doi.org/10.5281/zenodo.24551323).
