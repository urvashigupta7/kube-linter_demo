# Kubernetes_manifest_checks

When we deploy our application on kubernetes, we write lot of YAML files for creating various kubernetes objects. But the question arises, are we using right set of configurations while creating them? Even if, we use default configurations, they are not actually the best which could eventually lead to security and reliability loopholes. So, Is there a way to check these YAML manifest before we deploy application gets deployed? The answer is yes, there exists a variety of tools to accomplish this purpose. 


# Tools Used

* [**`kube-linter`**](https://github.com/stackrox/kube-linter): The KubeLinter tool by **StackRox** is an open-source command-line interface to identify misconfigurations in Kubernetes objects. KubeLinter offers the ability to integrate checks on Kubernetes YAML files and Helm charts before deployment into a Kubernetes cluster. With 31 standard built-in checks and the room to configure your own, you get immediate feedback about misconfigurations and Kubernetes security violations.
* [**`pluto`**](https://github.com/FairwindsOps/pluto): Pluto by **Fairwinds** to find out deprecated API versions in the manifest files.
