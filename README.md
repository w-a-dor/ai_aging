# AI & Aging in Europe – Data Preprocessing & Metric Engineering

This repository supports the capstone research project:

> **“Can Generative AI Help Europe Age Better?”**  
> *A sectoral analysis of workforce aging and GenAI potential across EU countries.*

It contains all code and data transformation workflows used to clean, merge, and analyze demographic and generative AI exposure data.

---

## Repository Structure
AI_AGING/
├── code/
│ ├── eurostat_transformation/ # Cleaning and sectoral aggregation of Eurostat data
│ │ ├── economic_activities_to_sectors.ipynb
│ │ ├── eurostat_countries_and_economic_activities_gender.ipynb
│ │ ├── eurostat_countries_and_economic_activities.ipynb
│ │ ├── eurostat_countries.ipynb
│ │ └── eurostat_economic_activities.ipynb
│ ├── gen_ai_adoption/ # Semantic mapping of Anthropic AEI to sectors
│ │ └── gen_ai_adoption_semantic_matching.ipynb
│ └── gen_ai_potential/ # Semantic mapping of GenAI potential data
│ └── gen_ai_potential_semantic_matching.ipynb
│
├── original_data/ # Unmodified input data sources
│ ├── anthropic.csv
│ └── gpts_are_gpts.csv
│
├── transformed_data/ # Cleaned, harmonized, and sector-mapped data
│ ├── ai_adoption_sector.csv
│ ├── ai_potential_sector.csv
│ ├── anthropic_clean_merging.csv
│ ├── economic_activity_sector.csv
│ ├── eurostat_countries.csv
│ ├── eurostat_full.csv
│ ├── eurostat_gender_countries.csv
│ ├── eurostat_gender_sectors.csv
│ ├── eurostat_sectors.csv
│ ├── gen_ai_adoption_model_disagreement_chatgpt.xlsx
│ ├── gen_ai_potential_model_disagreement_chatgpt.xlsx
│ └── gpts_clean_merging.csv
│
├── .gitignore
└── README.md

---

## Purpose

This repo documents:

- Cleaning and harmonization of **Eurostat** labor force data by **country**, **sector**, and **age group**
- Transformation of **Anthropic Economic Index (AEI)** and **GenAI potential scores** to align with EU economic sectors
- Semantic matching using **sentence-transformer models**
- Construction of key metrics for:
  - Workforce aging (level and pace)
  - GenAI adoption and potential
  - Sector-country alignment of demographic risk and GenAI opportunity

---

## Tech Stack

- **Python 3.10+**
- `pandas`, `numpy`, `scikit-learn`, `sentence-transformers`
- Jupyter Notebooks for transparent step-by-step processing
- GPT-4/ChatGPT used for manual validation in ambiguous semantic cases

---

## Data sources:
Eurostat Labour Force Survey (2014–2024)
Anthropic Economic Index (AEI)
GPTs-are-GPTs GenAI exposure scores (Eloundou et al.)

---

## Key Metrics Generated
Proportion of older workers (50+) per sector & country
Pace of aging (2014–2024 change)
AI adoption scores (based on Anthropic task-level usage)
GenAI potential scores (from expert-annotated β-scores)
Sectoral and national AI gaps (potential vs. adoption)

---

## Author

Weronika Dorociak
MSc Applied Social Data Science
London School of Economics