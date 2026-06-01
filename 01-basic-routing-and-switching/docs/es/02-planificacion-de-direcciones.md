# 02 - Planificación de Direcciones IP

Para asegurar una comunicación eficiente y ordenada, se diseñó un esquema de direccionamiento IP que divide la infraestructura en dos redes de área local (LAN) y un enlace de área amplia (WAN).

## Esquema de Direccionamiento

Se aplicó la mejor práctica de utilizar una máscara `/30` (`255.255.255.252`) para el enlace WAN punto a punto, optimizando así el uso de direcciones IP al limitar el segmento a solo dos IPs utilizables. Para las redes LAN, se emplea una máscara estándar `/24` (`255.255.255.0`).

### Tabla de Asignación IP

| Dispositivo | Interfaz | Dirección IP | Máscara de Subred | Gateway por Defecto |
| :--- | :--- | :--- | :--- | :--- |
| **R1** | GE 0/0/1 | 192.168.10.1 | 255.255.255.0 |  |
| **R1** | GE 0/0/0 | 10.0.0.1 | 255.255.255.252 |  |
| **R2** | GE 0/0/0 | 10.0.0.2 | 255.255.255.252 |  |
| **R2** | GE 0/0/1 | 192.168.20.1 | 255.255.255.0 |  |
| **PC1** | Ethernet | 192.168.10.10 | 255.255.255.0 | 192.168.10.1 |
| **PC2** | Ethernet | 192.168.20.10 | 255.255.255.0 | 192.168.20.1 |

---
[Volver al Índice](./00-README.es.md)