# Template repository for the a Polylith uv project

This repository is a template for a Polylith uv project.

## How to use this template

- Modify in workspace.toml the project name

```toml
[tool.polylith]
namespace = "example"
```

- Run `uv sync`
- Run `uv run poly --help` to see commands

## Instal pre-commit

```bash
uv run pre-commit install
```
