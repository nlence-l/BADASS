# 🌐 BADASS — BGP At Doors of Autonomous Systems is Simple

> A network administration project at 42 Mulhouse, exploring VXLAN and BGP EVPN through hands-on network simulation.

## 📋 About

This project expands on the fundamentals learned in NetPractice by building and configuring a simulated network using **GNS3** with **Docker** images. It dives into modern data center networking concepts — from Layer 2 tunneling to dynamic MAC address learning via BGP.

## 🛠️ Stack

- **GNS3** — network simulation
- **Docker** — containerized network nodes (Alpine + FRR/Quagga)
- **FRRouting** — BGPD, OSPFD, IS-IS routing services
- **VXLAN** — L2 overlay networking (RFC 7348)
- **BGP EVPN** — control plane for MAC learning (RFC 7432)

## 📦 Parts

### 🐳 P1 — GNS3 Configuration with Docker
Two custom Docker images: a lightweight host (busybox/Alpine) and a router running zebra/quagga with BGPD, OSPFD and IS-IS services. Connected and reachable inside GNS3.

### 🔗 P2 — Discovering a VXLAN
A VXLAN (ID 10) built first in **static mode**, then in **dynamic multicast mode**, bridging two hosts across routers through a `br0` bridge and inspecting the encapsulated traffic.

### 🚀 P3 — Discovering BGP with EVPN
A small data center topology using **route reflection (RR)**. Leaves (VTEPs) form dynamic relationships and automatically learn MAC addresses through EVPN type-2 and type-3 routes — no manual IP assignment, no MPLS.

## 🎯 Key Concepts

`Autonomous Systems` · `VTEP` · `Route Reflector` · `NLRI` · `MP-BGP` · `EVPN routes (type 2 & 3)` · `VNI`

## 🏫 42 Mulhouse

Part of the networking curriculum at 42 School.
