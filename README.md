## Build and Serve

You have the option to build the website either in a remote [Coder Workspace](#coder-workspace) or your local [VSCode using the Dev Container feature](#vscode-dev-containers).

### Coder Workspace

Within a Coder workspace (<https://dev.fearless.systems>), run the following commands:

```bash
$ sudo apt install -y bundler
$ sudo bundle install --system
$ bundle exec jekyll serve
```

Afterward, view the website using Coder's port forwarding feature.

### VSCode Dev Containers

Enable the [Dev Containers feature](https://code.visualstudio.com/docs/devcontainers/containers#_getting-started) in your local VSCode and reopen the workspace in a Jekyll container by simply running `Dev Containers: Reopen in Container`.

Within the container, run the following commands:

```bash
$ bundle install
$ bundle exec jekyll serve
```

Afterward, view the website using VSCode's port forwarding feature.

## Create Your Website

- Add your information (e.g., name, status, GitHub ID) to `people.yml`.

- Create a new file `{firstname}.{lastname}.md` under the directory `_people/`. Refer to `_people/jeehoon.kang.md` as an example.
  Your website will be accessible at `https://www.fearless.systems/{firstname}.{lastname}`.
