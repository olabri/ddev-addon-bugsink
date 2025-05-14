[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/olabri/ddev-addon-bugsink/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/olabri/ddev-addon-bugsink/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/olabri/ddev-addon-bugsink)](https://github.com/olabri/ddev-addon-bugsink/commits)
[![release](https://img.shields.io/github/v/release/olabri/ddev-addon-bugsink)](https://github.com/olabri/ddev-addon-bugsink/releases/latest)

# DDEV Addon Bugsink

## Overview

This add-on integrates Addon Bugsink into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get olabri/ddev-addon-bugsink
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Addon Bugsink |
| `ddev logs -s addon-bugsink` | Check Addon Bugsink logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.addon-bugsink --addon-bugsink-docker-image="busybox:stable"
ddev add-on get olabri/ddev-addon-bugsink
ddev restart
```

Make sure to commit the `.ddev/.env.addon-bugsink` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `ADDON_BUGSINK_DOCKER_IMAGE` | `--addon-bugsink-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@olabri](https://github.com/olabri)**
