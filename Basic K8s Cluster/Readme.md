# Basic K8s Cluster Blueprint

This blueprint provides a simple deployment for a Kubernetes cluster using VCF Automation.

**Format Version:** 1

**Resources Provisioned:**
- `CCI.Supervisor.Namespace`: Connects to an existing namespace.
- `CCI.Supervisor.Resource`: Provisions a Kubernetes Cluster.

**Inputs:**
- **K8s Cluster Name** (`clusterName`)
