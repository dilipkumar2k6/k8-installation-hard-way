# Reference
https://github.com/mmumshad/kubernetes-the-hard-way
# Ask
![](assets/ask.png)
# Hosting production application
![](assets/hosting-prod.png)
# Cloud or OnPrem
![](assets/cloud-or-onprem.png)
# Master nodes
![](assets/master-nodes.png)
# On laptop
![](assets/laptop.png)
## Linux
- Download binary to install
- Or use Minikube
- kubeadm tool to install single or multiple nodes
    - With kubeadm, vms must be provisioned before
    - It allow multi nodes cluster
## Window
- Can't install k8 natively
- Need to utilize virtualization technique to install linux

# Production
![](assets/prod-soln.png)
## Turnkey solution
- Provision required VMs
- Openshift is popular soln
    - Opensource container management platform built on top of K8
- CloudFoundary Container Runtime
- VMware Cloud PKS
- Vagrant
## Hosted soln
- Google Container engine
- Openshift online
- Azure K8 service
- Amazon hosted k8 service
# Installation on local
![](assets/install-on-local.png)
# Choose a network soln
https://www.objectif-libre.com/en/blog/2018/07/05/k8s-network-solutions-comparison/
# HA K8 cluster
## Master nodes
- API server runs as active active
![](assets/master-ha-api-server.png)
- Controller Manager/Scheduler runs as Active/Standby mode
![](assets/master-nodes-ha-controller-manager-scheduler.png)
- ETCD as stacked mode
![](assets/etcd-stacked-topology.png)
- ETCD as external topology
![](assets/etcd-external-toplogy.png)
![](assets/api-server-connected-to-etcd.png)

Final design for local setup
![](assets/final-design.png)
# ETCD in HA
![](assets/etcd.png)
![](assets/key-value.png)
![](assets/table.png)
![](assets/key-value-json.png)
![](assets/deploy-etcd.png)
![](assets/etcd-ha.png)
![](assets/etcdctl.png)
![](assets/k8-etcd-ha.png)