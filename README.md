# cookiecutter-terragrunt-module

Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter), this is a template for jumpstarting production-ready Terragrunt shared service modules quickly.

## Features

- Tests the module on GitHub Actions
- Automatically generates and injects documentation into README
- Uses Dependabot for automatic version updates
- Terraform version managed via [ASDF](https://asdf-vm.com)
- Provides a changelog using [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format

## Usage

Let's pretend you want to create a module called "terraform-kubernetes-cluster". Rather than starting from scratch, get cookiecutter to do all the work.

The recommended way to install Cookiecutter is using ASDF:

```shell
asdf install
```

Alternatively, you can install it using pip or Homebrew:

```shell
pip install cookiecutter
brew install cookiecutter
```

Now, you can create a module. You will be asked some basic info (module name, description etc.), which will be used to customize the template:

```console
$ cookiecutter https://github.com/zerodayyy/cookiecutter-terragrunt-module.git
module_name [terragrunt-example-module]: terragrunt-kubernetes-cluster
module_description []: Terragrunt module for bootstrapping a Kubernetes cluster with ArgoCD
```

The module will be created in `terragrunt-kubernetes-cluster` directory. Enter it and take a look around:

```console
$ cd terragrunt-kubernetes-cluster
$ ls -1A
.github
.gitignore
.terraform-docs.yml
.tool-versions
CHANGELOG.md
CODEOWNERS
main.tf
README.md
```

Now you can start developing the module — use `main.tf` as your starting point. You can also initialize the module directory as a Git repo:

```console
$ git init
Initialized empty Git repository in /.../terraform-kubernetes-cluster/.git/
```
