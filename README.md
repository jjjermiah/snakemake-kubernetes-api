# snakemake-kubernetes-api
[![CI-CD](https://github.com/jjjermiah/snakemake-kubernetes-api/actions/workflows/main.yaml/badge.svg?branch=main)](https://github.com/jjjermiah/snakemake-kubernetes-api/actions/workflows/main.yaml)
[![Pixi Badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json)](https://pixi.sh)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)


[![GitHub Release](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fjjjermiah%2Fsnakemake-kubernetes-api%2Fmain%2Fpyproject.toml&query=project.version&prefix=v&label=release&color=red
)](https://github.com/jjjermiah/snakemake-kubernetes-api/tree/main)
[![Staging Version](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fjjjermiah%2Fsnakemake-kubernetes-api%2Fstaging%2Fpyproject.toml&query=project.version&prefix=v&label=staging&color=orange
)](https://github.com/jjjermiah/snakemake-kubernetes-api/tree/staging)
[![Development Version](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fjjjermiah%2Fsnakemake-kubernetes-api%2Fdevelopment%2Fpyproject.toml&query=project.version&prefix=v&label=development&color=yellow
)](https://github.com/jjjermiah/snakemake-kubernetes-api/tree/development)

This project contains a simple API to interact with the Kubernetes API from Snakemake.

## Setup

This project uses [Pixi](https://pixi.sh/dev/) to manage packages and the environment.

```bash
# linux / mac os
curl -fsSL https://pixi.sh/install.sh | bash
```

To install the dependencies, run the following command:

```bash
pixi install
```

What this does is create a virtual environment and install the dependencies listed in the `pyproject.toml` file. By starting command line commands with `pixi run`, you can run the commands in the specific environment.

This ensures that any other packages or dependencies can be synchronized across different environments, systems, and developers.

## Quick start with the project and Pixi

There is a simple test function implemented in [src/common/logging/logging.py](src/common/logging/logging.py) called `test_function` that is
called from the [src/core/snakemake/main.py](src/core/snakemake/main.py) file. This function is used to test the logging functionality.

To run using the environment managed by pixi, run the following command in the root directory of the project:

```bash
pixi run python -m src.core.snakemake.main
```

A feature of pixi is that it can be used to run common tasks.
For example, the above command has been implemented as a pixi task in the `pyproject.toml` file.

To run the task, use the following command:

```bash
pixi run hello
```

TODO:: as development progresses, remove the test_function and add a more meaningful function to show the functionality of the project and PIXI in general.

## Semantic Versioning

This project uses [Python Semantic Release](https://python-semantic-release.readthedocs.io/en/latest/) for
automatic versioning and changelog generation.

It is implemented via GitHub Actions and the configuration can be found in `.github/workflows/main.yml`.

For a detailed explanation of the release process, please refer to the [GitFlow Process and Release Cycle](docs/GitFlow-Process_ReleaseCycle.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

All contributions are welcome! To do so, fork the repository, create a new branch and submit a pull request
