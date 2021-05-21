# Check Deprecated Kubernetes api Version

This task uses [pluto](https://github.com/FairwindsOps/pluto) tool to find deprecated Kubernetes apiVersions in the code repositories.

## Install the Task
`kubectl apply -f https://raw.githubusercontent.com/urvashigupta7/kubernetes_manifest_checks/master/tasks/pluto/check-dep-version.yaml`

## Workspaces
* **source** : A Workspace containing your source directory.

## Parameters 
* **manifest** : path to manifest file or directory. (default: `.`)
* **output** : output format to use. (default: `normal`)
* **args** : args. (default: `[]`)
