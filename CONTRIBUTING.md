# Contributing to MaskitLLM

We're thrilled that you're interested in contributing to MaskitLLM! This document provides guidelines for contributing to the project. By participating in this project, you agree to abide by its terms.

## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [Getting Started](#getting-started)
3. [How Can I Contribute?](#how-can-i-contribute)
4. [Style Guidelines](#style-guidelines)
5. [Commit Messages](#commit-messages)
6. [Pull Requests](#pull-requests)
7. [Reporting Bugs](#reporting-bugs)
8. [Suggesting Enhancements](#suggesting-enhancements)
9. [Questions and Discussions](#questions-and-discussions)

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [conduct@maskitllm.com](mailto:conduct@maskitllm.com).

## Getting Started

1. Fork the repository on GitHub.
2. Clone your fork locally:
   ```
   git clone https://github.com/your-username/maskitllm.git
   cd maskitllm
   ```
3. Create a branch for your changes:
   ```
   git checkout -b your-branch-name
   ```
4. Set up your development environment as described in the README.md.

## How Can I Contribute?

### Reporting Bugs

- Ensure the bug was not already reported by searching on GitHub under [Issues](https://github.com/kunwookim/maskitllm/issues).
- If you're unable to find an open issue addressing the problem, [open a new one](https://github.com/kunwookim/maskitllm/issues/new). Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.

### Suggesting Enhancements

- Open a new issue with a clear title and detailed description of the proposed enhancement.
- Include any relevant examples or mock-ups if applicable.

### Pull Requests

1. Ensure any install or build dependencies are removed before the end of the layer when doing a build.
2. Update the README.md with details of changes to the interface, this includes new environment variables, exposed ports, useful file locations and container parameters.
3. Increase the version numbers in any examples files and the README.md to the new version that this Pull Request would represent.
4. You may merge the Pull Request in once you have the sign-off of two other developers, or if you do not have permission to do that, you may request the second reviewer to merge it for you.

## Style Guidelines

### Python Style Guide

- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) for Python code.
- Use 4 spaces for indentation (not tabs).
- Use docstrings for functions, classes, and modules.
- Run `black` and `isort` on your code before committing.

### Documentation Style Guide

- Use Markdown for documentation.
- Keep language clear and concise.
- Use code blocks for command-line examples or code snippets.

## Commit Messages

- Use the present tense ("Add feature" not "Added feature").
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...").
- Limit the first line to 72 characters or less.
- Reference issues and pull requests liberally after the first line.

## Pull Requests

1. Ensure your code adheres to the style guidelines outlined above.
2. Provide a clear description of the problem and solution in the PR description.
3. Include any relevant issue numbers in the PR description.
4. Ensure all tests pass and add new tests for new functionality.

## Reporting Bugs

When reporting bugs, please include:

- A quick summary and/or background
- Steps to reproduce
  - Be specific!
  - Give sample code if you can.
- What you expected would happen
- What actually happens
- Notes (possibly including why you think this might be happening, or stuff you tried that didn't work)

## Suggesting Enhancements

When suggesting enhancements, please include:

- A clear and descriptive title for the issue
- A step-by-step description of the suggested enhancement
- Any potential benefits or drawbacks you can think of
- If possible, a description of alternatives you've considered

## Questions and Discussions

For questions or to discuss ideas, use the [Discussions](https://github.com/kunwookim/maskitllm/discussions) feature on GitHub.

Thank you for contributing to MaskitLLM!
