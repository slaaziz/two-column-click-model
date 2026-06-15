# A Two-Dimensional Click Model for Two-Column Search and Recommendation Interfaces

This repository contains the code, notebooks, and supporting materials for my MSc thesis on modeling user click behavior in two-column search and recommendation interfaces.

The project uses the Qilin dataset to investigate whether explicitly modeling both row and column position improves click prediction compared to traditional click models designed for single ranked lists. Experiments are conducted on both the search and recommendation splits of Qilin to assess whether findings generalize across interaction contexts.

## Research Question
How can user click behavior in two-column search interfaces be modeled, and to what extent do two-dimensional click models improve click prediction over traditional click models designed for single ranked lists?

### Sub-questions
- Which scanning assumptions (e.g., row-by-row or S-shaped scanning) best explain observed user click behavior?
- To what extent do two-dimensional click models improve predictive performance over click models designed for single ranked lists?
- What implications do two-dimensional click models have for interpreting click data in two-column search interfaces?

## Thesis Focus
- Exploratory data analysis of user interaction logs on both the search and recommendation splits
- Analysis of row and column position effects in a two-column layout
- Development of a family of two-dimensional click models, including a Factored 2D PBM and a Neural 2D PBM
- Comparison with classical click models for single ranked lists, including a theoretical equivalence proof for naive coordinate remapping
- Significance testing (McNemar's test) of model differences

## Repository Structure
- `EDA_rec.ipynb` — Exploratory data analysis for the recommendation split
- `EDA_search.ipynb` — Exploratory data analysis for the search split (primary)
- `model_rec.ipynb` — Model implementation and evaluation for the recommendation split
- `model_search.ipynb` — Model implementation and evaluation for the search split (primary)
- `media/` — Figures generated from the notebooks; a subset of these are included in the thesis
- `archive/` — Early development notebooks, kept for transparency:
  - `EDA.ipynb` — First exploratory analysis attempt, run on a smaller subset of the dataset before switching to the full search and recommendation splits
  - `model.ipynb` — Early model notebook — initial attempt using naive parameter estimation rather than the learned row and column factors used in the final Factored 2D PBM

## Dataset
This project uses the Qilin dataset for multimodal information retrieval and user session analysis, specifically the `search_train`/`search_test` and `recommendation_train`/`recommendation_test` splits.

## Goal
The goal is to determine whether a two-dimensional representation of result placement better captures user examination behavior in two-column search and recommendation interfaces and improves click prediction.

## Installation
```
pip install -r requirements.txt
```