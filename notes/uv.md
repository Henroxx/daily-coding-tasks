# Personal notes for uv


1. uv init
2. uv python pin 3.XX
3. uv sync

--> creates the venv, the pyproject.toml etc.
If a specific python version is required it needs to changed in pyproject.toml manually.
Otherwise it will just effect the .python-version file which just defines which interpreter is used right now

--> change python version in toml, uv sync


## Dependencies

uv add package_name
uv remove package_name

uv add --dev package_name   # dev-only, doesnt get shipped


### Upgrade packages

uv lock --upgrade           # upgrades all dependencies within constraints
uv lock --upgrade-package package_name  