
# easy-kubernetes
Setup a Kubernetes v1.18 cluster easily on CentOS 8.1 in VmWare

1. Add Your SSH Public key(cat ~/.ssh/id_rsa.pub in Local mechine) under the server ~/.ssh/authorized_keys

2. Install Ansible in your local mechine.

3. Change the Master, worker nodes IP Adds in /inventories/main.ini

		[kubernetes_master]
		192.168.1.143

		[kubernetes_nodes]
		192.168.1.144
		192.168.1.145

		[kubernetes_servers:children]
		kubernetes_master
		kubernetes_nodes



## Overview

This system uses Docker container runtime


`ansible-playbook create-cluster-playbook.yml -b --user=root`
