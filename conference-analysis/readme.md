# AI Conference Affiliation Analysis

This repository contains a small data analysis project that examines **industry participation and industry–academia collaboration in major AI conferences**.

The main goal is to analyze **AI research output from the perspective of companies**, and to explore **which universities and research institutes collaborate with industry in top AI venues**.

The analysis focuses on:

- company research output in AI conferences
- industry–academia collaboration patterns
- major research organizations partnering with companies
- geographic distribution of collaborations

## Research Questions

This project aims to answer several questions about industry participation in AI research:

1. Which companies publish the most papers in top AI conferences in collaboration with research institutes?
2. How frequently do companies collaborate with universities or research institutes?
3. Which research organizations appear most often in industry collaborations?
4. What is the regional distribution of these collaborations?

The analysis is based on paper metadata from the following conferences: NeurIPS, ICML, CVPR, ICLR

## Data Processing Pipeline

The workflow of this project is:

Raw conference metadata (JSON)

↓

Affiliation cleaning and preprocessing

↓

Company detection

↓

Research organization detection

↓

Industry–academia collaboration analysis

↓

Result tables (Excel)

## Repository Structure

```text
data/
├── raw/                       # Original metadata collected from conference sources
│   ├── cvpr2025.json
│   ├── iclr2025.json
│   ├── icml2025.json
│   └── neurips2025.json
│
└── processed/                 # Cleaned datasets after preprocessing
    ├── cvpr2025.xlsx
    ├── iclr2025.xlsx
    ├── icml2025.xlsx
    └── neurips2025.xlsx

notebook/
└── conference_affiliation_analysis_case.ipynb

outputs/
├── cvpr2025_company_research_partnerships.xlsx
├── iclr2025_company_research_partnerships.xlsx
├── icml2025_company_research_partnerships.xlsx
└── neurips2025_company_research_partnerships.xlsx

README.md
```

## Output Tables

Each output Excel file contains structured tables describing company participation and collaboration patterns, including:

- total papers by company
- accepted papers
- acceptance rate by company
- industry–academia collaboration counts
- research organizations collaborating with companies
- country and regional distribution

## Notebook

The repository includes a single example notebook:

notebook/conference_affiliation_analysis_case.ipynb

This notebook demonstrates the main workflow:

- preprocessing conference metadata
- cleaning affiliation fields
- detecting company affiliations
- identifying research organizations
- analyzing industry–academia collaborations

## Notes

This repository is intended as a demonstration of the analysis workflow and results.

Some raw datasets may be omitted due to file size limitations.
