# IDPcentral Scripts, Data, and Notebooks

This repository contains the scripts to generate the IDPcentral Knowledge Graph based on data harvested from [DisProt](https://disprot.org/), [MobiDB](https://mobidb.org/), and [ProteinEnsemble (PED)](https://proteinensemble.org/).

The starting point for this repository were the files developed during the ELIXIR sponsored BioHackathon-Europe 2020. That work was reported in [BioHackrXiv v3jct](https://doi.org/10.37044/osf.io/v3jct). This repo updates the scripts for the revised deployments, and scales the work to the entire content of the three sites.

### Notes

- The term 'source' is used to distinguish the page that was scraped
- The term 'dataset' is used to identify the collection of data that a particular record page (e.g. disprot:DP000003) belongs to

## Analysis Notebook

The notebook for exploring the generated knowledge graph can be run on the cloud using the mybinder service[^1]; click on logo below to get going.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AlasdairGray/IDP-KG/HEAD?labpath=notebooks%2FAnalysisQueries.ipynb)

[^1]: See this [tutorial](https://github.com/alan-turing-institute/the-turing-way/blob/main/workshops/boost-research-reproducibility-binder/workshop-presentations/zero-to-binder-python.md) for an overview of what [MyBinder](https://mybinder.org/) is and offers.

## REST API

A Linked Data [REST API](https://grlc.io/api-url?specUrl=https://raw.githubusercontent.com/AlasdairGray/IDP-KG/main/idpcentral-api.yml#/) is provided using the [grlc](https://grlc.io) services. 

- Swagger docs: https://grlc.io/api-url?specUrl=https://raw.githubusercontent.com/AlasdairGray/IDP-KG/main/idpcentral-api.yml#/
- Configuration file: [idpcentral-api.yml](idpcentral-api.yml)
