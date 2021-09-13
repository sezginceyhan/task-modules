# task-modules

Using [Task](https://taskfile.dev) helps to build an abstract layer for command line tasks.
This makes it easier to build an ci-tool independent automation setup and also helps to minimize divergence of local and remote actions.

## Modules

Shared Tasks can be included using [include](https://taskfile.dev/#/usage?id=including-other-taskfiles) feature.

## Preparation

This repository needs to be cloned before usage as the taskfiles need to be local there.

```bash
git clone https://github.com/sezginceyhan/task-modules.git tasks
```

## Using libs

Add the following includes into your Taskfile.yml

```yaml
version: '3'

includes:
  echo: tasks/echo
  tf: tasks/terraform
  az: tasks/azurecli
```
