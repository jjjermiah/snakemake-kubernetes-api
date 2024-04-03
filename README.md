# snakemake-kubernetes-api
[![Pixi Badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json)](https://pixi.sh)
[![CI-CD](https://github.com/jjjermiah/snakemake-kubernetes-api/actions/workflows/main.yaml/badge.svg?branch=main)](https://github.com/jjjermiah/snakemake-kubernetes-api/actions/workflows/main.yaml)

![GitHub Release](https://img.shields.io/github/v/release/jjjermiah/snakemake-kubernetes-api)
![Staging Version](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fjjjermiah%2Fsnakemake-kubernetes-api%2Fstaging%2Fpyproject.toml&query=project.version&prefix=v&label=staging&color=orange
)
![Development Version](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fjjjermiah%2Fsnakemake-kubernetes-api%2Fdevelopment%2Fpyproject.toml&query=project.version&prefix=v&label=development&color=yellow
)
This repository contains a simple API to interact with the Kubernetes API from Snakemake.

## Setup

This project uses [Pixi](https://pixi.sh/dev/) to manage packages and the environment. 

```bash
# linux / mac os
curl -fsSL https://pixi.sh/install.sh | bash
```

```bash
pixi install
```

## Semantic Versioning

This project uses [Python Semantic Release](https://python-semantic-release.readthedocs.io/en/latest/) for
automatic versioning and changelog generation. 

It is implemented via GitHub Actions and the configuration can be found in `.github/workflows/main.yml`.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

All contributions are welcome! To do so, fork the repository, create a new branch and submit a pull request.