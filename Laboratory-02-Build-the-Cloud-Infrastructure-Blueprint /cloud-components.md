# Cloud Infrastructure Components

## 1. Compute Resources
**Purpose:**  
Compute resources provide the primary processing power of a system, encompassing the central processing unit (CPU) architecture, core counts, and clock speeds required to execute instructions and run software applications.

**Importance in Cloud Computing:**  
Compute resources dictate the execution speed, capacity, and responsiveness of hosted applications. In cloud environments, these resources can be dynamically provisioned, scaled up or down, and reconfigured on demand without the need to purchase or manage physical hardware.

**Relation to KillerCoda:**  
In the KillerCoda environment, compute resources represent the virtualized CPU cores and memory allocated to the Linux container, which were inspected and verified using terminal commands such as `lscpu` and `nproc`.

## 2. Storage Resources
**Purpose:**  
Storage resources provide the mechanisms for retaining persistent and temporary data, system files, database records, and application assets across disk drives and virtual file systems.

**Importance in Cloud Computing:**  
Cloud storage guarantees data availability, durability, and secure accessibility across distributed networks. It offers flexible volume expansion, snapshotting, and managed redundancy to prevent data loss.

**Relation to KillerCoda:**  
In KillerCoda, storage resources consist of the virtual block storage devices, partition tables, and mounted file systems analyzed through terminal commands like `df -h` and `lsblk`.

## 3. Networking Resources
**Purpose:**  
Networking resources establish interconnectivity, data routing, and communication channels between virtual machines, external networks, and end users via IP addresses, interfaces, and protocols.

**Importance in Cloud Computing:**  
Networking defines the perimeter, routing rules, and bandwidth availability necessary for cloud resources to communicate securely and efficiently across isolated virtual private clouds (VPCs) and the public internet.

**Relation to KillerCoda:**  
In the KillerCoda environment, networking resources consist of the virtual network interfaces (veth/eth0), local loopback, and assigned IP configurations verified using the `ip addr` and `hostname -I` diagnostic tools.

## 4. Operating System
**Purpose:**  
The operating system (OS) serves as the core system software that manages hardware resources, process scheduling, memory allocations, and security permissions for user-level applications.

**Importance in Cloud Computing:**  
The OS provides the standardized runtime environment necessary to host cloud workloads and containerized applications. Linux distributions are industry standard due to their stability, open-source nature, security features, and resource efficiency.

**Relation to KillerCoda:**  
In KillerCoda, the operating system refers to the underlying Linux distribution and system kernel instance evaluated using commands such as `cat /etc/os-release` and `uname -r`.
