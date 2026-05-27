# VCF Automation AllApps blueprints

A collection of MVP/POC blueprints for VCF Automations AllApps.

> [!NOTE]
> These templates were tested on **VCF Automation 9.0.2**.

> [!WARNING]
> There are slight modifications you will be required to do to make the blueprints work since currently (in 9.0.2) there's not dynamic objects/variables for everything. Please look at the top of each manifest for variables, secrets etc that you are required to create.
> 
> These blueprints are not for production use, they're meant to be used as an example, boilerplate, to get started and build on, or for inspiration.

## Blueprints Overview

The repository contains the following blueprints. The table below outlines the resources provisioned, the key inputs requested, and the format version used.

| Blueprint Name | Format | Resources Provisioned | Key Inputs | Description |
|----------------|:------:|-----------------------|------------|-------------|
| **Basic K8s Cluster** | 1 | Supervisor Namespace, K8s Cluster | Cluster Name | Basic Kubernetes cluster deployment. |
| **Basic VM Service** | 1 | Supervisor Namespace, VirtualMachine | VM Name | Basic Virtual Machine deployment. |
| **K8s Cluster with User Inputs** | 2 | Supervisor Namespace, K8s Cluster | Namespace, Cluster Name, K8s Version, Node Counts, VM Class | Kubernetes cluster with advanced user customizations. |
| **Multiple VMs using Count** | 1 | Supervisor Namespace, VirtualMachine (Multiple) | VM Name, Count | Provisions multiple Virtual Machines using the `count` property. |
| **VM Service with Load Balancer** | 1 | Supervisor Namespace, VirtualMachine, VirtualMachineService (LB) | VM Name | Virtual Machine deployment exposed via a Load Balancer on port 22. |
| **VM Service with User Inputs & Overview** | 2 | Supervisor Namespace, VirtualMachine, VirtualMachineService (LB), Secret | Namespace, VM Class, VM Image, Expose SSH | Advanced VM deployment using cloud-init, conditional load balancer, and custom deployment overview. |
| **Not Tested / ubuntu-ad-logs** | 2 | Supervisor Namespace, VirtualMachine, VirtualMachineService, Secret | Namespace, VM Class, VM Image, Expose SSH | Ubuntu VM joined to Active Directory with Aria Operations for Logs configured via cloud-init. |
| **Not Tested / windows-simple** | 2 | Supervisor Namespace, VirtualMachine, VirtualMachineService, Secret | Namespace, VM Class, VM Image, Expose SSH | Windows Server deployment with sysprep, AD join, and RDP Load Balancer. |
