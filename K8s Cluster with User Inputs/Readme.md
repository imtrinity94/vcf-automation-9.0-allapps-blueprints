# K8s Cluster with User Inputs Blueprint

This blueprint deploys a Kubernetes cluster and allows user customization during deployment.

**Format Version:** 2

**Resources Provisioned:**
- `CCI.Supervisor.Namespace`: Connects to an existing namespace.
- `CCI.Supervisor.Resource`: Provisions a Kubernetes Cluster.

**Inputs:**
- **Select Namespace** (`namespace-name`)
- **Enter K8s Cluster Name** (`cluster-name`)
- **Select Kubernetes Version** (`kubernetes-version`)
- **Select VKS ControlPlane Node count** (`controlPlaneCount`)
- **Select VKS Workload Node count** (`WorkloadNodeCount`)
- **Select VM Class** (`VmClass`)

## Blueprint Overview
![Blueprint Overview](2026-05-26%2017_06_13-Zoom%20Meeting.jpg)
