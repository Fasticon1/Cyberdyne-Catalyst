# Cyberdyne-Catalyst

![Cyberdyne Catalyst](https://raw.githubusercontent.com/Fasticon1/Cyberdyne-Catalyst/refs/heads/main/CyberdyneCatalyst.webp)

## About This Project

**Cyberdyne-Catalyst** is a Docker Compose-based homelab setup designed for learning and experimenting with AI, data management, security, and resource monitoring. This repository contains the configurations for various services, organized into logical stacks.

**Please Note:** This project is currently a work in progress. Configurations and services may change.

---
## Services & Stacks

This repository is structured into the following service stacks:

### AI Stack
This stack focuses on providing tools and platforms for AI development and experimentation.
* **OpenWebUI**: A user-friendly web interface for various AI models.
* **Flowise**: A low-code tool for building LLM-based applications.
* **UnstructuredAPI**: An API for parsing and extracting information from unstructured data.
* **JupyterLab**: An interactive development environment for notebooks, code, and data.
* **n8n**: An extendable workflow automation tool.

You can find the Docker Compose configuration for these services in `Services/ai-stack/docker-compose.yml`.

---
### Monitoring Stack
This stack is dedicated to monitoring metrics, logs, and overall homelab resources.
* **Grafana**: For visualizing metrics and logs.
* **Prometheus**: For metrics collection and alerting.
* **Loki**: For log aggregation.
* **Promtail**: For shipping logs to Loki.
* **cAdvisor**: For monitoring container resource usage and performance.
* **OpenSearch**: A distributed search and analytics engine.
* **Pyroscope**: For continuous profiling to understand application performance.

Configurations:
* `Services/Monitoring-stack/docker-compose.yml`
* `Services/Monitoring-stack/loki-config.yml`
* `Services/Monitoring-stack/prometheus.yml`
* `Services/Monitoring-stack/promtail-config.yml`

---
### Database Stack
This stack includes various database solutions for data storage and management.
* **Redis**: An in-memory data structure store, used as a database, cache, and message broker.
* **PostgreSQL**: A powerful, open-source object-relational database system.
* **Milvus**: A vector database built for AI applications.

You can find the Docker Compose configuration for these services in `Services/database-stack/docker-compose.yml`.

---
## Goals
The primary goal of this repository is to facilitate learning in the following areas:
* Artificial Intelligence model deployment and usage.
* Data management strategies and database technologies.
* Homelab security practices.
* Monitoring of telemetry, metrics, and system resources.
* Mastering Docker Compose for local service deployment, in preparation for learning and utilizing Ansible for broader infrastructure automation.

---
## Future Development
* Further refinement of existing service configurations.
* Addition of more services related to AI, data engineering, and security.
* Detailed documentation for each service setup and usage.( To refine technical writing skills)

---