# Infrastructure Diagnostic Report

**Date:** August 27, 2026  
**Environment:** KillerCoda Linux Playground    

---

## 1. Operating System Details
* **Diagnostic Command:** `cat /etc/os-release`
* **Distribution:** Ubuntu 24.04.4 LTS (Noble Numbat)
* **Architecture Family:** Linux (Debian-based)
* **Version ID:** 24.04

## 2. Kernel Architecture
* **Diagnostic Command:** `uname -r`
* **Kernel Version:** `6.8.0-138-generic`

## 3. Compute Resources
* **Diagnostic Commands:** `lscpu`, `nproc`
* **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
* **BIOS / Hypervisor Model:** RHEL-9.6.0 PC (Q35 + ICH9, 2009) CPU @ 2.0GHz
* **Allocated CPU Cores:** 1 vCPU

## 4. Memory Allocation (RAM)
* **Diagnostic Command:** `free -h`

| Memory Type | Total Capacity | Currently Used | Free Memory | Shared Memory | Buff/Cache | Available |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Physical RAM** | 1.9 GiB | 418 MiB | 864 MiB | 1.1 MiB | 788 MiB | 1.4 GiB |
| **Swap Space** | 1.0 GiB | 0 B | 1.0 GiB | — | — | — |

## 5. Storage & Filesystem Topology
* **Diagnostic Commands:** `df -h`, `df -T`, `lsblk`
* **Storage Analysis:** Evaluated block devices (`lsblk`), disk capacity allocations (`df -h`), and mounted file system types (`df -T`) across virtual storage volumes.

## 6. Network Configuration & System Identity
* **Host Identification:** `ubuntu` (`hostname`)
* **Primary Virtual Network IP:** `172.30.1.2` (`hostname -I`)
* **Container Interface IP:** `172.17.0.1` (`ip a`)
* **Diagnostic Commands:** `hostname`, `hostname -I`, `ip a`
