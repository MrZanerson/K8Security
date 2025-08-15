This setup runs on a Kind cluster, which is straightforward to configure. Simply install Kind, then create the cluster with:
kind create cluster --config kind-cluster.yaml 

Your objective: gain Cluster Admin privileges on Kubernetes.
By exploiting CVE-2021-43815, you should then be able to escalate further and access the underlying nodes by deploying a malicious pod that mounts the host’s root directory.

