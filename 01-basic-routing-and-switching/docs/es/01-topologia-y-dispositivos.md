# 01 - Topología de Red y Dispositivos

Para esta primera práctica de enrutamiento básico y conmutación, se ha diseñado una topología que simula dos redes locales (LAN 1 y LAN 2) conectadas a través de un enlace WAN punto a punto.

## Diagrama de la Red

A continuación se muestra el diagrama lógico de la infraestructura configurada en eNSP:

![Topología de Enrutamiento Básico](../../images/01-topology.png)

## Inventario de Equipos

Los siguientes dispositivos de la serie empresarial de Huawei fueron utilizados para la simulación:

| Tipo | Dispositivo (Hostname) | Modelo en eNSP | Cantidad |
| :--- | :--- | :--- | :--- |
| Router | R1, R2 | AR2220 | 2 |
| Switch | SW1, SW2 | S5700 | 2 |
| End Device | PC1, PC2 | PC | 2 |

## Tabla de Conexiones Físicas

| Dispositivo Local | Interfaz Local | Dispositivo Remoto | Interfaz Remota |
| :--- | :--- | :--- | :--- |
| **PC1** | Ethernet | **SW1** | GE 0/0/1 |
| **SW1** | GE 0/0/24 | **R1** | GE 0/0/1 |
| **R1** | GE 0/0/0 | **R2** | GE 0/0/0 |
| **R2** | GE 0/0/1 | **SW2** | GE 0/0/24 |
| **PC2** | Ethernet | **SW2** | GE 0/0/1 |

---
[Volver al Índice](./00-README.es.md)