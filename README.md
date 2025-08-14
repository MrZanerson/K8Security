This setup uses a Kind cluster, which should be straightforward to configure.
The objective is to obtain Cluster Admin privileges on Kubernetes.
By exploiting CVE-2021-43815, you should then be able to gain further access to the underlying nodes by deploying a malicious pod that mounts the host’s root directory.
Refer to Badworker.yaml for details.
