# snakemake-kubernetes-api
[![Pixi Badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json)](https://pixi.sh)

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