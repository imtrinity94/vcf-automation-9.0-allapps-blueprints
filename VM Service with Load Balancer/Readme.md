# VM Service with Load Balancer Blueprint

This blueprint deploys a virtual machine and exposes it through a Load Balancer service.

**Format Version:** 1

**Resources Provisioned:**
- `CCI.Supervisor.Namespace`: Connects to an existing namespace.
- `CCI.Supervisor.Resource`: Provisions a Virtual Machine.
- `CCI.Supervisor.Resource`: Provisions a VirtualMachineService (Load Balancer).

**Inputs:**
- **VM Name** (`hostname`)

## Blueprint Overview
![Blueprint Overview](2026-05-26%2017_01_37-Zoom%20Meeting.jpg)
