# LLM Evaluation Practices in Software Engineering, Cybersecurity, and Computer Science: A Systematic Literature Review

## 1. Overview

This repository contains the replication package for the systematic literature review (SLR) entitled **"LLM Evaluation Practices in Software Engineering, Cybersecurity, and Computer Science: A Systematic Literature Review."**

The study systematically investigates evaluation methodologies for Large Language Models (LLMs) across three research domains:

- Software Engineering (SE)
- Cybersecurity (CySec)
- Computer Science (CS)

The final review corpus comprises **295 primary studies**, which form the basis of the qualitative synthesis, methodological taxonomy, quantitative analysis, and discussion presented in the paper.

This repository provides the search-result spreadsheets, intermediate datasets, final study corpus, and PRISMA flow diagram to support the transparency, verification, and reproducibility of the study selection and analysis process.

## 2. Search Strategy for SLR

The systematic search was conducted using **eight search-query variations** across four digital libraries:

1. Google Scholar
2. IEEE Xplore Digital Library
3. ACM Digital Library
4. ScienceDirect

### 2.1. Initial Manual Identification Screening and Saturation-Based Stopping Rule

The initial search returned **1,198,779 raw search results**, distributed across the four digital libraries as follows:

| Digital Library | Raw Search Results |
|---|---:|
| Google Scholar | 591,400 |
| IEEE Xplore | 24,877 |
| ACM Digital Library | 158,525 |
| ScienceDirect | 423,977 |
| **Total** | **1,198,779** |

These figures represent the raw search-result counts reported by the respective digital libraries. The large retrieval volume resulted from the use of broad search strings intended to maximize coverage and reduce the likelihood of overlooking relevant publications. This was particularly evident in Google Scholar, which indexes scholarly publications from multiple publishers and research platforms and retrieves records through broad keyword matching across bibliographic information and indexed content. Consequently, its search results provide wider coverage than collections restricted to individual publishers or digital libraries.


Given the exceptionally large retrieval volume, manually examining every raw search result was not practically feasible. Therefore, an initial manual screening strategy based on a **saturation-based stopping rule** was applied.

One researcher examined titles and abstracts from the search-result pages for each query and digital library. Screening proceeded from the initial result pages, where records were generally more closely aligned with LLM evaluation, towards subsequent pages, where the relevance of the results progressively declined.

This decline was associated with the broad retrieval behavior of the search engines, which increasingly returned records containing individual query terms, such as *large*, *language*, *model*, *LLM*, *evaluation*, *performance*, *benchmarking*, and *assessment*, without necessarily addressing LLM evaluation.

For each query, screening was discontinued when **two consecutive search-result pages yielded no new relevant studies**. This operational stopping rule reduced the examination of increasingly irrelevant results while retaining potentially relevant records.

During this stage, records clearly outside the scope of the review were not retained. These included studies primarily concerned with applications of LLMs in:

- **Natural and Physical Sciences:** physics, chemistry, and materials science.
- **Life Sciences and Healthcare:** biomedicine, clinical informatics, genomics, and epidemiology.
- **Applied Engineering and Industry:** civil, mechanical, aerospace, and petroleum engineering.
- **Social Sciences and Humanities:** law, economics, and sociology.

These studies were excluded because their primary contributions concerned domain-specific applications rather than the evaluation of LLM capabilities, performance, limitations, robustness, or evaluation methodologies.

**Researcher involvement:** One researcher conducted the initial identification and title-and-abstract screening using the predefined review objectives and saturation-based stopping rule.

### 2.2. Initial Screening

The **10,079 records** were retained and consolidated from the four digital libraries.

The distribution of these records was:

| Digital Library | Records Retained |
|---|---:|
| Google Scholar | 5,400 |
| IEEE Xplore | 1,530 |
| ACM Digital Library | 1,516 |
| ScienceDirect | 1,633 |
| **Total** | **10,079** |

Google Scholar contributed the largest number of retained records, partly because its indexing covers scholarly publications from multiple publishers and digital libraries. In contrast, platforms such as IEEE Xplore and ACM Digital Library primarily provide access to publications within their respective digital collections.
Records excluded from 10,079 as not relevant to LLM evaluation are **7,856**, Records retained for further processing are **2,223**

| Selection Step | Number of Records |
|---|---:|
| Non relevant record to LLM evaluation | 7,856 |
| Record Left for further processing | **2,223** |




### 2.3. Duplicate Identification and Removal

Duplicate identification and removal were performed after the relevance assessment and before methodological eligibility screening.

This sequencing was adopted because the initial retrieval contained a substantial proportion of records that were subsequently excluded as irrelevant. Performing duplicate detection across the entire raw retrieval set would therefore have required processing a considerably larger collection, including records that would not proceed to subsequent screening. Furthermore, duplicate identification required manual verification to minimize the risk of removing distinct studies.

Duplicate detection was performed using Microsoft Excel. Potential duplicates were identified by sorting and filtering records according to their titles, with particular attention to differences in capitalization, punctuation, spacing, and formatting. Each flagged record was subsequently examined manually before removal.

Records were considered duplicates when they met one or more of the following criteria:

- Exact title match.
- Highly similar titles or minor formatting differences referring to the same publication, confirmed through the first author's name and other bibliographic information.
- Identical DOI, where available.

The duplicate-removal process resulted in the following progression:

| Selection Step | Number of Records |
|---|---:|
| Records retained after relevance assessment | 2,223 |
| Duplicate records identified and removed | 217 |
| Unique records retained after duplicate removal | **2,006** |

Consequently, `SpreadSheet-05.xlsx` contains the **2,006 unique records** obtained after removing the 217 manually verified duplicates from the 2,223 records retained following relevance assessment.

