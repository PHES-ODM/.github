---
editor_options: 
  markdown: 
    wrap: 72
---

# <img src="img/ODM-logo.png" align="right" width="180"/> The Public Health Environmental Surveillance Open Data Model (PHES-ODM, or ODM)

<!-- badges: start -->

[![Lifecycle:
development](https://img.shields.io/badge/lifecycle-stable-green.svg)](https://lifecycle.r-lib.org/articles/stages.html#stable-1)
![](https://img.shields.io/github/v/release/big-life-lab/covid-19-wastewater?color=green&label=GitHub)
[![License: CC BY
4.0](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![](https://img.shields.io/badge/doi-10.17605/OSF.IO/49Z2B-yellowgreen.svg)](https://osf.io/49z2b/)

<!-- badges: end -->

## Description

PHES-ODM began as an open data model for wastwater-based surveillance of
SARS-CoV-2. PHES-ODM Versions 2 & 3 expand the original ODM to include
surface and air testing, in addition to water. These later versions
allow for tracking of public health threats in any environment, and
include robust support for reporting biologics, toxins, and/or other
health risks.

The ODM strives to improve environmental and wastewater surveillance
through interoperable data. The ODM follows an open science approach,
including including [FAIR Guiding
Principles](https://www.go-fair.org/fair-principles/). People and
institutions can contribute to the development of the ODM and the ODM
seeks to support a wide range of users. As part of that mission, the ODM
team have developped a suite of tools to support use and uptake of the
model. Repositories for the tools can be found here, and include a
validator, a sharing tool, a mapping tool, and a pipeline to transform
PCR outputs directly into ODM.

## Data and metadata dictionary

The ODM is comprised of 19 report tables and 7 look-up tables, linked to
each other based on logic relationships. The following figure provides
an overview of the different data sources that are currently captured.

![Schematic representation of the ODM](img/subway.png)

![Entity Relationship Diagram](img/ODM_ERD_V3.0.0.png)

The ODM is modular in its structure, and all tables are not mandatory.
The structure is scalable as well to be only as complex as users need it
to be, with much of the model existing optionally, but supporting all
possible use-cases.

## Artifacts List - Communications & External-Facing

### GitHub - model 
 - [Big-Life-Lab/PHES-ODM](https://github.com/Big-Life-Lab/PHES-ODM) 
 - [Big-Life-Lab/PHES-ODM-Doc](https://github.com/Big-Life-Lab/PHES-ODM-Doc) 

### GitHub - software
 - [Big-Life-Lab/PHES-ODM-Validation](https://github.com/Big-Life-Lab/PHES-ODM-Validation)
 - [Big-Life-Lab/PHES-ODM-Validation-Web](https://github.com/Big-Life-Lab/PHES-ODM-Validation-Web) (Private)
 - [Big-Life-Lab/PHES-ODM-sharing](https://github.com/Big-Life-Lab/PHES-ODM-sharing)
 - [Big-Life-Lab/PHES-ODM-Mapper](https://github.com/Big-Life-Lab/PHES-ODM-Mapper)
 - [Big-Life-Lab/PHES-ODM-LinkMLGenerator](https://github.com/Big-Life-Lab/PHES-ODM-LinkMLGenerator)
 - [Big-Life-Lab/PHES-ODM-MapGenerator](https://github.com/Big-Life-Lab/PHES-ODM-MapGenerator) (Private)
 - [martinwellman/phes-odm-conductor](https://github.com/martinwellman/phes-odm-conductor) (Private)
 - [qpcr-analyzer]() 
 
### GitHub - supporting infrastructure
 - [PHES-ODM/.github](https://github.com/PHES-ODM/.github)
 - [Big-Life-Lab/release-automation-testing](https://github.com/Big-Life-Lab/release-automation-testing)
 
### Websites:
 - [Offical Website](https://www.phes-odm.org)
 - [Lucid Chart ERD](https://lucid.app/lucidchart/847978df-d627-4b8a-a379-faca7a517ef4/edit?viewport_loc=-2932%2C-2689%2C13808%2C8809%2CztJGI_4dY9KX&invitationId=inv_0de7777b-888b-4d8a-827d-2306bdc48cce)
 - [Discourse Page](https://odm.discourse.group)
 - [OADP website](https://oadp.phes-odm.org)
 - [Documentation Website](https://docs.phes-odm.org)
 – maybe other libraries’documentation sites?
 - [Vimeo videos](https://vimeo.com/projectbiglife)
 - [OSF Repository](https://osf.io/49z2b/)
 - [Zenodo Repository](https://zenodo.org/records/10794558) (not named, but I own it still for some reason – maybe delete??)
 - [Panacea Network Presentation Video - SPA](https://www.youtube.com/watch?v=tBLe8J2jGWU)
 - [Panacea Network Presentation Video - ENG](https://www.youtube.com/watch?v=QE8wNO3S0-4&t=1439s)
 - (To-do: ---separate out presentations ------)

### Publications:
 - [PHES-ODM Introductory Publication in Water Science & Technology](https://iwaponline.com/wst/article/89/1/1/99450/A-comprehensive-open-source-data-model-for)
 - Email address: [phesd_odm\@ohri.ca](mailto:phesd_odm@ohri.ca){.email}
 
## Artifacts List - Files 
 -	linkMl schema + config files/mapping sheets(?)/modules/directories
 -	csv files
 -	templates
 -	ERD pdfs
 -	Documentation files
 -	SQL database structure
 -	Design materials, logo, icon library
 -	Governance documentation
 -	TORs
*Consider dependencies, but separately. Major ones are LinkML, Excel, LucidChart, and LinkML schemasheets*

## Acknowledgements

Development and maintenance of the ODM is the result of a collaboration
between researchers from multiple institutions:

-   The University of Ottawa
-   [CIHR Coronavirus Variants Rapid Response Network
    (CoVaRR-Net)](https://covarrnet.ca)
-   Université Laval
-   CHEO Research Institute
-   modelEAU
-   CentrEau - Centre québécois de recherche sur la gestion de l'eau
-   Public Health Agency Canada
-   Ministry of Environment, Conservation, and Parks - MECP Ontario
-   European Union DG Joint Research Centre
-   The Ottawa Hospital Research Institute
