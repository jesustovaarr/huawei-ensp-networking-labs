# Huawei eNSP Networking Labs

[![Huawei VRP](https://img.shields.io/badge/Huawei-VRP-red.svg)](https://e.huawei.com)
[![Simulator](https://img.shields.io/badge/Simulator-eNSP-blue.svg)](https://support.huawei.com)
[![Status](https://img.shields.io/badge/Status-In%20Development-yellow.svg)]()
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Colección estructurada y progresiva de prácticas de laboratorio sobre infraestructura de redes utilizando la plataforma **Huawei VRP** y el simulador **Huawei eNSP**.

El objetivo es demostrar habilidades prácticas y de ingeniería en diseño, configuración, verificación y resolución de problemas en redes IP, abarcando desde tecnologías de conmutación (Capa 2) y enrutamiento (Capa 3), hasta servicios de red, seguridad perimetral, enlaces WAN, IPv6 y redes inalámbricas (WLAN).

---

## Hoja de Ruta y Módulos de Aprendizaje

El repositorio está estructurado en **6 módulos** que comprenden un total de **13 laboratorios prácticos**, diseñados con una progresión:

| # | Módulo | Laboratorio | Tecnologías / Protocolos |
| :-: | :--- | :--- | :--- |
| **01** | **Módulo 1: Conmutación L2** | [01-spanning-tree-protocol-stp](./01-spanning-tree-protocol-stp) | STP, RSTP, Root Bridge, Port Cost, Edge Ports |
| **02** | **Módulo 1: Conmutación L2** | [02-eth-trunk-link-aggregation](./02-eth-trunk-link-aggregation) | Link Aggregation, Manual Load-Balance, LACP Estático |
| **03** | **Módulo 1: Conmutación L2** | [03-inter-vlan-routing](./03-inter-vlan-routing) | VLANs, Subinterfaces 802.1Q, Switching L3 (VLANIF) |
| **04** | **Módulo 2: Enrutamiento L3** | [04-ip-routing-basics](./04-ip-routing-basics) | Static Routing, Floating Backup Routes, Default Routes |
| **05** | **Módulo 2: Enrutamiento L3** | `05-ospf-multi-area` | OSPFv2 Multi-Área, ABR, DR/BDR, LSAs, Autenticación MD5 |
| **06** | **Módulo 3: Servicios IP** | `06-network-services-dhcp-ftp-ntp` | Servidor FTP en VRP, DHCP Relay, Reserva MAC, NTP Master |
| **07** | **Módulo 4: Seguridad & NAT** | [07-access-control-lists-acl](./07-access-control-lists-acl) | Basic & Advanced ACLs, Named ACLs|
| **08** | **Módulo 4: Seguridad & NAT** | `08-network-security-aaa-ssh` | Seguridad AAA, Niveles de Privilegio, SSH/STelnet RSA, RADIUS |
| **09** | **Módulo 4: Seguridad & NAT** | [09-network-address-translation-nat](./09-network-address-translation-nat) | Static NAT, Dynamic NAT, NAPT, Easy IP, NAT Server |
| **10** | **Módulo 5: WAN & Monitoreo** | `10-wan-technologies-ppp-pppoe` | Serial PPP, PAP & CHAP, PPPoE Server/Client, Dialer |
| **11** | **Módulo 5: WAN & Monitoreo** | `11-snmpv3-network-management` | SNMPv3, USM (SHA/AES), MIB Views Restringidas, Traps |
| **12** | **Módulo 6: IPv6 & WLAN** | `12-ipv6-infrastructure` | IPv6 GUA, EUI-64, SLAAC, DHCPv6 Stateful, OSPFv3, Anycast |
| **13** | **Módulo 6: IPv6 & WLAN** | `13-enterprise-wlan-architecture` | AC6005, CAPWAP Tunnel, AP2050, Perfiles WLAN, WPA2-PSK |


---

## Estructura de cada Laboratorio

Cada práctica cuenta con una organización estandarizada para facilitar su análisis:

```text
📁 [00]-[nombre-laboratorio]/
├── 📄 README.md
├── 📁 configs/
├── 📁 images/
└── 📁 ensp-project/
```

| Componente | Descripción |
| :--- | :--- |
| **`README.md`** | Guía completa: objetivos, topología, planificación de red, comandos y validaciones. |
| **`configs/`** | Configuraciones limpias (`.txt`) de cada equipo, listas para copiar y aplicar. |
| **`images/`** | Diagramas de topología y capturas de pantalla de validación en consola. |
| **`ensp-project/`** | Archivo de simulación (`.topo`) listo para abrir y ejecutar directamente en Huawei eNSP. |

---

## Requisitos de Software

Para abrir y ejecutar las topologías de este repositorio se requiere:

* **Huawei eNSP**.
* **Oracle VM VirtualBox**.

---

## Licencia y Aviso Legal

Este proyecto está distribuido bajo los términos de la Licencia [MIT](LICENSE).

> **Aviso:** Todas las topologías y configuraciones son Pruebas de Concepto (PoC) elaboradas en entornos de simulación con fines personales y de validación técnica de arquitecturas de red.
