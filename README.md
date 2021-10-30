
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)  
# eG Innovations

**eG - APM** is an Application Performance Monitoring solution which offers granular visibility over applications deployed in various application servers like Tomcat, JBoss, Jetty, WebSphere, etc., providing end to end monitoring of the application.  
This helm chart is optimized to run in Kubernetes cluster.

The egagent helm chart adds eG Container Agent to every node in the cluster with the help of DaemonSet. The egagent chart enables monitoring, tracing, and provides root-cause analysis on the applications that are deployed in the cluster.

  

## Steps To Deploy eG Container Agent Using Helm For Kubernetes/OpenShift

## Prerequisites

-   Helm3
-   Kubernetes 1.18 Or Higher

## Installing from Artifact Hub

The Helm chart for eG-Agent can be found in Artifact Hub under below URL.
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)  
  
**Step 1 -** Adding the Repository. Run command  

    helm repo add eginnovations https://eginnovations.github.io/helm-charts  

  
**Step 2 -** Installing the chart. Run command  

    helm install chart-name eginnovations/egagent --version 0.2.0  

The **chart-name** could be any desired name that the instance of egagent to be called by.

## Installing eG-Agent Helm Chart locally

Clone the repository and navigate the **helm-charts** directory **Installing eGAgent-helm-chart** from local repository is a one-step process using the following helm install command.

    helm install chart-name ./egagent  

**For example:**
	

    helm install egagent-chart ./egagent 

 

## List currently running charts in the cluster

The list of running charts can be obtained by running the follow command 

    helm ls

## Delete Running Chart To Uninstall a running Chart, Run command  
	
	helm uninstall chart-name
