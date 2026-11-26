# Data dictionary for Horse Red Light Spec Index

Fields below follow the public CSV schema. An ellipsis marks an abbreviated example. A dash in the unit column indicates a dimensionless or inapplicable unit.

Seller excerpts record wording seen on dated listings. Bracketed ellipses mark editorial omissions. The coded flags describe what the observed pages disclosed.

## SPEC-INDEX-2026-11.csv

| Column | Type | Unit | Definition | Example |
| --- | --- | --- | --- | --- |
| `record_id` | text | — | Stable product record identifier | R01 |
| `brand` | text | — | Brand listed for the item | Northeast EquiWellness |
| `product_name` | text | — | Product or model name | GlowLine Bell Boot |
| `device_type` | category | — | Device or equipment form | hoof_and_pastern_bell_boot |
| `sales_unit` | text | — | Unit or grouping offered on the listing | 1 boot / pair |
| `single_price_usd` | text | USD | Observed single-item price, which may carry source or listing qualifiers | 149.00 |
| `bundle_price` | text | listing currency | Bundle amount and bundle size as recorded | pair 278.00 |
| `list_price` | text | listing currency | Reference or list amount and its package context | 1407.00 |
| `wavelengths_nm` | text | nm | Published wavelengths, including stated emitter configurations | 660 + 850 |
| `led_count` | text | emitters | Published LED count, which may include qualifiers | 80 |
| `irradiance_mw_cm2` | text | mW/cm² | Published irradiance value or range | 120 |
| `irradiance_conditions` | text | — | Stated location or conditions for the irradiance figure | not_published |
| `charge_time` | text | as stated | Full-charge time where documented | not_published |
| `battery` | text | as stated | Battery capacity, voltage, or run-time details as recorded | ≈1 hour of use (≈4 × 15 min) |
| `session_timer` | text | as stated | Session duration or timer and pulse settings | 15 min automatic timer · 10 Hz |
| `warranty_terms` | text | as stated | Terms associated with product defects or coverage | 1 year for manufacturing defects |
| `return_terms` | text | as stated | Return period and conditions recorded for the listing | 30 days |
| `return_shipping` | text | as stated | Notes on return postage or fees | not_published on product page (2026-11-17 policy: buyer pays for a change-of-mind… |
| `fit` | text | as stated | Listed fit, adjustment range, or dimensions | not_published |
| `source_url` | URL | — | Address of the source listing | https://www.northeastequiwellness.com/product-page/glowline-bell-boot-red-near-infra… |
| `checked_date` | text | ISO dates | Date or dates on which the source was checked | 2026-11-23 |
| `bundle_unit_price_usd` | text | USD per item | Recorded per-item amount for eligible bundles by size | pair 139.00 |
| `irradiance_distance` | text | as stated | Measurement distance with its publication status | not_published |
| `meter_model` | text | — | Meter description in the captured documentation | not_published |
| `fda_language` | category | — | Coding of statements about regulatory matters | not_published |
| `seller_health_claim` | category | yes or no | Whether captured language met the health-claim coding criterion | yes |
| `water_rating` | category | — | Coding of the stated classification for water exposure | not_published |
| `delivery_timing` | text | as stated | Recorded delivery timing information | not_published |
| `us_address_disclosed` | category | yes or no | Whether the reviewed listing disclosed a US address | no |
| `dispatch_origin_disclosed` | category | yes or no | Whether the reviewed listing disclosed a dispatch origin | no |
| `listing_notes` | text | — | Additional context about the seller disclosures | Free shipping. |
| `seller_health_claim_quote` | text | — | Excerpt of the seller's health claim | to assist healing of acute injuries and long term conditions of the hooves and… |
| `seller_health_statement_quote` | text | — | Seller statement about the evidence for clinical benefits | Specific clinical benefits of these boots have not been established. |
| `seller_delivery_quote` | text | — | Excerpt of the seller's estimated delivery or dispatch wording | Delivered |
| `seller_fda_quote` | text | — | Excerpt of the seller's FDA wording | These statements have not been evaluated by the Food and Drug Administration. |
| `seller_water_exposure_quote` | text | — | Excerpt of the seller's water-exposure wording | Do not use on a wet horse. |
| `seller_return_policy_quote` | text | — | Excerpt of the seller's return wording | You have 30 calendar days from the date of purchase (invoice) |
| `seller_us_location_quote` | text | — | US city and state displayed by the seller | Ocala, FL |
| `seller_irradiance_quote` | text | — | Excerpt of the seller's irradiance wording | Irradiance: 150mW/cm2 at surface |
| `seller_led_count_quote` | text | — | Excerpt of the seller's LED count wording | 110 LED diodes and 330 LED chips |
| `seller_disclosure_quote` | text | — | Excerpt of the seller's technical disclosure | Irradiance and EMF values have not been independently […] |
| `seller_quote_checked_date` | text | ISO dates | Date or dates of the checks that supplied the seller excerpts | 2026-11-23 |
