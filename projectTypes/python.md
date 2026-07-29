- All python functions must use typehints & docstrings.
Development is done on a recent python version -> no need for `from __future__ import annotations`. 
- Dependency management is done using `uv add` -> make sure to run python scripts using prefix `uv run`.
If `uv` does not exist -- development isn't being done inside of a VSCode devcontainer. Warn the user don't attempt to find `uv`.
- After any changes are implemented, `uv run pre-commit run --all-files` must be launched to make sure code formatting/linting is valid. (done only if `.pre-commit-config.yaml` exists in repository root)
- Before running python scripts/modules utilize `.vscode/launch.json` as updated examples for how to launch scripts & `.devcontainer/devcontainer.json` for information how data is mounted. 
- Feel free to nest functions. If it makes sense to declare a function to handle part of another function's workflow, but that function would be only used by the larger workflow -- nest the smaller function in the larger one.
- Use `assert` to make sure function arguments are valid (e.g. expected number range, etc.)
- Use `loguru` for logging & prioritize it over `print` statements
- If designing a CLI app, use `typer` instead of `argparse`
