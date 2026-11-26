# Data dictionary for Equine Light Therapy Evidence Map

Fields below follow the public CSV schema. An ellipsis marks an abbreviated example. A dash in the unit column indicates a dimensionless or inapplicable unit.

The study table uses publication titles as recorded. The counts table has a separate block for each study set, including a total row within each block.

## EVIDENCE-STUDIES-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `study_id` | text | — | Stable study identifier | E01 |
| `pmid` | identifier | — | PubMed identifier for the main publication where available | 6633135 |
| `linked_publication_pmid` | identifier | — | Linked report of the same experiment where applicable | 35008124 |
| `publication_year` | integer | year | Publication year | 1983 |
| `journal` | text | — | Publication venue | Lasers Surg Med |
| `study_title` | text | — | Publication title | A study of the effects of lasering on chronic bowed tendons at Wheatley Hall Farm… |
| `study_design` | category | — | Study design or evidence type recorded during screening | uncontrolled_series |
| `modality` | category | — | Light device or source classification | laser_class_unreported |
| `wavelength_nm` | text | nm | Reported wavelengths with any qualifiers | 904 |
| `tissue_region` | category | — | Anatomical site or tissue group | tendon |
| `hoof_or_lower_leg` | category | 0, 1, or undetermined | Whether a hoof or lower-leg site was identified | 1 |
| `hoof_tissue` | indicator | 0 or 1 | Hoof-tissue flag | 0 |
| `horse_count` | integer | horses | Reported count of live horses in the study when recoverable | 42 |
| `control_group` | category | yes or no | Whether a comparator was recorded | no |
| `author_reported_result` | category | — | Direction or nature of the result as reported by the authors | unreported |
| `limited_source_detail` | indicator | 0 or 1 | Flags records characterized from the available title-level information | 0 |
| `source_url` | URL | — | Address of the publication or evidence record | https://pubmed.ncbi.nlm.nih.gov/6633135/ |
| `collected_date` | date | YYYY-MM-DD | Date the study record was captured | 2026-11-24 |
| `source_record_id` | identifier | — | Identifier linking the study to its source record | 6633135 |
| `study_set` | category | — | Database-search or review-sourced provenance | search |

## EVIDENCE-MAP-2026.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `study_set` | category | — | Counting scope for the search-only or expanded view | search |
| `tissue_region` | category | — | Anatomical grouping or the corresponding block total | tendon |
| `led` | integer | studies | Studies coded as LED | 0 |
| `low_power_laser` | integer | studies | Studies coded as low-power laser | 1 |
| `high_intensity_laser` | integer | studies | Studies coded as high-intensity laser | 4 |
| `co2_laser` | integer | studies | Studies coded as defocused carbon dioxide laser | 0 |
| `laser_class_unreported` | integer | studies | Studies identifying laser without a power classification | 1 |
| `modality_unreported` | integer | studies | Studies without a recorded light source classification | 1 |
| `total` | integer | studies | Total across modality columns for the indicated row | 7 |