### 2.4. Eligibility 

The 2,006 unique records were subsequently assessed against the methodological eligibility criteria of the review.

This assessment examined whether LLM evaluation constituted a substantive component of each study. The examined methodological aspects included evaluation objectives, assessment mechanisms, metrics, validation techniques, benchmarks, evaluation frameworks, experimental procedures, datasets, and empirical findings.

Studies in which evaluation was only incidental to an LLM-based application, or which did not make a substantive methodological contribution to LLM evaluation, were excluded.

The resulting selection was:

| Selection Step | Number of Studies |
|---|---:|
| Unique records assessed | 2,006 |
| Studies excluded | 1,314 |
| Studies retained for In-Depth Analysis | **692** |

Accordingly, `SpreadSheet-06.xlsx` contains the 692 studies retained after methodological eligibility assessment.

### 2.5. In-Depth Analysis

The 692 studies retained after methodological screening were subjected to further analysis to determine whether they primarily addressed LLM evaluation within the predefined research domains of Software Engineering, Cybersecurity, and Computer Science.

Studies that did not meet this domain-specific eligibility criterion were excluded because they fell outside the predefined scope of the review.

The resulting selection was:

| Selection Step | Number of Studies |
|---|---:|
| Studies assessed for domain-specific eligibility | 692 |
| Studies excluded for not meeting the predefined domain criteria | 397 |
| Studies retained for final inclusion | **295** |

### 2.6. Final Inclusion

The final selection resulted in a corpus of **295 primary studies**, which constitutes the empirical foundation of the systematic literature review.

Following the establishment of this corpus, an inductive qualitative analysis was conducted to examine the evaluation objectives, assessment mechanisms, validation procedures, datasets, and methodological characteristics reported across the included studies.

This analysis revealed four recurring evaluation paradigms:

1. **Human Evaluation**
2. **Automated Evaluation**
3. **Adversarial Evaluation**
4. **Benchmark-Driven Evaluation**

The resulting taxonomy comprises four principal paradigms and 23 subcategories. These categories were derived inductively from recurring methodological patterns in the included studies rather than being predefined during the study selection process.

Accordingly, SpreadSheet-07.xlsx contains the 295 studies.

## 3. Relationship Between the Intermediate Datasets

The seven spreadsheets document the progression from the initial database searches to the final review corpus.

The relationship between the refined datasets is summarized below:

| Dataset | Number of Records | Selection Stage |
|---|---:|---|
| `SpreadSheet-01.xlsx` to `SpreadSheet-04.xlsx` | — | Raw search results and bibliographic information from the four digital libraries. |
| `SpreadSheet-05.xlsx` | 2,006 | Unique records after removing 217 duplicates from the 2,223 records retained following relevance assessment. |
| `SpreadSheet-06.xlsx` | 692 | Studies retained after methodological eligibility assessment. |
| `SpreadSheet-07.xlsx` | 295 | Final studies retained after domain-specific eligibility assessment. |

The three refined datasets represent successive stages of refinement rather than independent collections of studies.

The numerical progression is:

**10,079 records → 7,856 excluded → 2,223 records → 217 duplicates removed → 2,006 unique records → 1,314 excluded → 692 studies → 397 excluded → 295 final studies.**

This progression explains how the relevance assessment, duplicate removal, methodological screening, and domain-specific eligibility criteria contributed to the construction of the final review corpus.

## 4. PRISMA Flow Diagram

The repository includes the PRISMA-style flow diagram illustrating the complete study selection process, from initial database identification to final inclusion.

The diagram summarizes the numerical progression across the six stages:

| Stage | Description | Records |
|---|---|---:|
| Identification | Raw search results retrieved from four digital libraries | 1,198,779 |
| Screening | Records examined (10,079), Records excluded from 10,079 as not relevant to LLM evaluation (7,856), Records retained for further processing (2,223) | 2,223 |
| Duplicate removal | Duplicate records identified and removed | 217 |
| Eligibility | Records retained after duplicate removal (2,006), Studies excluded for not focusing on LLM evaluation methodologies (1,314). | 692 |
| In-Depth Analysis | Studies retained for domain-specific eligibility assessment (692), Studies excluded for not meeting the predefined domain criteria (397).   | 295 |
| Final inclusion | Primary studies included in the review | **295** |

## 6. Reproducibility and Transparency

The replication package is intended to support the verification of the study selection process and the findings reported in the manuscript.

In particular, the repository provides:

- Raw search-result spreadsheets and bibliographic information from the four digital libraries.
- The distribution of records retained from each digital library following initial screening.
- Intermediate datasets documenting the successive study selection stages.
- The unique records retained after duplicate identification and manual verification.
- The datasets retained after methodological and domain-specific eligibility assessment.
- The final corpus of 295 primary studies.
- The PRISMA flow diagram summarizing the complete selection process.

The intermediate spreadsheets should be interpreted according to their respective stages in the selection process. For example, the 2,006-record dataset represents the unique records remaining after removing 217 duplicates from the 2,223 records retained following relevance assessment.

Together, these materials provide a transparent account of how the final corpus was established and how the included studies underpin the review's findings.

## 7. Repository Access

The replication package is publicly available at:

**GitHub Repository:**  
https://github.com/UbaidUllahResearch/LLMEvaluationSLR

Researchers can use the provided datasets to inspect the study selection process, verify the final corpus, examine the methodological taxonomy, and extend the analysis to additional LLM evaluation studies.

## 8. Contact

For questions, comments, or further information concerning the replication package and the systematic literature review, please contact the corresponding author.
