# Contributing to OpenGene Toolkit

Thank you for your interest in contributing to the OpenGene Toolkit! This document outlines the process for contributing to the project, whether you are suggesting new data sources, reporting issues, or submitting code changes.

## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [How to Contribute](#how-to-contribute)
   - [Reporting Issues](#reporting-issues)
   - [Suggesting New Data Sources](#suggesting-new-data-sources)
   - [Submitting Code Changes](#submitting-code-changes)
   - [Improving Documentation](#improving-documentation)
3. [Development Workflow](#development-workflow)
   - [Setting Up the Development Environment](#setting-up-the-development-environment)
   - [Creating a Branch](#creating-a-branch)
   - [Making Changes](#making-changes)
   - [Testing](#testing)
   - [Submitting a Pull Request](#submitting-a-pull-request)
4. [Review Process](#review-process)
5. [Community and Communication](#community-and-communication)

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## How to Contribute

### Reporting Issues

If you encounter a bug, have a question, or want to suggest an improvement, please open an issue on the [GitHub issue tracker](https://github.com/hekredmoone9/open-gene-toolkit/issues).

**When reporting an issue, please include:**

- A clear and descriptive title.
- Steps to reproduce the problem (if applicable).
- Expected and actual behavior.
- Any relevant error messages, screenshots, or logs.
- Information about your environment (operating system, Python version, etc.).

### Suggesting New Data Sources

The OpenGene Toolkit aims to integrate genetic modification data from diverse sources. If you know of a public dataset, database, or publication that should be included, please open an issue with the label **"data-source"**.

**Please provide:**

- A brief description of the dataset.
- Links to the original source (DOI, URL, etc.).
- The data type (e.g., CRISPR screen, transposon insertion, knockout study).
- Any relevant metadata (species, experimental conditions, etc.).
- Why this dataset is valuable for the community.

### Submitting Code Changes

We welcome contributions of all sizes, from fixing typos to implementing new features. Before starting work on a major change, it is often helpful to discuss your idea in an issue or on the discussion board to ensure alignment with project goals.

### Improving Documentation

Good documentation is crucial for the success of any open‑source project. If you notice missing, outdated, or unclear documentation, please submit a fix. This includes README files, inline code comments, and tutorial materials.

## Development Workflow

### Setting Up the Development Environment

1. **Fork the repository** on GitHub.
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/<your-username>/open-gene-toolkit.git
   cd open-gene-toolkit
   ```
3. **Set up the upstream remote** (optional but recommended):
   ```bash
   git remote add upstream https://github.com/hekredmoone9/open-gene-toolkit.git
   ```

### Creating a Branch

Create a new branch for your changes. Use a descriptive name that reflects the nature of your contribution.

```bash
git checkout -b feature/your-feature-name
```

### Making Changes

Make your changes in the appropriate directory (see [PROJECT_STRUCT.md](PROJECT_STRUCT.md) for the project layout). Follow the existing code style and conventions.

### Testing

If you are adding new functionality, please include tests that verify your changes. If you are fixing a bug, add a test that reproduces the bug and shows that your fix resolves it.

### Submitting a Pull Request

1. **Commit your changes** with clear, descriptive commit messages.
2. **Push your branch** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
3. **Open a pull request** against the `main` branch of the upstream repository.
4. **Fill out the pull request template** (if available) and provide a concise description of your changes, linking to any related issues.

## Review Process

Once a pull request is submitted, project maintainers and other contributors will review your changes. You may be asked to make adjustments or provide additional information. The goal is to ensure that contributions are high‑quality and align with the project’s direction.

**Please be patient**—reviewers are volunteers who dedicate their time to the project.

## Community and Communication

- **Discussion Board:** For general questions, ideas, or help, use the GitHub Discussions feature (if enabled).
- **Weekly Meetings:** We plan to hold regular virtual meetings for contributors (details to be announced).
- **Contact:** You can reach the project leads by mentioning `@hekredmoone9` in issues or pull requests.

Thank you for helping to build a valuable resource for the genetics community!