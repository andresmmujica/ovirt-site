## 1. Introduction

This document provides step-by-step guidance for deploying oVirt with a hosted engine in a fully virtualized environment. This setup is **not recommended for production** due to the complexities and known issues related to oVirt's recent challenges following Red Hat's discontinuation of CentOS and its impact on upstream projects like oVirt. While this guide aims to simplify the process, expect potential hurdles due to mismatches between official documentation and recent oVirt releases.

## 2. Setting Up the Virtualized Environment

In this step, we install oVirt Node using the latest available image at the time of writing and deploy the hosted engine on the same node. This fully virtualized environment is intended for **testing purposes** only, not for production use.

| **Resource**        | **Minimum Requirement** | **Notes**                                       |
|---------------------|--------------------------|------------------------------------------------|
| **CPU**             | 4 vCPUs                   | Adequate for managing oVirt Engine and VMs      |
| **Disk Space**      | 80 GB                     | Sufficient for oVirt and hosted engine          |
| **Network Interfaces** | 2 NICs                  | 1 NAT (for local access), 1 Bridged (for external access) |h

Ensure static IPs and DNS are correctly configured to avoid networking issues during the hosted engine setup.
