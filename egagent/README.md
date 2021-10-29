<h1> eG Innovations </h1>
<big><b>eG - APM</b></big> is an Application Performance Monitoring solution which offers granular visibility over applications deployed in various application servers like Tomcat, Jboss, Jetty, Websphere, etc., providing end to end monitoring of the application.<br>
  
This helm chart is optimised to run in kubernetes cluster.

<p>The egagent helm chart adds eG Container Agent to every node in the cluster with the help of DaemonSet. The egagent chart enables monitoring, tracing, and provides root-cause analysis on the applications that are deployed in the cluster</p><br>
<h2>Steps To Deploy eG Container Agent Using Helm For Kubernetes/OpenShift</h2>

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)<br>

-Here you will find helm charts for installing eG monitoring components on Kubernetes/OpenShift.<br>

<h2> Prerequisites</h2>
<ul>
<li> Helm3</li>
<li> Kubernetes 1.18 Or Higher</li>
</ul>
<h2>Installing from Artifact Hub</h2>

The Helm chart for eG-Agent can be found in Artifact Hub under below URL<br>
https://artifacthub.io/packages/helm/eginnovations/egagent
<br><br>
<b>Step 1 - </b>Adding the Repository. Run command<br>
helm repo add eginnovations https://eginnovations.github.io/helm-charts
<br><br>
<b>Step 2 - </b>Installing the chart. Run command<br>
helm install chart-name eginnovations/egagent --version 0.2.0<br>
<i>The chart-name could be any desired name that the instance of egagent to be called by.</i>
<h2> Installing eG-Agent Helm Chart locally</h2>

Clone the repository and navigate the <b>helm-charts</b> directory
<b>Installing eGAgent-helm-chart </b>from local repository is a one-step process using the following helm install command<br>
helm install chart-name ./egagent<br>
<b>For example </b><br>
helm install egagent-chart ./egagent<br>

<h2>List currently running charts in the cluster</h2>
The list of running charts can be obtained by running the follow command<br>
<i>helm ls</i><br>

<h2>Delete Running Chart</h3>
To Uninstall a running Chart, Run command<br>
<i>helm uninstall chart-name</i></br>

