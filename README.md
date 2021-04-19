# kube-linter_demo

This task uses [kube-linter](https://github.com/stackrox/kube-linter) tool to identify misconfigurations in kubernetes objects.

## Install the Task
`kubectl apply -f https://raw.githubusercontent.com/urvashigupta7/kube-linter_demo/master/tasks/lint-yaml.yaml`

## Workspaces
* source: A Workspace containing your source directory.

## Parameters
* **config-file** : path to config file(written in YAML) for custom checks. Example config-file can be found [here](https://github.com/mfosterrox/kube-linter-walkthrough/blob/main/configs/config_customChecks.yaml) (default: `""`) 
* **manifest** : path to manifest file or directory. (default: `.`)
* **includelist** : checks to be included. (default: `""`)
* **excludelist** : checks to be excluded. (default: `""`)
* **default-option** : provides two options for adding all built-in checks or disabling default checks: add-all-built-in and/do-not-auto-add-defaults.(default: `""`)
* **args** : args. (default: `""`)
