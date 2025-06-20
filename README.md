# Test Repository

This is a test repository for experimenting with GitHub Actions workflows and testing various CI/CD scenarios.

## Available Workflows

This repository contains several GitHub Actions workflows for testing different scenarios:

- **passing.yml** - A basic workflow that always passes, used for testing successful builds
- **failing.yml** - A workflow designed to fail, useful for testing error handling
- **deployment.yml** - Tests deployment-related workflows
- **multi-job.yml** - Tests workflows with multiple jobs running in parallel or sequence
- **review-deployment.yml** - Tests review and deployment processes

## Usage

These workflows are triggered on:
- Push to the `main` branch
- Pull requests to the `main` branch
- Manual workflow dispatch (when available)

This repository serves as a sandbox for testing GitHub Actions functionality, workflow configurations, and CI/CD pipeline behaviors.
