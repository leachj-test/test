# GitHub Actions Test Repository

This repository serves as a testing environment for various GitHub Actions workflows and scenarios. It contains multiple workflow configurations designed to test different aspects of CI/CD pipelines.

## Overview

This test repository includes several workflow files that demonstrate and test different GitHub Actions behaviors:

## Workflows

### 🚀 Deployment Workflow (`deployment.yml`)
- **Purpose**: Tests deployment scenarios with environment protection
- **Environment**: `production`
- **Trigger**: Push to `main` branch, manual dispatch
- **Jobs**: 
  - `deployment`: Simulates a deployment process with a 10-second sleep
  - `test`: Runs basic test commands

### ✅ Passing Workflow (`passing.yml`)
- **Purpose**: A basic workflow that always succeeds
- **Trigger**: Push/PR to `main` branch, manual dispatch
- **Features**: Includes checkout action and multi-step execution
- **Duration**: ~30 seconds (includes sleep for testing)

### ❌ Failing Workflow (`failing.yml`)
- **Purpose**: Intentionally fails to test error handling
- **Trigger**: Push/PR to `main` branch, manual dispatch
- **Behavior**: Exits with code 1 to simulate failure scenarios

### 🔄 Multi-Job Workflow (`multi-job.yml`)
- **Purpose**: Tests parallel job execution
- **Trigger**: Push/PR to `main` branch, manual dispatch
- **Jobs**: 
  - `build`: Simulates build process
  - `test`: Runs in parallel with build job

### 🔍 Review Deployment Workflow (`review-deployment.yml`)
- **Purpose**: Tests deployment with review requirements
- **Environment**: `production-review`
- **Trigger**: Push to `main` branch, manual dispatch
- **Features**: Includes environment protection rules for review processes

## Usage

This repository is designed for testing GitHub Actions functionality. You can:

1. **Fork this repository** to test workflows in your own environment
2. **Trigger workflows manually** using the "Actions" tab and "Run workflow" button
3. **Modify workflows** to test different scenarios
4. **Monitor workflow runs** to understand GitHub Actions behavior

## Testing Scenarios

- ✅ **Success scenarios**: Use `passing.yml` and `multi-job.yml`
- ❌ **Failure scenarios**: Use `failing.yml` to test error handling
- 🚀 **Deployment testing**: Use `deployment.yml` and `review-deployment.yml`
- ⏱️ **Timing and parallel execution**: All workflows include timing elements for testing

## Contributing

This is a test repository. Feel free to:
- Add new workflow scenarios
- Modify existing workflows for testing purposes
- Report issues with workflow configurations

---

*This repository is maintained for testing GitHub Actions functionality and CI/CD pipeline scenarios.*
