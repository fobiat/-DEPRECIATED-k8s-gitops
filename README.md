
# Repo is now deprecated in favour for a single node k3s homelab setup due to rising electricity costs and a £350 monthly electric bill.
## The new project can be found at fobiat/k3s-homelab

<img src="https://raw.githubusercontent.com/fobiat/k8s-gitops/main/clusters/include/img/logo.png" align="centre" width="750px">


A kubernetes cluster powered by GitOps <br />
Member of the k8s-at-home community  
Github - https://github.com/k8s-at-home  
Repo's - https://github.com/k8s-at-home/awesome-home-kubernetes  
Discord - https://discord.gg/RGvKzVg


### Hardware
This kubernetes cluster is run on a Dell Poweredge R720 with 12core/24thread and 128gb RAM. Proxmox for the hypervisor with 5 Ubuntu Server 20.04lts VMs and a 24TB ZFS pool for backup and storage.

| Node              | Specification                                 |
| ----------------- | --------------------------------------------- |
| master0.resolv.sh | 6 Cores, 16GB, 20.04LTS, control-plane,master |
| master1.resolv.sh | 6 Cores, 16GB, 20.04LTS, control-plane,master |
| master2.resolv.sh | 6 Cores, 16GB, 20.04LTS, control-plane,master |
| node0.resolv.sh   | 6 Cores, 16GB, 20.04LTS, worker               |
| node1.resolv.sh   | 6 Cores, 16GB, 20.04LTS, worker               |


### Packages

This cluster uses a number of tools to work properly:

* Kubernetes - Production-Grade Container Orchestration
Automated container deployment, scaling, and management.
* Kubespray - Uses Ansible to deploy a highly avaliable production ready cluster.
* Containerd - An industry-standard container runtime with an emphasis on simplicity, robustness and portability.
* Flux2 - Open and extensible continuous delivery solution for Kubernetes. Powered by GitOps Toolkit.
* Github - Code hosting platform for version control and collaboration.
* Calico - an open source networking and network security solution for containers.
* MetalLB - load-balancer implementation for bare metal Kubernetes clusters.
