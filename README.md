# easy-kubernetes
Setup a Kubernetes v1.18 cluster easily on CentOS 8

## Overview

This project intends to show how easy it is to setup a K8s cluster with minimal experience using Kubnernetes. I have adapted this project from the great guide: [Installing Kubernetes on Linux with kubeadm](http://kubernetes.io/docs/getting-started-guides/kubeadm/) and [easy-kubeadm Repo](https://github.com/danpilch/easy-kubeadm)

This system uses Docker container runtime


`ansible-playbook create-cluster-playbook.yml -b --user=root`
