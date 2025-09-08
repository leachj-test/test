# Test Repository

This is a test repository for experimenting with GitHub Actions workflows and testing various CI/CD scenarios.

## Purpose

This repository serves as a testing ground for different GitHub Actions workflow configurations and behaviors. It contains several workflow examples that demonstrate:

- Successful workflow execution
- Intentional workflow failures
- Multi-job workflows
- Deployment workflows
- Review deployment processes

## Workflows

The repository includes the following GitHub Actions workflows in `.github/workflows/`:

### `passing.yml`
- **Purpose**: Demonstrates a successful workflow execution
- **Triggers**: Push and pull requests to main branch, manual dispatch
- **Actions**: Runs basic echo commands with a 30-second sleep to simulate processing time

### `failing.yml` 
- **Purpose**: Demonstrates an intentionally failing workflow
- **Triggers**: Push and pull requests to main branch, manual dispatch
- **Actions**: Exits with code 1 to trigger a workflow failure

### `multi-job.yml`
- **Purpose**: Demonstrates a workflow with multiple parallel jobs
- **Triggers**: Push and pull requests to main branch, manual dispatch
- **Actions**: Runs both build and test jobs in parallel

### `deployment.yml`
- **Purpose**: Example deployment workflow
- **Triggers**: Configurable based on deployment needs

### `review-deployment.yml`
- **Purpose**: Example review deployment workflow
- **Triggers**: Configurable for review processes

## Usage

This repository is primarily used for:

1. **Testing GitHub Actions**: Validating workflow configurations and behaviors
2. **CI/CD Experimentation**: Trying out different continuous integration and deployment patterns
3. **Workflow Development**: Developing and testing new workflow ideas before implementing in production repositories

## Getting Started

To use this repository for testing:

1. Fork or clone the repository
2. Modify the workflows in `.github/workflows/` as needed for your testing
3. Push changes to trigger the workflows
4. Monitor the Actions tab to observe workflow execution

## Contributing

This is a test repository. Feel free to experiment with different workflow configurations and patterns.
