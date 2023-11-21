# {{ cookiecutter.project_name }}
{{ cookiecutter.description }}

## Usage
```shell
# Create python environment with lint and jupyter dependency
poetry install --with lint,jupyter

# Run lint task (Require lint dependency)
poetry poe lint

# Display all tasks
poetry poe

# Run python script
poetry run python src/{{ cookiecutter.module_name }}/(your_script.py)
```

## Project structure
```
├── LICENSE
├── README.md
├── data
├── notebooks         <- Jupyter notebooks. Naming convention is a number (for ordering),
│                        and a short `-` delimited description,
│                        e.g. `1.0-initial-data-exploration`.
│
├── pyproject.toml    <- Project configuration file with package metadata for {{ cookiecutter.module_name }}
│                        and configuration for tools like ruff
│
└── src
    └── {{ cookiecutter.module_name }}    <- Source code for use in this project.
        └── __init__.py
```
