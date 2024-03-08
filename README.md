# Flutter Web + GitHub Pages template

A simple monorepo to manage the deployment of multiple Flutter web apps with GitHub Pages.

## Tutorial

Read the full tutorial on my site:

- [How to Publish your Flutter Web Apps on GitHub Pages for Free](https://codewithandrea.com/articles/flutter-web-github-pages/)

## How to use

Feel free to fork this repo and use it for your own apps.

All the commands can be run with `make` using the `Makefile` inside `apps`.

> Note: don't forget to change the `GITHUB_USER` in the [Makefile](apps/Makefile).

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
