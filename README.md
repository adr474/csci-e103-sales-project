# CSCI E-103 — Sales Data Engineering Project

Harvard Extension School | Data Engineering for Analytics

## Project Overview

This project develops an end-to-end data engineering and analytics solution using Databricks, Apache Spark, and Delta Lake.

Using a historical retail sales dataset, our team will design and implement data ingestion, transformation, machine learning, and business intelligence workflows.

The project follows a Medallion Architecture (Bronze → Silver → Gold) and explores incremental processing, streaming design, data optimization, CI/CD, and disaster recovery.

## Team & Responsibilities

| Member | Role | Primary Responsibilities |
|---|---|---|
| Adrian | Data Architect / Lead | Architecture, integration, CI/CD, streaming design, DR |
| Zac | Data Engineer | Data ingestion and transformation pipelines |
| Oakley | Data Engineer | Data ingestion and transformation pipelines |
| Pruthvi | Data Scientist | Model development, training, and validation |
| Felicia | Data Scientist | Model development, training, and validation |
| Ben | BI Analyst | Dashboards, visualizations, access controls |

Specific responsibilities may evolve as development progresses.

## Project Architecture

The system follows a Medallion Architecture:

**Source Data → Bronze → Silver → Gold → ML / BI**

- **Bronze:** Raw data ingestion with minimal transformation.
- **Silver:** Data cleaning, validation, deduplication, and standardization.
- **Gold:** Business-ready datasets and aggregate tables.
- **Machine Learning:** Model training, evaluation, and prediction.
- **Business Intelligence:** Dashboards and analysis using curated data.

Incremental ingestion and a proposed streaming architecture are also included in the project scope.

See `docs/` for detailed architecture diagrams and design decisions.

## Technology Stack

- Databricks (Serverless)
- Apache Spark / PySpark
- Delta Lake
- Unity Catalog
- Databricks Jobs & Pipelines
- MLflow
- SQL / Python
- Git & GitHub

## Repository Structure

```text
csci-e103-sales-project/
├── docs/
├── notebooks/
├── src/                   # Reusable code and utilities
├── tests/                 # Project tests
├── README.md
└── .gitignore
```

Directories will be added as needed.

## Development & Collaboration

### Getting Started

1. Accept the invitation to the GitHub repository.
2. Log into the course Databricks workspace.
3. Connect your personal GitHub account in Databricks settings.
4. Create a personal Databricks Git folder linked to this repository.
5. Create a feature branch for your assigned work.
6. Confirm access to the appropriate project data assets.

### Git Workflow

1. Pull the latest changes from `main`.
2. Create or switch to your feature branch.
3. Develop and test your work in Databricks.
4. Commit and push changes to GitHub.
5. Open a pull request targeting `main`.
6. Have another team member review the changes.
7. Merge approved contributions.

**Do not develop directly on `main`.**

Example branch names:

- `feature/adrian`
- `feature/zac`
- `feature/oakley`
- `feature/pruthvi`
- `feature/felicia`
- `feature/ben`

### Data Management

- Shared project data is managed in Databricks.
- Developers should use separate development tables when testing.
- Coordinate before modifying shared Bronze, Silver, or Gold tables.
- Do not commit raw datasets, secrets, or credentials to GitHub.
- Document shared table names, schemas, and data contracts.

## Project Milestones

| Date | Deliverable |
|---|---|
| Nov 22, 2026 | Architecture, scope, and project planning |
| Nov 25, 2026 | Functional data engineering pipeline | 
| Dec 1, 2026 | Machine learning model |
| Dec 5, 2026 | BI dashboard |
| Dec 8, 2026 | Final project submission |

## Project Documentation


Project planning, presentation materials, and contribution records are maintained separately in the shared Google Drive.

## Project Status

**In Development**

Architecture and workspace configuration are in progress.

