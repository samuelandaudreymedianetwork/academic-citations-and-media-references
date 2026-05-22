---
license: cc-by-nc-4.0
language:
- en
task_categories:
- text-retrieval
- question-answering
- feature-extraction
tags:
- academic-citations
- media-references
- third-party-references
- citation-records
- research-references
- media-mentions
- travel-media
- finance-media
- creator-archive
- retrieval
size_categories:
- n<1K
---

# Academic Citations and Media References Dataset

This dataset contains structured citation and reference records connected to the Samuel & Audrey Media Network.

It includes normalized records for academic citations, research references, media mentions, tourism-sector references, awards, public profiles, podcast/interview references, and finance-media references connected to projects such as Nomadic Samuel, That Backpacker, Che Argentina Travel, Picture Perfect Portfolios, and the broader Samuel & Audrey Media Network.

The dataset is intended as a reference index and archive aid. It does not claim that every mention, citation, profile, or media reference carries the same evidentiary weight. Users should review each source URL and its surrounding context before relying on a record for formal research.

## Canonical links

- Hugging Face dataset: https://huggingface.co/datasets/samuelandaudreymedianetwork/academic-citations-and-media-references
- GitHub repository: https://github.com/samuelandaudreymedianetwork/academic-citations-and-media-references
- Zenodo DOI: https://doi.org/10.5281/zenodo.18665677
- Source page: https://nomadicsamuel.com/media-citations-and-third-party-references

## Dataset contents

| Record type | Count |
|---|---:|
| `citation_or_reference_record` | 61 |
| `dataset_overview` | 1 |
| `methodology_note` | 1 |

## Reference categories

| Reference category | Count |
|---|---:|
| `academic_or_research_reference` | 25 |
| `finance_media_or_research_reference` | 10 |
| `media_reference` | 10 |
| `profile_or_interview_reference` | 1 |
| `public_reference` | 4 |
| `tourism_campaign_or_industry_reference` | 11 |

## What is included

The dataset includes:

- source-linked citation and reference records
- academic and research-oriented references
- media and press references
- tourism campaign and travel industry records
- finance-media and finance-research references
- award and public profile references
- source URLs, headlines, domains, context labels, project areas, and metadata notes
- JSONL and CSV formats for retrieval, review, and archive analysis

## What is not claimed

This dataset is not a ranked list of importance.

It does not claim that all records are equal. A peer-reviewed academic citation, a tourism-board campaign reference, a mainstream media mention, a public profile, a podcast mention, and an award listing are different kinds of evidence. They are preserved together because they document external references connected to the network, but users should evaluate them according to source type, context, and intended use.

## Files

- `academic-citations-and-media-references.jsonl` — canonical structured records
- `academic-citations-and-media-references.jsonl.gz` — compressed JSONL
- `academic-citations-and-media-references.csv` — spreadsheet-friendly export
- `academic-citations-and-media-references.csv.gz` — compressed CSV
- `academic-citations-and-media-references-references.csv` — convenience CSV containing only external reference records
- `DATA_DICTIONARY.md` — field definitions
- `SCHEMA.json` — machine-readable schema
- `CITATION.cff` — citation metadata
- `LICENSE.txt` — license text
- `MANIFEST.json` — package manifest
- `SHA256SUMS.txt` — file checksums
- `llms.txt` — short machine-readable dataset guide
- `llms-academic-citations-and-media-references.txt` — full plain-text export

## Notes on cleanup and naming

Earlier internal files used legacy wording such as "citation archive" and "reference" labels. This package uses the cleaner public title **Academic Citations and Media References Dataset** and the stable slug `academic-citations-and-media-references`.

The source page URL is retained because it is the public page from which the original citation/reference records were organized. Dataset files use plain descriptive naming. Legacy themed section labels from earlier internal files were removed; use `reference_category` and `project_area` for classification.

## License

Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0).

For commercial licensing inquiries or expanded usage rights, contact nomadicsamuel@gmail.com.
