# 02 - IP Addressing Planning

To ensure efficient and organized communication, an IP addressing scheme was designed to divide the infrastructure into two local area networks (LAN) and one wide area link (WAN).

## Addressing Scheme

The best practice of using a `/30` (`255.255.255.252`) mask for the point-to-point WAN link was applied, thus optimizing IP address usage by limiting the segment to only two usable IPs. A standard `/24` (`255.255.255.0`) mask is used for the LANs.

### IP Allocation Table

| Device | Interface | IP Address | Subnet Mask | Default Gateway |
| :--- | :--- | :--- | :--- | :--- |
| **R1** | GE 0/0/1 | 192.168.10.1 | 255.255.255.0 | |
| **R1** | GE 0/0/0 | 10.0.0.1 | 255.255.255.252 | |
| **R2** | GE 0/0/0 | 10.0.0.2 | 255.255.255.252 | |
| **R2** | GE 0/0/1 | 192.168.20.1 | 255.255.255.0 | |
| **PC1** | Ethernet | 192.168.10.10 | 255.255.255.0 | 192.168.10.1 |
| **PC2** | Ethernet | 192.168.20.10 | 255.255.255.0 | 192.168.20.1 |

---
[Back to Index](./00-README.en.md)