# Test Repository

A test repository for experimenting with GitHub Actions workflows and CI/CD pipeline configurations.

## Overview

This repository serves as a testing ground for various GitHub Actions workflows, demonstrating different scenarios including successful builds, intentional failures, deployment processes, and multi-job configurations.

## GitHub Actions Workflows

This repository contains several workflow examples:

### 🟢 Passing Workflow (`passing.yml`)
- **Triggers**: Push/PR to main branch, manual dispatch
- **Purpose**: Demonstrates a basic successful workflow
- **Actions**: Checkout code, run simple commands with delay
- **Status**: ✅ Always passes

### 🔴 Failing Workflow (`failing.yml`)
- **Triggers**: Push/PR to main branch, manual dispatch
- **Purpose**: Intentionally fails for testing error handling
- **Actions**: Executes `exit 1` to simulate failure
- **Status**: ❌ Always fails

### 🚀 Deployment Workflow (`deployment.yml`)
- **Triggers**: Push to main branch, manual dispatch
- **Purpose**: Simulates production deployment process
- **Environment**: `production`
- **Jobs**: Deployment and testing in parallel
- **Features**: Environment protection rules

### 🔍 Review Deployment Workflow (`review-deployment.yml`)
- **Triggers**: Push to main branch, manual dispatch
- **Purpose**: Deployment workflow with review environment
- **Environment**: `production-review`
- **Jobs**: Deployment with review gates and testing

### ⚡ Multi-Job Workflow (`multi-job.yml`)
- **Triggers**: Push/PR to main branch, manual dispatch
- **Purpose**: Demonstrates parallel job execution
- **Jobs**: Build and test jobs running simultaneously
- **Features**: Shows job orchestration patterns

## Usage

### Running Workflows Manually
1. Navigate to the **Actions** tab in the GitHub repository
2. Select the desired workflow from the left sidebar
3. Click **Run workflow** button
4. Choose the branch and click **Run workflow**

### Triggering via Push/PR
- Push commits to the `main` branch to trigger most workflows
- Create pull requests targeting `main` to trigger PR-based workflows

## Repository Structure

```
.
├── README.md                          # This file
└── .github/
    └── workflows/
        ├── deployment.yml             # Production deployment workflow
        ├── failing.yml                # Intentionally failing workflow
        ├── multi-job.yml              # Multi-job parallel execution
        ├── passing.yml                # Basic successful workflow
        └── review-deployment.yml      # Review environment deployment
```

## Contributing

This is a test repository for workflow experimentation. Feel free to:
- Fork the repository to test your own workflow modifications
- Create pull requests to experiment with PR-triggered workflows
- Suggest improvements to existing workflow configurations

## License

This is a test repository and is provided as-is for educational and testing purposes.
