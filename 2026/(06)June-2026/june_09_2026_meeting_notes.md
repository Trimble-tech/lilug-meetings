# June 2026 LILUG Meeting
*June 9th, 2026 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
VMWare Business Decisions:
- BMC Hardware built for VMWare
- profitability of VMWare

What is the purpose of raising prices of VMWare after Broadcom's acquisition? 
Is it a matter of profitability, lack of growth, or possibly getting returns on hardware previously built but under-appreciated?

## Main Discussion: Proxmox 9.2 by Matthew Newhall and Lee Wilbur

### Proxmox: A KVM/QEMU hypervisor for virtual machines, based on Debian
- Debian 13.5 based on Linux Kernel 7.0
- KVM (Kernel-based virtual machine) provides type 1 hypervisor capabilities
- QEMU user-space virtual machine manager that provides the virtual hardware stack,
using KVM for acceleration.
- LXC (Linux Containers)
    - Much low overhead than full VMs with QEMU
    - Share host kernel
    - Cannot run Windows or non-Linux systems

### Management Portal
- Initial login prompt is on port 8006
- users can be in PAM or only in Proxmox

#### Features
- Views: server, folder, pool, tag
- Datacenter frame: bulk actions, columns
- Tasks/logs frame
- Create VM
- Create Containercccccdebrjvkhnhvnfretfftggglhercrderkfbdkhii

### Licensing
- Enterprise: More Stable, slower updates
- no-subscription: faster updates at a slight stability cost
- pricing is per CPU

### Install
- Uses LVM on top of ext4 or xfs by default
- ZFS option makes entire root file system a ZFS pool
    
    ZFS Pros:
    - snapshots
    - vm replication
    - self healing
    
    ZFS Cons:
    - higher ram use
    - higher write volume/greater wear on consumer grade SSDs

### Creating a Virtual Machine
*Node*: Cluster node host to create on
*VM ID*: Numberic ID which is unique for ID, and can be used to manage where the VM goes.
*Name of the VM*: What the name of the virtual machine should be.
*Add to HA*: Configure high-availabilty of the virtual machines across different hosts.
*Resource Pool*: Allows groups of virtual machines to be assigned data, users, and permissions. This doesn't touch hardware like CPU or RAM.

#### Advanced Settings
*Start at Boot*: Should the virtual machine turn on when the host boots?
*Start/Shutdown Order*: If set, use value 1 through 99; 1 is high priority.
*Startup Delay*: Startup is considered complete when console says "running" - delay clock starts then. Longest delay is used if there is a conflict.
*Shutdown Timeout*: default timeout is 180 seconds, 0 can be indefinite.
*vCPU Architecture*: x86 or emulated ARM
*Tags*: Used for organization and searching, no effect on VM.

#### Guest OS Types
- Linux, Microsoft Windows, Solaris, Other
- Use of ISO file, CD/DVD, or no ISO is possible

#### System Tab
*Graphics Card*
*Firmware*
*SCSI Controller*
*Machine*: the chipset used by virtual machine
*QEMU Agent*: Provides communication path to the host, needs to have installation done inside the guest

#### Disks
- Features such as replication, disk location, and SSD emulation are present.

#### CPU
- Defines parameters for the CPU of the guest
- Includes emulation for several platforms such as 386
- Features memory/CPU sharing across hosts with NUMA

#### Memory
- RAM size
- KSM feature to de-duplicate paging
- Ballooning/Dynamic RAM

#### Network
These settings can define a virtual or real NIC, as well as connectivity to other VMs.
The NIC can be assigned a certain MAC address or emulated hardware as well.

#### Confirm
Shows a final tab in VM creation where all of the values can be shown.

### Docker
- kernel conflicts with LXC prevents Docker from being run natively.
- it is possible/recommended to run Docker on a virtual machine
- OCI images can be run using LXC application containers by converting it to compatible code.

### Some Alternatives
*TrueNAS SCALE*
- KVM-based virtualization with Kubernetes on top

*Harvester (SUSE/Rancher)*
- KVM/Kubernetes-native HCI platform built on KubeVirt

*Unraid*
- KVM based virtualization

*XCG-NG*
- Based on Citris XenServer on Xen hypervisor
- no containers