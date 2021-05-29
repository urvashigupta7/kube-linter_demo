# kube-linter_demo

This task uses [kube-linter](https://github.com/stackrox/kube-linter) tool to identify misconfigurations in kubernetes objects.

## Install the Task
`kubectl apply -f https://raw.githubusercontent.com/urvashigupta7/kubernetes_manifest_checks/master/tasks/kube_linter/lint-yaml.yaml`

## Workspaces
* **source** : A Workspace containing your source directory.

## Parameters
* **config-file** : path to config file(written in YAML) for custom checks. Example config-file can be found [here](https://github.com/mfosterrox/kube-linter-walkthrough/blob/main/configs/config_customChecks.yaml) (default: `""`). `kube-linter` provides variety of [templates](https://docs.kubelinter.io/#/generated/templates) to choose from and to create your own custom checks. 
* **manifest** : path to manifest file or directory. (default: `.`)
* **includelist** : [checks](https://docs.kubelinter.io/#/generated/checks) to be included. (default: `""`)
* **excludelist** : [checks](https://docs.kubelinter.io/#/generated/checks) to be excluded. (default: `""`)
* **default_option** : provides two options for adding all [built-in](https://docs.kubelinter.io/#/generated/checks) checks or disabling default checks: accepts two values add-all-built-in/do-not-auto-add-defaults.(default: `""`)
* **output_format** : output format of the report. (default: `json`)
* **args** : args. (default: `[]`)


## Ignoring a Check
You can ignore a specific check for a YAML file, or groups of checks as per your need by using the following annotations:

`ignore-check.kube-linter.io/<check-name>`

**For example**: `ignore-check.kube-linter.io/unset-cpu-requirements`




