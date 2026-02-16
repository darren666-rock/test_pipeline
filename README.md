# test_pipeline

A simple pipeline sample demonstrating GitHub Actions CI/CD workflow.

## Overview

This repository contains a simple Python calculator application with an automated CI/CD pipeline using GitHub Actions.

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── pipeline.yml    # GitHub Actions workflow definition
├── app.py                  # Simple calculator application
├── test_app.py            # Unit tests
├── requirements.txt       # Python dependencies
└── README.md             # This file
```

## Pipeline Features

The GitHub Actions pipeline automatically:
1. **Checks out the code** from the repository
2. **Sets up Python environment** (Python 3.10)
3. **Installs dependencies** from requirements.txt
4. **Runs unit tests** using Python's unittest framework
5. **Executes the application** to verify it works

## Pipeline Triggers

The pipeline runs on:
- Push to `main` or `master` branches
- Pull requests targeting `main` or `master` branches
- Manual trigger via workflow_dispatch

## Local Development

### Running the Application

```bash
python app.py
```

### Running Tests

```bash
python -m unittest test_app.py
```

## Application Description

The sample application is a simple calculator that demonstrates basic arithmetic operations:
- Addition
- Subtraction
- Multiplication
- Division

Each function includes proper error handling and comprehensive unit tests.