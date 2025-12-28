# Project Structure

This document outlines the proposed directory structure for the OpenGene Toolkit repository. The structure is designed to keep the project organized, scalable, and easy to navigate for contributors.

## Overview

```
open-gene-toolkit/
├── data/                    # Example datasets, schemas, and reference files
├── docs/                    # Documentation, tutorials, and user guides
├── scripts/                 # Standalone utility scripts for data validation, processing, etc.
├── src/                     # Core source code (Python modules, packages)
├── tests/                   # Unit and integration tests
├── .github/                 # GitHub-specific configurations (workflows, issue templates)
├── LICENSE
├── README.md
├── CONTRIBUTING.md
├── PROJECT_STRUCT.md
└── pyproject.toml / setup.py   # Python package metadata and dependencies
```

## Directory Descriptions

### `/data`

This directory contains example datasets, schema definitions, and reference files that illustrate the expected data formats for the OpenGene Toolkit.

- `schemas/` – JSON Schema or YAML definitions for standardized data formats (e.g., knockout results, transposon insertion data).
- `examples/` – Example files that conform to the defined schemas, useful for testing and onboarding.
- `reference/` – Reference genomes, gene annotations, or other static resources that may be used by analysis pipelines.

### `/docs`

All project documentation lives here, including user guides, developer documentation, and API references.

- `user-guide/` – Step‑by‑step instructions for using the toolkit’s features.
- `developer/` – Information about the codebase, architecture, and contribution workflows.
- `api/` – Auto‑generated API documentation (if applicable).
- `tutorials/` – Jupyter notebooks or markdown files that walk through common use cases.

### `/scripts`

Standalone scripts that perform specific tasks such as data validation, format conversion, or simple analyses. These scripts are intended to be run directly and may not be part of the core library.

- `validate_schema.py` – A script that checks whether a given data file conforms to the project’s schema (see Issue #3).
- `import_dataset.py` – A script to import a public dataset into the standardized format.
- `utilities/` – Helper scripts for common operations (e.g., downloading data, cleaning metadata).

### `/src`

The core source code of the OpenGene Toolkit, organized as a Python package (or packages). This is where the main functionality for data integration, querying, and analysis resides.

- `opengene/` – The main Python package.
  - `core/` – Core modules (data models, schema validation, I/O).
  - `integration/` – Modules for importing data from specific sources (CRISPR screens, transposon databases, etc.).
  - `analysis/` – Statistical and visualization utilities.
  - `cli/` – Command‑line interface entry points.
- `setup.py` / `pyproject.toml` – Package metadata and dependency management.

### `/tests`

Contains all unit tests, integration tests, and test data. Follows the same sub‑directory layout as `/src` to keep tests close to the code they validate.

- `unit/` – Tests for individual functions and classes.
- `integration/` – Tests that verify the interaction between multiple components.
- `fixtures/` – Small test datasets and mock objects used by the tests.

### `/.github`

GitHub‑specific configuration files for automating workflows, managing issues, and enforcing community standards.

- `workflows/` – GitHub Actions workflows for CI/CD (testing, linting, deployment).
- `ISSUE_TEMPLATE/` – Templates for bug reports, feature requests, and data‑source suggestions.
- `PULL_REQUEST_TEMPLATE.md` – Template for pull request descriptions.
- `CODE_OF_CONDUCT.md` – Contributor code of conduct (referenced from CONTRIBUTING.md).

## Notes

- This structure is **provisional** and may evolve as the project grows. Contributors are encouraged to suggest improvements via issues or pull requests.
- All new directories should include a `README.md` file explaining their purpose and content.
- Keep file and directory names lowercase with hyphens or underscores for readability (follow Python package naming conventions where appropriate).

## Getting Started

To start working with the codebase, clone the repository and explore the directories above. If you are unsure where to place a new file, please open an issue for discussion.