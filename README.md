# <img src="img/ODM-logo.png" align="right" alt="" width="180"/> The Public Health Environmental Surveillance Open Data Model (PHES-ODM, or ODM)

<!-- badges: start -->

[![Lifecycle:
development](https://img.shields.io/badge/lifecycle-stable-green.svg)](https://lifecycle.r-lib.org/articles/stages.html#stable-1)
![](https://img.shields.io/github/v/release/big-life-lab/covid-19-wastewater?color=green&label=GitHub)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![](https://img.shields.io/badge/doi-10.17605/OSF.IO/49Z2B-yellowgreen.svg)](https://osf.io/49z2b/)

<!-- badges: end -->

## Description

PHES-ODM began as an open data model for wastwater-based surveillance of SARS-CoV-2. PHES-ODM Versions 2 & 3 expand the original ODM to include surface and air testing, in addition to water. These later versions allow for tracking of public health threats in any environment, and include robust support for reporting biologics, toxins, and/or other health risks.

The ODM strives to improve environmental and wastewater surveillance through interoperable data. The ODM follows an open science approach, including including [FAIR Guiding Principles](https://www.go-fair.org/fair-principles/). People and institutions can contribute to the development of the ODM and the ODM seeks to support a wide range of users. As part of that mission, the ODM team have developped a suite of tools to support use and uptake of the model. Repositories for the tools can be found here, and include a validator, a sharing tool, a mapping tool, and a pipeline to transform PCR outputs directly into ODM.

## Data and metadata dictionary

The ODM is comprised of 19 report tables and 7 look-up tables, linked to each other based on logic relationships. The following figure provides an overview of the different data sources that are currently captured.

![Schematic representation of the ODM](img/subway.png)

![Entity Relationship Diagram](img/ODM_ERD_V3.0.0.png)

The ODM is modular in its structure, and all tables are not mandatory. The structure is scalable as well to be only as complex as users need it to be, with much of the model existing optionally, but supporting all possible use-cases.

## Acknowledgements

Development and maintenance of the ODM is the result of a collaboration between researchers from multiple institutions:

- The University of Ottawa
- [CIHR Coronavirus Variants Rapid Response Network (CoVaRR-Net)](https://covarrnet.ca)
- Université Laval
- CHEO Research Institute
- modelEAU
- CentrEau - Centre québécois de recherche sur la gestion de l'eau
- Public Health Agency Canada
- Ministry of Environment, Conservation, and Parks - MECP Ontario
- European Union DG Joint Research Centre
- The Ottawa Hospital Research Institute
