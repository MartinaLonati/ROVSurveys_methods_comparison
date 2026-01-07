# Processed data

## Overview
This directory contains processed datasets used to compare the performance of remotely operated vehicle (ROV) with traditional elasmobranch survey methods: underwater visual censuses (UVC), catch surveys, and baited remote underwater video systems (BRUVS).

All datasets in this folder were derived from annotated video footage and/or field survey records and were formatted specifically for the statistical analyses reported in the associated manuscript.

Raw video data are not included in this repository.

---

## Experimental structure
Processed data correspond to three independent experiments conducted on the east coast of Australia.

### Experiment 1 – Moore Reef (ROV and UVC)
- Location: Moore Reef, northern Great Barrier Reef
- Methods: ROV transects and diver-based UVC transects (or DOV: diver operated vehicle)
- Transects: Four 100 m transects spanning depths of 5–20 m
- Data include:
  - Survey ID
  - Method - either ROV survey or underwater visual surveys carrying a diver operated video (DOV).
  - Depth
  - Time of day - three possible time brackets (dawn, afternoon, and dusk)
  - The type of reef aspect and habitat the transect was carried on
  - The species signed and it's count of individuals 
  _ The survey duration

These data were used to compare overall elasmobranch abundance and species detection between ROV and UVC surveys.

---

### Experiment 2 – North West Island (ROV and catch surveys)
- Location: North West Island, southern Great Barrier Reef
- Methods: ROV surveys and single-hook drumline catch surveys
- Sampling period: Five consecutive days
- Data include:
  - Elasmobranch counts or sightings
  - Cumulative soak time (hours) or survey time calculated from start and end times
  - Set - the number of the single drumline (dropline) or the transet number per day
  - Derived metrics:
    - Catch per unit effort (CPUE)
    - Sightings per unit effort (SPUE)

This data were used to compare relative abundance estimates between ROV surveys and catch surveys, while accounting for different efforts 

### Experiment_2.sp – North West Island (ROV and catch surveys)
- Location: North West Island, southern Great Barrier Reef
- Methods: ROV surveys and single-hook drumline catch surveys
- Sampling period: Five consecutive days
- Data include:
  - Elasmobranch counts or sightings for each species

This data was used to compare species richness between ROV surveys and catch surveys

---

### Experiment 3 – Coral Sea Marine Park (ROV and BRUVS)
- Location: Multiple reefs within the Coral Sea Marine Park
- Methods: BRUVS deployments and depth-stratified ROV transects
- Data include:
  - BRUV-derived MaxN values per deployment, and ROV derived MaxN per transect and depth bin
  - ROV sightings aggregated into 10 m depth bins
  - ROV data was aggregated into depth bins to enable comparison with BRUV-derived MaxN values.
  - Standardised survey effort per observation unit
  - Data was filtered to consider only elasmobranchs althoug raw data contained other teleost species

Only sites where elasmobranchs were detected were retained for methods comparison.

---

## Data processing notes
- Video footage was annotated prior to data processing.
- For Experiments 1 and 2, synchronised multi-camera videos were used to minimise double-counting.All videos, includine Experiment 3 where annotated using Event Measure
- All processing steps were implemented using scripts in the `code/` directory.

---

## Restrictions and considerations
- Raw video files are excluded due to file size and storage limitations.
- Processed data are intended to support reproducibility of analyses presented in the manuscript and are not intended as standalone survey products.

---

## Related files
- Analysis scripts: `code/`
