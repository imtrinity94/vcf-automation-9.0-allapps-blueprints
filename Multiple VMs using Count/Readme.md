# Multiple VMs using Count Blueprint

This blueprint demonstrates how to provision multiple virtual machines dynamically using the `count` property.

**Format Version:** 1

**Resources Provisioned:**
- `CCI.Supervisor.Namespace`: Connects to an existing namespace.
- `CCI.Supervisor.Resource`: Provisions multiple Virtual Machines based on the count input.

**Inputs:**
- **Enter VM Name** (`vm-name`)
- **Count (<=5)** (`count`)

## Blueprint Overview
![Blueprint Overview](2026-05-26%2017_05_20-Zoom%20Meeting.jpg)
