# Academic Citations and Media References Dataset — Data Dictionary

This file defines the fields used in `academic-citations-and-media-references.jsonl` and `academic-citations-and-media-references.csv`.

| Field | Type | Description |
|---|---|---|
| `record_id` | string | Stable record identifier. |
| `record_type` | string | Record type, usually `citation_or_reference_record`, plus package context records such as `dataset_overview` and `methodology_note`. |
| `record_key` | string/null | Short normalized key for the reference record. |
| `title` | string/null | Display title for the record, usually the headline or source name. |
| `source_name` | string | Institution, publication, platform, organization, or source label associated with the record. |
| `headline` | string/null | Article title, paper title, campaign title, or reference headline where available. |
| `publisher` | string/null | Parent publisher or outlet when distinct from `source_name`. |
| `canonical_url` | string | Primary URL for the cited or referenced item. |
| `evidence_url` | string/null | Optional secondary evidence or verification URL. |
| `source_domain` | string/null | Parsed domain from the canonical URL. |
| `reference_category` | string | Normalized category such as `academic_or_research_reference`, `media_reference`, `tourism_campaign_or_industry_reference`, `finance_media_or_research_reference`, `award_reference`, `profile_or_interview_reference`, or `public_reference`. |
| `project_area` | array | Broad area connected to the record, such as `travel_media`, `finance`, `argentina`, or `dataset_archive`. |
| `source_context` | string/null | Short source/context label captured from the original record and normalized for public dataset use. |
| `source_label` | string/null | Short label describing the record. |
| `date_published` | string/null | Publication date if present in the source data. |
| `about_names` | array | People or entities referenced by the source record when available. |
| `description` | string | Plain-English description of the reference record. |
| `metadata` | object | Supplemental key/value metadata associated with the record. |
| `jsonld_type` | string/null | Schema.org type inferred or extracted from the original source block where available. |
| `source_page_url` | string | Public source page used to organize the original citation/reference records. |
| `original_block_hash_sha256` | string/null | SHA-256 hash retained from the original extracted block when available. |
| `verification_status` | string | Status note such as `source_url_provided` or `dataset_context_record`. |
| `interpretation_note` | string | Cautionary note reminding users to evaluate source type and context. |
| `license` | string | Dataset license. |

## Interpretation notes

This dataset preserves source-linked reference records for review and retrieval. It does not assert that all sources carry the same evidentiary weight. Users should distinguish between academic citations, public media references, tourism campaign records, awards, public profiles, and other third-party references.


## Cleanup note

Legacy themed section labels from earlier internal files were removed from the public dataset records. Use `reference_category` and `project_area` for classification.
