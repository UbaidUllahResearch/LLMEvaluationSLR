# LLM Evaluation Practices in Software Engineering, Cybersecurity, and Computer Science: A Systematic Literature Review

## 1. Overview

This repository contains the replication package for the systematic literature review (SLR) entitled **"LLM Evaluation Practices in Software Engineering, Cybersecurity, and Computer Science: A Systematic Literature Review."**

The study systematically investigates evaluation methodologies for Large Language Models (LLMs) across three research domains:

- Software Engineering (SE)
- Cybersecurity (CySec)
- Computer Science (CS)

The final review corpus comprises **295 primary studies**, which form the basis of the qualitative synthesis, methodological taxonomy, quantitative analysis, and discussion presented in the paper.

This repository provides the intermediate datasets, bibliographic records, final study corpus, and PRISMA flow diagram to support the transparency, verification, and reproducibility of the study selection and analysis process.

## 2. Repository Structure

The repository contains seven intermediate spreadsheets and the PRISMA flow diagram. Each spreadsheet corresponds to a particular stage of the search, screening, or study selection process.

| File Name | Records | Description |
|---|---:|---|
| `SpreadSheet-01.xlsx` | — | Search results and extracted bibliographic information from Google Scholar. |
| `SpreadSheet-02.xlsx` | — | Search results and extracted bibliographic information from IEEE Xplore. |
| `SpreadSheet-03.xlsx` | — | Search results and extracted bibliographic information from ACM Digital Library. |
| `SpreadSheet-04.xlsx` | — | Search results and extracted bibliographic information from ScienceDirect. |
| `SpreadSheet-05.xlsx` | 2,006 | Unique records retained after relevance assessment and duplicate removal. |
| `SpreadSheet-06.xlsx` | 692 | Studies retained after methodological eligibility assessment. |
| `SpreadSheet-07.xlsx` | 295 | Final corpus of primary studies included in the systematic literature review. |

The first four spreadsheets document the search results and associated bibliographic information from the selected digital libraries. The remaining spreadsheets represent the progressively refined datasets obtained during the study selection process.

## 3. Search and Study Selection Process

The systematic search was conducted using eight search-query variations across four digital libraries:

1. Google Scholar
2. IEEE Xplore Digital Library
3. ACM Digital Library
4. ScienceDirect

The search returned **1,198,779 raw records** across the four platforms. This figure represents the total number of search results reported by the digital libraries and should not be interpreted as the number of records individually examined by the researchers.

Given the exceptionally large retrieval volume, an initial manual screening strategy based on a saturation-based stopping rule was applied. Titles and abstracts were examined progressively, and screening for each query was discontinued when two consecutive result pages yielded no new relevant studies.

The subsequent study selection process comprised the following stages.

### 3.1. Initial Screening and Relevance Assessment

Following the initial search and saturation-based screening procedure, the retrieved records were consolidated for further relevance assessment.

A total of **10,079 records** were assessed to determine their relevance to LLM evaluation. Records were considered relevant if they included an evaluation component addressing LLM performance, capabilities, limitations, reliability, factuality, robustness, security, safety, alignment, reasoning, generation quality, code-related capabilities, hallucination, bias, toxicity, instruction following, efficiency, or evaluation methodology.

Studies focusing exclusively on the application of LLMs to downstream tasks without evaluating model performance or contributing to an evaluation methodology were excluded.

Following this assessment:

- Records assessed for relevance: **10,079**
- Records excluded as not relevant to LLM evaluation: **7,856**
- Records retained for further processing: **2,223**

### 3.2. Duplicate Identification and Removal

Duplicate identification and removal were conducted after the initial relevance assessment and before methodological eligibility screening.

This sequencing was adopted because the initial retrieval contained a substantial number of records that were subsequently excluded as irrelevant to the review. Performing duplicate detection across the entire raw retrieval set would therefore have required processing a considerably larger collection, including records that would not proceed to subsequent screening. Furthermore, duplicate identification involved manual verification to minimize the risk of removing distinct studies. Conducting this verification after the relevance assessment made the process more manageable while preserving the integrity of the retained records.

Duplicate detection was performed using Microsoft Excel. Potential duplicates were identified by sorting and filtering records according to their titles, with particular attention to differences in capitalization, punctuation, spacing, and formatting. Each flagged record was subsequently examined manually before removal.

Records were considered duplicates when they met one or more of the following criteria:

- Exact title match.
- Highly similar titles or minor formatting differences, referring to the same publication and confirmed through the first author's name and other bibliographic information.
- Identical DOI, where available.

The duplicate-removal process resulted in the following progression:

| Selection step | Number of records |
|---|---:|
| Records retained after relevance assessment | 2,223 |
| Duplicate records identified and removed | 217 |
| Unique records retained after duplicate removal | **2,006** |

Consequently, `SpreadSheet-05.xlsx` contains the **2,006 unique records** obtained after removing the 217 manually verified duplicates from the initial set of 2,223 records.

### 3.3. Methodological Eligibility Assessment

The 2,006 unique records were subsequently assessed against the methodological eligibility criteria of the review.

