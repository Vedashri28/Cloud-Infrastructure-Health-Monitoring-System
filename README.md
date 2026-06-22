# Cloud-Infrastructure-Health-Monitoring-System
Developed a Cloud Infrastructure Health Monitoring System using AWS, Docker, Prometheus, Grafana, and Node Exporter to monitor and visualize real-time server performance metrics.

##  Project Overview

Cloud Infrastructure Health Monitoring System is a real-time infrastructure monitoring solution built using AWS EC2, Docker, Prometheus, Grafana, and Node Exporter.

The platform collects system metrics such as CPU usage, Memory usage, Disk utilization, Network statistics, and Server uptime, and visualizes them through interactive Grafana dashboards for effective infrastructure monitoring.

---

##  Problem Statement

Managing and monitoring servers manually becomes difficult as infrastructure grows.

This project helps DevOps teams:

* Monitor CPU usage
* Monitor Memory utilization
* Monitor Disk space
* Monitor Network activity
* Track system uptime
* Visualize performance trends
* Identify potential issues before downtime

---
##  Architecture Diagram

User
  │
  ▼
Grafana Dashboard (3000)
  │
  ▼
Prometheus (9090)
  │
  ▼
Node Exporter (9100)
  │
  ▼
AWS EC2 Ubuntu Server

##  Architecture

AWS EC2 (Ubuntu)

→ Node Exporter

→ Prometheus

→ Grafana

→ Dashboard Visualization

---

## Technologies Used

* AWS EC2
* Ubuntu Linux
* Docker
* Prometheus
* Grafana
* Node Exporter

---

##  Implementation Steps

### Step 1: Launch AWS EC2 Instance

* Created Ubuntu EC2 instance
* Configured Security Groups
* Connected using SSH

### Step 2: Install Docker

* Installed Docker Engine
* Started Docker Service
* Verified Docker Installation

### Step 3: Deploy Node Exporter

* Pulled Node Exporter Docker Image
* Exposed Port 9100
* Verified metrics endpoint

### Step 4: Configure Prometheus

* Created prometheus.yml
* Configured scrape targets
* Deployed Prometheus Container
* Exposed Port 9090

### Step 5: Deploy Grafana

* Deployed Grafana Container
* Exposed Port 3000
* Configured Admin Login

### Step 6: Connect Grafana to Prometheus

* Added Prometheus as Data Source
* Verified successful connection

### Step 7: Create Monitoring Dashboard

* Imported Node Exporter Full Dashboard (ID: 1860)
* Visualized CPU, Memory, Disk, Network, and Uptime metrics

---

##  Features

* Real-Time Monitoring
* CPU Usage Tracking
* Memory Usage Monitoring
* Disk Utilization Monitoring
* Network Statistics
* Uptime Monitoring
* Interactive Dashboards
* Historical Metrics Visualization

---

## 💡 Skills Demonstrated

- Linux
- AWS EC2
- Docker
- Prometheus
- Grafana
- Monitoring & Observability
- Networking
- DevOps

## Project Screenshots
### SSH Connection to AWS EC2
![SSH Connection](screenshots/ssh-connection.png)

### Running Docker Containers
![Docker Containers](screenshots/docker-containers.png)

### Prometheus Dashboard
![Prometheus Dashboard](screenshots/prometheus-dashboard.png)

### Grafana Login
![Grafana Login](screenshots/grafana-login.png)

### Grafana Home
![Grafana Home](screenshots/grafana-home.png)

### Prometheus Data Source Connection
![Datasource](screenshots/grafana-prometheus-datasource.png)

### Infrastructure Dashboard
![Dashboard](screenshots/grafana-dashboard-overview.png)

### CPU and Memory Monitoring
![CPU Memory](screenshots/grafana-cpu-memory.png)

### Node Exporter Monitoring Dashboard
![Node Exporter](screenshots/grafana-node-exporter-dashboard.png)

---

##  Access URLs

Prometheus:
http://18.116.231.205:9090

Grafana:
http://18.116.231.205:3000

##  Outcome

Successfully built a centralized monitoring platform capable of collecting, storing, and visualizing server performance metrics in real time.

---

##  Author

Vedashri Giri

B.Tech Student | DevOps & Cloud Enthusiast
