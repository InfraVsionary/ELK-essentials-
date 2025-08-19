# ELK Stack 

> 🚀 A clean, ready-to-run ELK (Elasticsearch, Logstash, Kibana) setup with Docker Compose.

## ✨ Features
- 📂 **stack/** → Configs (Elasticsearch, Logstash, Filebeat)  
- 🛠 **scripts/** → Maintenance helpers 
- 📖 **docs/** → Ops notes  
- 🐳 **docker-compose.yml** → Modular services  

## ⚡ Quick Start
```bash
git clone https://github.com/InfraVsionary/ELK-essentials.git
cd ELK-essentials
docker compose up -d
```


# ELK Stack

A clean, ready-to-run ELK (Elasticsearch, Logstash, Kibana) setup with Docker Compose.  
Lightweight and tuned to run smoothly even on small EC2 instances (2 GB RAM / 2 vCPU).

## Features
- `stack/` → Configurations for Elasticsearch, Logstash, and Filebeat  
- `scripts/` → Host bootstrap and maintenance helpers  
- `docs/` → Notes and references for operations  
- `docker-compose.yml` → Modular, production-inspired service definitions  

## One-time Host Setup

Before running the stack on a fresh EC2 instance, prepare the host:

```bash
git clone https://github.com/InfraVsionary/ELK-essentials.git
cd ELK-essentials
make host-bootstrap
make up

## Access

Kibana → http://<EC2_PUBLIC_IP>:5601
Elasticsearch API → http://<EC2_PUBLIC_IP>:9200 (for development use only)
