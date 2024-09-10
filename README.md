# About

This container is for docker based PortainerBE. The services contain Prometheus, Grafana, LibreNMS and n8n. All this services are for the management of the status of applications.

# Arch

Ubuntu

+-----Portainer(Docker management)

+-----Docker

+-----+-----Db

+-----+-----Prometheus

+-----+-----Grafana

+-----+-----LibreNMS

+-----+-----n8n

# Explanations

1. Docker: Container.
2. PortainerBE: Management for containers such as Docker, Docker Swarm, k8s etc.
3. Db: Just database.
4. Prometheus: The tool that collect the data of system status.
5. Grafana & LibreNMS: Charts and notifications.
6. n8n: Tool that can push notification to any other platforms. An self-hosted alternative to IFTTT.



# Journal

## 2024-09-09

1. Start of developing
2. Creation of LXC container on PVE4
3. Waiting for LAN static IP allocation

## 2024-09-10

1. Rebuild on PVE1 in ID 107
2. development IP allocated at LAN for 10.213.30.20, VLAN ID is 30
3. Installed Docker, PortainerBE
4. Created docker network with "front-tier" for web UI, and "back-tier" for container's communication

