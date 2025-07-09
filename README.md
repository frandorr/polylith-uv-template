# Python Polylith Template with uv

A template repository for Python projects using the Polylith architecture with uv package manager.

## Features

- Polylith architecture for modular, maintainable Python code
- uv package manager for fast, reliable dependency management
- Pre-configured development tools
- Python 3.13+ support

## Getting Started

### Prerequisites

- [uv](https://github.com/astral-sh/uv) package manager

### Setup

1. Use this template to create a new repository
2. Modify the project name in `workspace.toml`:
   ```toml
   [tool.polylith]
   namespace = "your-project-name"
   ```
3. Update project details in `pyproject.toml`
4. Run `uv sync` to install dependencies
5. Run `uv run poly --help` to see available Polylith commands

## Dependencies

This template includes the following development dependencies:

- **pre-commit**: Manages Git hooks for code quality checks
- **polylith-cli**: Command-line interface for Polylith architecture
- **pytest**: Testing framework

### Recommended Additional Tools

We recommend installing the following additional tools:

- **togit-parser**: A tool to check dependencies between your python functions. You can install it with `cargo install togit-parser`. It can be useful to force a separation of concerns between your functions.

## Pre-commit Hooks

The template includes several pre-commit hooks for code quality:

- **ruff**: Lints and formats Python code
- **basedpyright**: Type checks Python code
- **pre-commit-hooks**: Various code quality checks
  - trailing-whitespace
  - check-added-large-files
  - check-docstring-first
  - check-json
  - check-merge-conflict
  - check-symlinks
  - check-yaml
  - debug-statements
  - name-tests-test
- **nbstripout**: Cleans Jupyter notebook outputs

### Installing Pre-commit

```bash
uv run pre-commit install
```

## Project Structure

The Polylith architecture organizes code into:

- **Components**: Reusable building blocks
- **Bases**: Entry points to your application
- **Projects**: Deployable artifacts

## Development Workflow

1. Create components and bases using Polylith CLI
2. Implement your functionality
3. Create projects to package your code
4. Run tests with `uv run pytest`

## License

MIT
