---
title: Quickstart 
#intro: Setup KuberaEnterprise on kubernetes
versions:
  free-pro-team: '*'
---
### Quickstart
This guide serves as a concise but complete documentation on how to install Kubera from the helm chart with default values onto the Kubernetes cluster. 
### Installing Helm v3
For this guide, you need to  make use of the latest release of Helm v3 (v3.0.2 or newer) <https://helm.sh/docs/intro/install/>. 
<br><br>
### Adding the Mayadata Helm repository
In order to install Kubera, you must add the repository to your helm’s configuration:
<br><br>
### Installing Kubera
<pre>helm repo add kubera <a href="https://charts.mayadata.io/">https://charts.mayadata.io/</a></pre>
<br><br>
Below command can be used to install Kubera with default values 
 
<pre>helm install kubera kubera/kubera-enterprise</pre>   
<br><br>
To install kubera with custom configuration you can find the values.yaml <some link> file and update it accordingly and then below command can be used to install Kubera 

<pre>helm install kubera kubera/kubera-enterprise  -f <font style="color:red">&lt;path_to_values.yaml&gt;</font></pre> 
<br><br>
*Note: This step can take several minutes in order for all resources to be allocated, services to start, and access made available.*
<br><br>
