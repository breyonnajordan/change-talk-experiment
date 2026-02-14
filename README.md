# An Experimental Test of Change Exposure in Civic Contexts

## Overview
This repository contains the data, analysis code, and outputs for an experimental study testing whether brief exposure to change talk or sustain talk influences beliefs about and intentions toward everyday civic engagement (petition signing and small donations).

The study was implemented as a Qualtrics survey and analyzed in R. No statistically significant effects were detected.


## Files
/data
  - [raw_data.csv](data/raw_data.csv) (personally identifiable information removed)

/scripts
  - [01_script.Rmd](scripts/01_script.Rmd)

/outputs
  - [change-talk-outputs.html](outputs/change-talk-outputs.html)

/docs
  - [paper](docs/change-talk-paper.pdf)
  - [poster](docs/change-talk-poster.pdf)
  - [presentation](docs/change-talk-presentation.pdf)

## Data
- Survey responses collected from 120 Wesleyan University students
- Survey designed by the author and approved by a data science instructor
- Personally identifying information (emails) removed prior to publication
- Some responses excluded due to incompletion or failed attention checks (see 01_cleaning.R)

## Method
- Participants were randomly assigned to one of four vignette conditions:
  - Petition signing × change talk
  - Petition signing × sustain talk
  - Donation × change talk
  - Donation × sustain talk
- Outcomes:
  - Intention to engage in civic action
    - Two composites (petitions, donations)
    - Each averaged across three 5-point Likert items
  - Belief in efficacy of civic action
    - Two composites (petitions, donations)
    - Each averaged across three 5-point Likert items
- Survey administered via Qualtrics
- Analysis conducted in R using standard linear modeling

## Reproducing the Analysis
- Run scripts:
  1. 01_script.R
    - Loads raw data
    - Removes identifying columns
    - Applies exclusions
    - Outputs cleaned_data.csv
    - Loads cleaned data
    - Fits models
    - Outputs model summaries
    - Generates figures and tables

## Requirements
- R (tested with R ≥ 4.5)
- RStudio (recommended)
- Packages are loaded within script (see headers)

## Results
- No significant results were found. 
- link to [output](outputs)
- link to [paper](docs/change-talk-paper), [poster](docs/change-talk-poster)

## Limitations
- No reading comprehension check was used; only an attention check at the end of the survey
- Brief exposure limits interpretability of null effects
- Results do not establish that change or sustain talk has no effect—only that any effect may be small or context-dependent in this design

## Related Links
- [Project page on my portfolio](https://breyonnajordan.com/projects/university-major/change-talk-experiment)

