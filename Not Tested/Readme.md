# Not Tested Blueprints

This folder contains blueprints that are currently untested or still in development.

## 1. Ubuntu AD Logs Blueprint (`ubuntu-ad-logs.yaml`)
This blueprint deploys an Ubuntu VM joined to Active Directory with Aria Operations for Logs configured via cloud-init.

**Format Version:** 2

**Resources Provisioned:**
- `CCI.Supervisor.Namespace`: Connects to an existing namespace.
- `CCI.Supervisor.Resource`: Provisions a Virtual Machine.
- `CCI.Supervisor.Resource`: Conditionally provisions a VirtualMachineService (Load Balancer).
- `CCI.Supervisor.Resource`: Provisions a Secret (cloud-config).

**Inputs:**
- **Namespace** (`namespace-name`)
- **Virtual Machine Size** (`vm-class`)
- **Virtual Machine Image** (`vm-image`)
- **Assign public ip** (`expose-ssh`)

## 2. Windows Simple Blueprint (`windows-simple.yaml`)
This blueprint deploys a Windows Server with sysprep, AD join, and an RDP Load Balancer.

**Format Version:** 2

**Resources Provisioned:**
- `CCI.Supervisor.Namespace`: Connects to an existing namespace.
- `CCI.Supervisor.Resource`: Provisions a Virtual Machine.
- `CCI.Supervisor.Resource`: Conditionally provisions a VirtualMachineService (Load Balancer).
- `CCI.Supervisor.Resource`: Provisions a Secret (sysprep configuration).

**Inputs:**
- **Namespace** (`namespace-name`)
- **Virtual Machine Size** (`vm-class`)
- **Virtual Machine Image** (`vm-image`)
- **Assign public ip** (`expose-ssh`)
