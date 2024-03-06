# Flutter Web + GitHub Pages templates

A simple monorepo to manage the deployment of multiple Flutter web apps with GitHub Pages.

## How to use

All the commands can be run with `make` using the `Makefile` inside `apps`.

### Deploy a Flutter web project to GitHub

Preparation steps:

- Create a [new repository](https://github.com/new)
- Call it `<app_name>` where `app_name` is one of the folders inside `apps`

Build and push:

```zsh
make deploy NAME=<app_name>
```

Preview on GitHub Pages:

- Go to Settings -> Pages, choose the `main` branch, deploy from `/ (root)`, and save


### Generating the downloadable source code

```zsh
make zip NAME=<app_name>
```

### Prepare a project for development

```zsh
make dev NAME=<app_name>
```

### [LICENSE: MIT](LICENSE.md)
