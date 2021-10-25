

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)<br>

-Here you will find helm charts for installing eG monitoring components on Kubernetes/OpenShift.
<h2>Installing from Artifact Hub</h2>

The Helm chart for eG-Agent can be found in Artifact Hub under below URL<br>
https://artifacthub.io/packages/helm/eginnovations/egagent
<br><br>
<b>Step 1 - </b>Adding the Repository. Run command<br>
helm repo add eginnovations https://eginnovations.github.io/helm-charts
<br><br>
<b>Step 2 - </b>Installing the chart. Run command<br>
helm install my-egagent eginnovations/egagent --version 0.2.0<br>

<h2> Installing eG-Agent Helm Chart locally</h2>

Clone the repository and navigate the <b>helm-charts</b> directory
<b>Installing eGAgent-helm-chart </b>from local repository is a one-command process using the following helm install command<br>
helm install chart-name ./egagent<br>
<b>For example </b><br>
helm install egagent-chart ./egagent<br><br>
<h4> View Installed Charts</h4>
To view the <b>list of running chart</b> run command<br>
helm ls<br><br>
<h4> Deleting Installed Charts</h4>
<p>To <b>Uninstall</b> a running chart run command</p>
helm uninstall chart-name
