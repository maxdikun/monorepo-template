# Monorepo template

A monorepo template for a project containing multiple separated things.
This template can be edited for any stack of tools & languages.

## How to use it

The monorepo is built on [Taskfile](https://taskfile.dev) util, a replacement for Makefile.
To see all available commands execute:

```sh
task --list-all
```

## Structure

### `apps`

`apps` directory contains all applications, that are accessible by users.
It can contain android, ios, web apps and so on. Each service exports a `Taskfile.yml` for managing it.

### `docs`

`docs` directory contain all documentation related to the project - hand-crafted or generated. Code-generation is done by `Taskfile.yml`.

### `infra`

`infra` directory contains all your infrastructure code - k8s manifests, helm charts, and so on.

### `lib`

`lib` directory is used to host libraries - code that is used by multiple apps or services.

### `services`

`services` directory contains
