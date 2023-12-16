# Animal Adoption Database

## Overview
The **Animal Adoption Database** project aims to aggregate data on adoptable animals from multiple sources into a centralized (at first) AWS database.

## Data Sources
- **Pet Finder**: [Pet Finder API](https://www.petfinder.com/developers/)
- **Rescue Groups**: [Rescue Groups API](https://rescuegroups.org/services/adoptable-pet-data-api/)
- **Pet Rescue**: [Pet Rescue API](https://www.petrescue.com.au/api/docs)

## Proposed Architecture
### Data Ingestion
- **Python Scripts**: For API data extraction
- **Processing Options**:
  - **EMR** or **Lambda Functions**: For serverless batch processing

### Storage
- **S3 Bucket**: Primary data storage solution

### Orchestration
- Options being considered:
  - **Kestra**
  - **Prefect**
  - **Airflow**

### Data Processing and Modeling
- **PySpark**: For data processing
- **(Optional) DBT Core**: To model data in layers (Bronze, Silver, and Gold)

### Additional Components
- **WAP Patterns**: To be determined
- **Public Dashboard**: For showcasing animal listings

## Personal Motivation
As the owner of one dog and two adopted cats, I am deeply invested in the cause of animal adoption. This project is not only a technical challenge but also a personal endeavor, inspired especially by the love for my black cat and the desire to address misconceptions about them.

> "Every time I look at my pets, I am reminded of the importance of adoption."

## Capstone Project
This endeavor is part of my Capstone project, focusing on leveraging technology for the betterment of pet adoption processes.
