# A Two-Dimensional Click Model for Two-Column Search Interfaces

This repository contains the code, notebooks, and supporting materials for my MSc thesis on modeling user click behavior in two-column search interfaces.

The project uses the Qilin dataset to investigate whether explicitly modeling both row and column position improves click prediction compared to traditional click models designed for single ranked lists.

## Research Question
How can user click behavior in two-column search interfaces be modeled, and do two-dimensional click models better predict clicks than traditional click models designed for single ranked lists?

### Sub-questions
- Which scanning assumptions (e.g., row-by-row or S-shaped scanning) best explain observed user click behavior?
- Do two-dimensional click models provide better predictive performance than click models designed for single ranked lists?
- What implications do two-dimensional click models have for interpreting click data in two-column search interfaces?

## Thesis Focus
- Exploratory data analysis of user interaction logs  
- Analysis of row and column position effects in a two-column layout  
- Development of a two-dimensional click model  
- Comparison with classical click models for single ranked lists  

## Repository Structure
- Exploratory Data Analysis in EDA.ipynb
-

## Dataset
This project uses the Qilin dataset for multimodal information retrieval and user session analysis.

## Goal
The goal is to determine whether a two-dimensional representation of result placement better captures user examination behavior in two-column interfaces and improves click prediction.

## Installation
pip install -r requirements.txt