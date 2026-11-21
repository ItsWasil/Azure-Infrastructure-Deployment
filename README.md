# Azure Infrastructure Deployment and Network Security

## Azure Administrator Capstone Project

**Cloud Platform:** Microsoft Azure  
**Project Type:** Cloud Infrastructure Administration  
**Region:** Central India  
**Resource Group:** RG-CloudTech-Lab

---

## 1. Project Overview

This project demonstrates practical exposure to Microsoft Azure infrastructure administration and load-balancing configuration.

The project focuses on configuring an Azure Standard Load Balancer, creating a backend pool, configuring an HTTP health probe, and associating the components through a load-balancing rule.

The objective is to understand how Azure Load Balancer components work together to manage network traffic and monitor backend endpoint health.

## 2. Project Objectives

- Understand Azure Load Balancer configuration.
- Explore backend pool management.
- Configure HTTP health probes.
- Configure TCP load-balancing rules.
- Understand frontend-to-backend traffic mapping.
- Document Azure infrastructure configuration.
- Understand backend health monitoring.

## 3. Technologies Used

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud platform |
| Azure Load Balancer | Network traffic distribution |
| Backend Pools | Backend resource grouping |
| Health Probes | Backend health monitoring |
| Load Balancing Rules | Traffic forwarding |
| HTTP | Health probe protocol |
| TCP | Load balancing protocol |

## 4. Infrastructure Details

### Azure Load Balancer

- Name: LB-Web
- Resource Group: RG-CloudTech-Lab
- Region: Central India
- SKU: Standard
- Tier: Regional

### Backend Pool

- Name: Backendpool-Web
- Purpose: Groups backend resources associated with the load balancer.

### Health Probe

- Name: health1
- Protocol: HTTP
- Port: 80
- Path: /
- Interval: 5 seconds

The health probe checks the configured backend endpoint to help determine whether backend instances are healthy.

### Load Balancing Rule

- Name: Rule-HTTP
- Protocol: TCP
- Port: 80
- Backend Pool: Backendpool-Web
- Health Probe: health1

The rule associates the frontend traffic configuration with the backend pool and health probe.

## 5. Implementation Screenshots

### 5.1 Load Balancer Overview

![Load Balancer Overview](screenshots/01-load-balancer-overview.png)

Shows the Azure Load Balancer resource and its configuration overview.

### 5.2 Health Probe List

![Health Probe List](screenshots/02-health-probe-list.png)

Shows the health probe configured for LB-Web.

### 5.3 Health Probe Configuration

![Health Probe Configuration](screenshots/03-health-probe-configuration.png)

Shows the HTTP health probe settings, including port 80, path `/`, and a five-second interval.

### 5.4 Backend Pool

![Backend Pool](screenshots/04-backend-pool.png)

Shows the Backendpool-Web configuration.

### 5.5 Additional Implementation Evidence

Refer to the remaining screenshots in the screenshots folder for additional project configuration.

## 6. Key Learning Outcomes

- Azure Load Balancer administration.
- Backend pool configuration.
- HTTP health probe configuration.
- TCP networking fundamentals.
- Load-balancing rule configuration.
- Cloud infrastructure documentation.

## 7. Conclusion

This project provided practical exposure to Azure Load Balancer configuration and cloud networking concepts.

It helped strengthen my understanding of backend pools, health probes, load-balancing rules, and Azure infrastructure administration.

---

**Project Category:** Microsoft Azure Administration  
**Project Level:** Beginner / Capstone  
**Documentation:** Maintained using GitHub