This assessment examined whether the studies made a substantive contribution to LLM evaluation methodologies. Relevant methodological aspects included evaluation objectives, assessment mechanisms, metrics, validation techniques, benchmarks, evaluation frameworks, experimental procedures, datasets, and empirical findings.

Studies in which evaluation was only incidental to an LLM-based application, or which did not make a substantive methodological contribution to LLM evaluation, were excluded.

The resulting selection was:

- Unique records assessed: **2,006**
- Studies excluded: **1,314**
- Studies retained for further assessment: **692**

The 692 retained studies were then examined against the predefined domain-specific eligibility criteria.

### 3.4. Domain-Specific Eligibility Assessment and Final Inclusion

The final eligibility assessment focused on studies primarily concerned with LLM evaluation within the predefined research domains of Software Engineering, Cybersecurity, and Computer Science.

Studies that did not primarily address LLM evaluation within these domains were excluded.

The final selection comprised:

- Studies assessed for domain-specific eligibility: **692**
- Studies excluded for not meeting the predefined domain criteria: **397**
- Final primary studies included: **295**

The resulting 295 studies constitute the final review corpus and provide the empirical foundation for the methodological synthesis, taxonomy construction, and analyses reported in the paper.

## 4. Relationship Between the Intermediate Datasets

The seven spreadsheets document the progression from the initial database searches to the final corpus. In particular, the relationship between the three refined datasets is as follows:

| Dataset | Number of records | Selection stage |
|---|---:|---|
| `SpreadSheet-05.xlsx` | 2,006 | Unique records after removing 217 duplicates from the 2,223 records retained after relevance assessment. |
| `SpreadSheet-06.xlsx` | 692 | Records retained after methodological eligibility assessment. |
| `SpreadSheet-07.xlsx` | 295 | Final studies retained after domain-specific eligibility assessment. |

Thus, the datasets represent successive stages of refinement rather than independent collections of studies.

The numerical progression is:

**2,223 records → 2,006 unique records → 692 studies → 295 final studies.**

This progression allows readers to understand how duplicate removal and the subsequent eligibility criteria contributed to the construction of the final review corpus.

## 5. Final Study Corpus and Research Analysis

`SpreadSheet-07.xlsx` contains the final 295 primary studies included in the systematic literature review.

These studies were examined to identify recurring evaluation objectives, assessment mechanisms, validation procedures, datasets, and methodological characteristics.

Based on an inductive qualitative analysis of the final corpus, four principal evaluation paradigms were identified:

1. **Human Evaluation**
2. **Automated Evaluation**
3. **Adversarial Evaluation**
4. **Benchmark-Driven Evaluation**

The taxonomy and its 23 subcategories were derived from recurring methodological patterns identified in the included studies rather than being predefined during the study selection process.

The final corpus was subsequently used to conduct the comparative and quantitative analyses across Software Engineering, Cybersecurity, and Computer Science.

## 6. PRISMA Flow Diagram

The repository includes the PRISMA flow diagram illustrating the study identification, screening, eligibility assessment, duplicate removal, and final inclusion stages.

The diagram summarizes the numerical progression of the study selection process:

| PRISMA stage | Description | Records |
|---|---|---:|
| Identification | Raw records retrieved from four digital libraries | 1,198,779 |
| Relevance assessment | Consolidated records assessed for relevance to LLM evaluation | 10,079 |
| Relevance assessment | Records excluded as not relevant to LLM evaluation | 7,856 |
| Duplicate removal | Duplicate records identified and removed | 217 |
| Unique records | Records retained after duplicate removal | 2,006 |
| Methodological eligibility | Studies excluded for not focusing on LLM evaluation methodologies | 1,314 |
| Further assessment | Studies retained for domain-specific eligibility assessment | 692 |
| Domain-specific eligibility | Studies excluded for not meeting the predefined domain criteria | 397 |
| Final inclusion | Primary studies included in the review | **295** |

**Note:** The 1,198,779 figure represents the total raw search results returned by the digital libraries. It does not represent the number of records individually examined during manual screening. The initial screening employed a saturation-based stopping rule.

## 7. Reproducibility and Transparency

The replication package is intended to support the verification of the study selection process and the findings reported in the manuscript.

In particular, the repository provides:

- Search-result spreadsheets and bibliographic information from the four digital libraries.
- Intermediate datasets documenting the successive study selection stages.
- The unique records retained after duplicate identification and manual verification.
- The datasets retained after methodological and domain-specific eligibility assessment.
- The final corpus of 295 primary studies.
- The PRISMA flow diagram summarizing the selection process.

The intermediate spreadsheets should be interpreted according to their respective stages in the selection process. The 2,006-record dataset, for example, represents the unique records remaining after duplicate removal, rather than the original 2,223 records retained following relevance assessment.

## 8. Repository Access

The replication package is publicly available at:

**GitHub Repository:**  
https://github.com/UbaidUllahResearch/LLMEvaluationSLR

Researchers can use the provided datasets to inspect the study selection process, verify the final corpus, examine the methodological taxonomy, and extend the analysis to additional LLM evaluation studies.

## 9. Contact

For questions, comments, or further information concerning the replication package and the systematic literature review, please contact the corresponding author.
