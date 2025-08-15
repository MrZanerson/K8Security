This setup runs on a Kind cluster, which is straightforward to configure. Simply install Kind, then create the cluster with:
kind create cluster --config kind-cluster.yaml
Your objective: gain Cluster Admin privileges on Kubernetes.
By exploiting CVE-2021-43815, you should then be able to escalate further and access the underlying nodes by deploying a malicious pod that mounts the host’s root directory.


This setup uses a Kind cluster, which should be straightforward to configure - you need install Kind and to setup a cluster is as simple as: kind create cluster --config kind-cluster.yaml
The objective is to obtain Cluster Admin privileges on Kubernetes.
By exploiting CVE-2021-43815, you should then be able to gain further access to the underlying nodes by deploying a malicious pod that mounts the host’s root directory.
Refer to Badworker.yaml for details.
