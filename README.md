# Predicting Antimicrobial Resistance (AMR) in Microbial Genomes and Cost Burden Analysis Using Machine Learning

## Overview
This project aims to analyze patterns of antimicrobial resistance (AMR) in *Campylobacter jejuni* and *C. coli* isolates from Scotland and England. It utilizes machine learning and statistical modeling to predict AMR phenotypes from genomic and epidemiological data, and to forecast the future clinical and economic burden of AMR in the UK.

## Problem Statement
The project addresses the critical public health challenge of antimicrobial resistance (AMR) in *Campylobacter*, a major cause of bacterial gastroenteritis worldwide. The increasing difficulty and cost of treating *Campylobacter* infections due to resistance to key antibiotics necessitate advanced predictive models to understand and mitigate AMR.

## Data Description
The dataset comprises 6,683 clinical and animal *Campylobacter* isolates collected between 2001 and 2017, sourced from the PubMLST database. It includes:
- Genomic data such as MLST types, AMR genes, and point mutations
- Epidemiological metadata (region, year, month, source of isolation)
- Resistance phenotypes for multiple antibiotic classes

## Methodology
The methodology involves:
1. Data preprocessing and feature engineering
2. Application of machine learning models including:
   - Random forest classification for AMR phenotype prediction
   - Time series models (SARIMAX and Prophet) for resistance forecasting
3. Economic analysis to project the future burden of AMR through 2050

## Key Findings
- 74% accuracy in predicting AMR phenotypes using machine learning models
- Identification of specific genetic determinants linked to resistance (gyrA mutations, tet(O) gene)
- Association of certain *Campylobacter* lineages with higher AMR rates
- Increasing trend in fluoroquinolone resistance prevalence over time
- Economic burden of AMR-associated Campylobacter infections projected to exceed £1.9 billion annually by 2050

## Visualizations

### AMR Trends and Projections (2000-2050)
![AMR Trends and Projections](results/complete_resistance_analysis.pdf)

### Economic Burden Projection
![Economic Burden Projection](results/economic_burden_plot.pdf)

## Installation Instructions
To run the code in this repository, you need to have Python installed along with the following libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn biopython plotly bokeh statsmodels prophet
