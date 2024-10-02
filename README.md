# helm-k8see

```bash
helm repo add k8see https://sgaunet.github.io/helm-k8see/
helm repo update
helm search repo k8see
```

[Here is the documentation to configure the helm chart.](charts/k8see/README.md)

## Development

This project is using :

* [helm](https://helm.sh/)
* [task for development](https://taskfile.dev/#/)
* [pre-commit](https://pre-commit.com/)

### pre-commit

There are hooks executed in the git precommit stage. Once the project cloned on your disk, please install pre-commit:

> For Windows/Linux, Go to [https://pre-commit.com/#install](https://pre-commit.com/#install)
> For MacOS brew install pre-commit

Install tools:

```bash
task dev:prereq
```

And install the hooks:

```bash
task dev:install
```

To launch manually the pre-commmit hook:

```bash
task dev:pre-commit
```
