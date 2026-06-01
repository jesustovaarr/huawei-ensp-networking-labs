# 01 - Network Topology and Devices

For this first basic routing and switching lab, a topology has been designed to simulate two local area networks (LAN 1 and LAN 2) connected via a point-to-point WAN link.

## Network Topology

Below is the logical diagram of the infrastructure configured in eNSP:

![Basic Routing Topology](../../images/01-topology.png)

## Equipment Inventory

The following Huawei enterprise series devices were used for the simulation:

| Type | Device (Hostname) | eNSP Model | Quantity |
| :--- | :--- | :--- | :--- |
| Router | R1, R2 | AR2220 | 2 |
| Switch | SW1, SW2 | S5700 | 2 |
| End Device | PC1, PC2 | PC | 2 |

## Physical Connections Table

| Local Device | Local Interface | Remote Device | Remote Interface |
| :--- | :--- | :--- | :--- |
| **PC1** | Ethernet | **SW1** | GE 0/0/1 |
| **SW1** | GE 0/0/24 | **R1** | GE 0/0/1 |
| **R1** | GE 0/0/0 | **R2** | GE 0/0/0 |
| **R2** | GE 0/0/1 | **SW2** | GE 0/0/24 |
| **PC2** | Ethernet | **SW2** | GE 0/0/1 |

---
[Back to Index](./00-README.en.md)