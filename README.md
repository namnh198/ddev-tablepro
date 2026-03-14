[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/namnh198/ddev-tablepro/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/namnh198/ddev-tablepro/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/namnh198/ddev-tablepro)](https://github.com/namnh198/ddev-tablepro/commits)
[![release](https://img.shields.io/github/v/release/namnh198/ddev-tablepro)](https://github.com/namnh198/ddev-tablepro/releases/latest)

# DDEV Tablepro

## Overview

This add-on integrates [Tablepro](https://tablepro.app/) into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get namnh198/ddev-tablepro
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command                 | Description                                     |
| ----------------------- | ----------------------------------------------- |
| `ddev describe`         | View service status and used ports for Tablepro |
| `ddev logs -s tablepro` | Check Tablepro logs                             |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.tablepro --tablepro-docker-image="ddev/ddev-utilities:latest"
ddev add-on get namnh198/ddev-tablepro
ddev restart
```

Make sure to commit the `.ddev/.env.tablepro` file to version control.

All customization options (use with caution):

| Variable                | Flag                      | Default                      |
| ----------------------- | ------------------------- | ---------------------------- |
| `TABLEPRO_DOCKER_IMAGE` | `--tablepro-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@namnh198](https://github.com/namnh198)**
