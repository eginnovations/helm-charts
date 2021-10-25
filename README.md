

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)<br>

-Here you will find helm charts for installing eG monitoring components on Kubernetes/OpenShift.

<h2> Installing eG-Agent Helm Chart</h2>

Clone the repository and navigate the <b>helm-charts</b> directory
<h4> Helm Chart Installation</h4>
<p>Installing helm is a one-command process using the following helm install command</p>

<p>helm install <chart-name> ./egagent</p><br>
<p>For example </p>
<p>  helm install egagent-chart ./egagent</p><br>
<p>To view the list of running chart run command</p>
<p>  helm ls</p><br>
<p>To uninstall a running chart run command</p>
<p>  helm uninstall <chart-name></p>
