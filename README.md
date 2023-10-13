# NASA_ODSR_DATA
This repo contains the main work on [NASA SPACE APPS CHALLENGE](https://www.spaceappschallenge.org/).

# OUR TEAM: [**Space-Born RNA**](https://www.spaceappschallenge.org/2023/find-a-team/dea-has-covid/?tab=details)
- [Anzor Gozalishvili](https://github.com/AnzorGozalishvili)
- [Amiran Gozalishvili](https://github.com/AmiranGozalishvili)
- [Revaz Revazashvili](https://github.com/revaza05)
- [Kristine Eliosidze](https://github.com/kristiELLL)
- [Medea Gejadze](https://www.linkedin.com/in/medea-gejadze-3ab818207/)
- [Salome Javashvili](https://www.linkedin.com/in/salome-javashvili/)

# Project Description
[Project Description](nasa_challenge_project_description.md)

# Notebooks
- [dataset curation notebook](dataset_curation.ipynb): contains the codes that collects data (NASA OSDR dataset) from s3, processes and merges tables into one.
- [Dataset exploration notebook](NASA_OSDR_explore.ipynb): contains data exploration code to guide users on loading it using huggingface datasets library, iterate on samples, read RNA sequences from fasta files and make ML model inference (RNABERT example)

# Dataset Files
- [assays_all](assays_all.csv): all experiment assays merged
- [assays](assays.csv): small sample of assays from OSD-524 experiment

# Huggingface Datasets Repository
- [NASA_OSDR](https://huggingface.co/datasets/anz2/NASA_OSDR): contains merged table on huggingface datasets repo
- [RNABERT](https://huggingface.co/anz2/RNABERT): incomplete work. Trying to make RNABERT available on Huggingface Models registry.

  
