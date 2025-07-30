# AI & Aging in Europe – Data Preprocessing & Metric Engineering

This repository supports the capstone research project:

> **“Can Generative AI Help Europe Age Better?”**  
> *A sectoral analysis of workforce aging and GenAI potential across EU countries.*

It contains all code and data transformation workflows used to clean, merge, and analyze demographic and generative AI exposure data.

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

## Contents of the Repository
This repo includes:

Raw data (excluding eurostat)

Cleaning routines for:
Eurostat Labour Force Survey (LFS)
Anthropic Economic Index (AEI)
GenAI exposure estimates from Eloundou et al. (2023)

Metric construction scripts, including:
Workforce aging indicators
Semantic matching routines using sentence embedding models
GenAI adoption scores
GenAI potential metrics

---

## Tech Stack

- **Python 3.10+**
- `pandas`, `numpy`, `scikit-learn`, `sentence-transformers`
- Jupyter Notebooks for transparent step-by-step processing
- GPT-4/ChatGPT used for manual validation in ambiguous semantic cases

---

## Data sources:
Eurostat Labour Force Survey (2014–2024): https://ec.europa.eu/eurostat/web/lfs
Anthropic Economic Index (AEI): https://huggingface.co/datasets/Anthropic/EconomicIndex
GPTs-are-GPTs GenAI exposure scores (Eloundou et al.): https://github.com/openai/GPTs-are-GPTs/

## Author

Weronika Dorociak
MSc Applied Social Data Science
London School of Economics