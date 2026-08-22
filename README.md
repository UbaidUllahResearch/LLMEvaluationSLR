# LLM Evaluation Systematic Literature Review (SLR)

## Overview

This repository contains the replication package for the systematic literature review on large language model (LLM) evaluation methodologies, encompassing 295 studies across Software Engineering, Cybersecurity, and Computer Science. The repository provides all artifacts necessary to reproduce the analyses, verify the findings, and extend the research.

## Repository Structure

| **File Name** | **Records** | **Description** |
|---------------|-------------|-----------------|
| `SpreadSheet-01--04.xlsx` | — | Raw search results and extracted metadata from Google Scholar, IEEE Xplore, ACM Digital Library, and ScienceDirect. |
| `SpreadSheet-05.xlsx` | 2,006 | Records retained after initial relevance filtering based on title, abstract, and keyword screening. |
| `SpreadSheet-06.xlsx` | 692 | Records remaining after title and abstract screening against predefined inclusion/exclusion criteria. |
| `Final_Dataset.xlsx` | 295 | The final curated corpus of 295 studies selected through consensus and team review, forming the basis for all analyses presented in the paper. |

## Screening Progression

The reduction from 2,006 to 295 studies reflects a deliberate, precision-oriented screening strategy:
- **Broad initial search:** Maximized recall to avoid missing relevant work
- **Progressive filtering:** Title/abstract screening → full-text assessment → consensus-based selection
- **Final corpus:** 295 studies balancing breadth and analytical rigor

## Analytical Scripts

Python scripts used to generate the quantitative analyses and figures reported in the paper are available in the `scripts/` directory:

- Data extraction and preprocessing
- Statistical analysis and visualization
- Taxonomy classification and overlap analysis

## Citation Source

Citation counts for preprints were obtained from Google Scholar, collected on August 15, 2025, to ensure temporal consistency. Preprints were included only if they had at least ten citations, balancing timeliness with scholarly validation.

## Usage

To reproduce the analyses:

The intermediate spreadsheets (SpreadSheet-01–06) contain evolving records and screening decisions developed as internal research artifacts. While included for transparency, they are not intended as a standalone replication package. The final curated dataset (`Final_Dataset.xlsx`) is the primary resource for verification and reuse.

## Contact

For questions or feedback, please contact the corresponding author.

---

**Repository:** https://github.com/UbaidUllahResearch/LLMEvaluationSLR
