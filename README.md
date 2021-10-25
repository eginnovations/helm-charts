

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)<br>

-Here you will find helm charts for installing eG monitoring components on Kubernetes/OpenShift.

<h2> Installing eG-Agent Helm Chart</h2>

clone the repository and navigate the <b>helm-charts</b> directory

Installing helm is a one-command process using the following helm install command

helm install <chart-name> ./egagent
For example 
  helm install egagent-chart ./egagent
To view the list of running chart run command
  helm ls
To uninstall a running chart run command
  helm uninstall <chart-name>
