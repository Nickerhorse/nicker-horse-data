# Nicker Equine Light Therapy Evidence Map 2026

A study inventory and cross-tabulation for light-based interventions and measurements in live horses. It separates literature found through database queries from additional studies located in a review.

| File | Data rows | SHA-256 |
| --- | ---: | --- |
| [`EVIDENCE-STUDIES-2026.csv`](data/EVIDENCE-STUDIES-2026.csv) | 35 | `51d50d219a59bbf90e4bb4a27cbfea06dc806dd61886acdd368fcc0da2aee251` |
| [`EVIDENCE-MAP-2026.csv`](data/EVIDENCE-MAP-2026.csv) | 25 | `bb842e458e58360e41740ab1e3f004d22ee6afa0c7a82b847b47272c6cdfdb7d` |

Row counts exclude headers. The CSV files use UTF-8 without a BOM and a comma field separator.

## Columns

- `EVIDENCE-STUDIES-2026.csv` (`study_records`, 35 rows) — `study_id`, `pmid`, `linked_publication_pmid`, `publication_year`, `journal`, `study_title`, `study_design`, `modality`, `wavelength_nm`, `tissue_region`, `hoof_or_lower_leg`, `hoof_tissue`, `horse_count`, `control_group`, `author_reported_result`, `limited_source_detail`, `source_url`, `collected_date`, `source_record_id`, `study_set`.
- `EVIDENCE-MAP-2026.csv` (`evidence_counts`, 25 rows) — `study_set`, `tissue_region`, `led`, `low_power_laser`, `high_intensity_laser`, `co2_laser`, `laser_class_unreported`, `modality_unreported`, `total`.

Column definitions and examples appear in [DATA-DICTIONARY.md](DATA-DICTIONARY.md).

## Collection and limits

Search PubMed and Europe PMC, then screen titles and abstracts for relevant original work in live horses. The data map covers 30 independent studies from the database search plus five additional entries sourced through a review. Access depth and detail vary by record. The cross-tab includes a search-only block and an expanded block that already contains the search-only rows. Use one block at a time and exclude its total row when aggregating the detail. Study counts describe research coverage and cannot establish an intervention effect.

See the [method note](METHOD.md) for the collection rules and the [dataset page](https://nickerhorse.com/pages/equine-light-therapy-evidence-map-2026) for the accompanying analysis.

## Citation and reuse

Source: Nicker (nickerhorse.com), Equine Light Therapy Evidence Map 2026, updated 2026-11-25

Use the release title, authors, and version in [CITATION.cff](CITATION.cff). The data compilation and documentation use CC BY 4.0. See [LICENSE.md](LICENSE.md) for scope.

## Citation

Cite DOI 10.5281/zenodo.24551009 (https://doi.org/10.5281/zenodo.24551009).
