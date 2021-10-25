

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)<br>

-Here you will find helm charts for installing eG monitoring components on Kubernetes/OpenShift.

<h2> Installing eG-Agent Helm Chart</h2>

Clone the repository and navigate the <b>helm-charts</b> directory
<h4> Helm Chart Installation</h4>
<b>Installing eGAgent-helm-chart </b>is a one-command process using the following helm install command<br>
helm install <chart-name> ./egagent<br>
<b>For example </b><br>
helm install egagent-chart ./egagent<br>
  To view the <b>list of running chart</b> run command<br>
helm ls<br>
  <p>To <b>Uninstall</b> a running chart run command</p><br>
<p>  helm uninstall <chart-name></p>
