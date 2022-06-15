# IDPcentral Scripts, Data, and Notebooks

This repository contains the scripts to generate the IDPcentral Knowledge Graph based on data harvested from [DisProt](https://disprot.org/), [MobiDB](https://mobidb.org/), and [ProteinEnsemble (PED)](https://proteinensemble.org/).

The starting point for this repository were the files developed during the ELIXIR sponsored BioHackathon-Europe 2020. That work was reported in [BioHackrXiv v3jct](https://doi.org/10.37044/osf.io/v3jct). This repo updates the scripts for the revised deployments, and scales the work to the entire content of the three sites.

__Authors:__
- [Alasdair J G Gray](http://orcid.org/0000-0002-5711-4872) ([@AlasdairGray](https://github.com/AlasdairGray))
- [Petros Papadopoulos](https://orcid.org/0000-0002-8110-7576) ([@petrospaps](https://github.com/petrospaps))
- [Imran Asif](https://orcid.org/0000-0002-1144-6265) ([@ImranAsif48](https://github.com/ImranAsif48))
- [Ivan Mičetić](https://orcid.org/0000-0003-1691-8425) ([@ivanmicetic](https://github.com/ivanmicetic))
- [Andras Hatos](https://orcid.org/0000-0001-9224-9820) 

__Citing IDP-KG:__ If you used IDP-KG in your work, please cite the [SWAT4HCLS paper](http://ceur-ws.org/Vol-3127/paper-1.pdf):
```bib
@inproceedings{GrayEtal:bioschemas-idpkg:swat4hcls2022,
  author = {Gray, Alasdair J. G. and Papadopoulos, Petros and Asif, Imran and Micetic, Ivan and Hatos, Andr{\'{a}}s},
  title = {Creating and Exploiting the Intrinsically Disordered Protein Knowledge Graph {(IDP-KG)}},
  booktitle = {13th International Conference on Semantic Web Applications and Tools for Health Care and Life Sciences, {SWAT4HCLS} 2022, Virtual Event, Leiden, The Netherlands, January 10th to 14th, 2022},
  series = {{CEUR} Workshop Proceedings},
  volume = {3127},
  pages = {1--10},
  publisher = {CEUR-WS.org},
  year = {2022},
  url = {http://ceur-ws.org/Vol-3127/paper-1.pdf}
}
```

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
