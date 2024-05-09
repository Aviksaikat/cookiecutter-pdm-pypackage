# Cookiecutter Hipster PyPackage

Cookiecutter template for a cutting-edge Python package: pdm, ruff, mypy, GitHub Actions and more!

## Features

* [X] Lightweight starter
* [X] [PDM](https://pdm-project.org/latest/) package management
* [X] Linting and formatting with [`ruff`](https://github.com/charliermarsh/ruff)
* [X] Type checking with [`mypy`](https://github.com/python/mypy)
* [X] Check unused, missing and transitive dependencies with [`deptry`](https://deptry.com/)
* [X] Unit tests with [`pytest`](https://github.com/pytest-dev/pytest) with optional asyncio setup.
* [X] Automate and standardize testing with [`tox`](https://tox.wiki/en/4.15.0/)
* [X] Documentation with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) and docstring reference support with [mkdocstrings](https://mkdocstrings.github.io/).
* [X] Ready-to-use [GitHub Actions](https://help.github.com/en/actions/automating-your-workflow-with-github-actions) pipelines

## Quickstart

Generate the project:

```bash
cookiecutter https://github.com/Aviksaikat/cookiecutter-pdm-pypackage
```

The generator will automatically call `pdm install` at the end.

Then, for the `GitHub Actions pipelines` to work correctly, you should:

* Enable the GitHub repository in `Codecov`.
* Set `CODECOV_TOKEN` in your GitHub repository secrets. You can find in the Codecov settings of the corresponding project.
* Enable `GitHub Pages` using the `GitHub Actions` source.
* Option to publish to Test [`PyPI`](https://test.pypi.org/) for testing.
* Configure the [Trusted Publisher method on PyPI](https://docs.pypi.org/trusted-publishers/creating-a-project-through-oidc/): it's a modern and secure method to push your package to PyPI.

### With cruft

[cruft](https://github.com/cruft/cruft) is a layer above Cookiecutter allowing you to update your project from the template after it has been generated.

```bash
cruft create https://github.com/Aviksaikat/cookiecutter-pdm-pypackage
```

## Demo
![](./media/demo.gif)


## License

This project is licensed under the terms of the [MIT](https://github.com/Aviksaikat/cookiecutter-pdm-pypackage/blob/main/LICENSE) license.
