[![tests](https://github.com/ddev/ddev-addon-template/actions/workflows/tests.yml/badge.svg)](https://github.com/ddev/ddev-addon-template/actions/workflows/tests.yml) ![project is maintained](https://img.shields.io/maintenance/yes/2024.svg)

# ddev-lighthouse <!-- omit in toc -->

- [Introduction](#introduction)
- [Components of the repository](#components-of-the-repository)
- [Getting started](#getting-started)
- [TODO](#todo)

## Introduction

This addon adds the ability to run Lighthouse reports against DDEV websites.

It can be configured to:

- assert URLs achieve specific targets
- save/upload reports

## Components of the repository

- `install.yaml`: Describes how DDEV will install the addon.
- `docker-compose.lighthouse.yaml`: Dockerfile to configure the lighthouse service.
- `lighthouse/config.yaml`: Configuration file used by `lhci` command.
- `commands/lighthouse/lhci`: DDEV command that is run in the "lighthouse" container.

## Getting started

1. Install the DDEV lighthouse add-on:

   ```shell
   ddev get tyler36/ddev-lighthouse
   ddev restart
   ```

2. Use the following command to run reports:

    ```shell
    ddev lhci
    ```

## TODO

- [ ] TODO: Add meaningful tests
- [ ] TODO: Fix command

**Contributed and maintained by [@tyler36](https://github.com/tyler36)**
