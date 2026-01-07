# Code

## Purpose
This folder contains R scripts used to analyse processed survey data and to compare the performance of ROV surveys with underwater visual censuses (UVC), catch surveys, and baited remote underwater video systems (BRUVS).

Analyses focus on comparisons of elasmobranch species richness and relative abundance across survey methods.

## Software environment
Analyses were conducted using:
- R version 4.3.1

Key R packages include:
- tidyverse (data cleaning and visualisation)
- dplyr
- ggplot2
- glmmTMB
- performance

Exact package versions are reported in the associated manuscript.

## Analytical workflow
Analyses are structured by experiment:

### Experiment 1 – UVC vs ROV
- Descriptive comparisons of species detections
- Poisson GLM comparing total elasmobranch counts
- Survey duration included as an offset term
- Model diagnostics assessed overdispersion, zero inflation, and residual structure

### Experiment 2 – Catch surveys vs ROV
- Descriptive comparison of species richness
- Calculation of:
  - Catch per unit effort (CPUE)
  - Sightings per unit effort (SPUE)
- Metrics calculated both across the full study period and per day

### Experiment 3 – BRUVS vs ROV
- Reef-specific Poisson GLMs
- Response variable: MaxN for both methods, with ROV MaxN calculated as the maximum number of elasmobranchs sighted per species, per depth bin
- Predictor: survey method (BRUVS vs ROV)
- Offset term used to standardise ROV survey time relative to BRUV soak time
- Model selection based on AIC

## Outputs
Scripts generate summary tables and figures used in the manuscript. Outputs are saved to designated results or figures directories as specified within individual scripts.

## Notes
- Scripts are intended to reproduce analyses reported in the manuscript, not to serve as a general-purpose analysis pipeline.
- Users should consult the manuscript Methods section for full methodological context.
