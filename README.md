# Azure Load Balancer Configuration and Network Traffic Management

## Microsoft Azure Administrator Capstone Project

**Cloud Platform:** Microsoft Azure  
**Project Category:** Cloud Infrastructure Administration  
**Project Level:** Beginner  
**Region:** Central India  
**Resource Group:** RG-CloudTech-Lab

---

## 1. Project Overview

This project demonstrates hands-on experience with Microsoft Azure infrastructure administration, focusing on Azure Load Balancer configuration and network traffic management.

The project involves configuring a Standard Azure Load Balancer, creating a backend pool, setting up an HTTP health probe, and configuring a load-balancing rule.

The primary objective is to understand how Azure Load Balancer components work together to manage incoming network traffic and monitor backend endpoint health.

## 2. Project Objectives

- Understand Azure Load Balancer architecture and functionality.
- Configure a Standard SKU Azure Load Balancer.
- Create and manage backend pools.
- Configure HTTP health probes.
- Implement TCP load-balancing rules.
- Understand frontend-to-backend traffic mapping.
- Learn backend health monitoring concepts.
- Gain practical exposure to Azure networking administration.

## 3. Technologies and Services Used

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud infrastructure platform |
| Azure Load Balancer | Network traffic distribution |
| Backend Pools | Backend resource grouping |
| Health Probes | Backend health monitoring |
| Load Balancing Rules | Traffic forwarding configuration |
| HTTP | Health probe protocol |
| TCP | Load-balancing rule protocol |

## 4. Azure Infrastructure Configuration

### 4.1 Azure Load Balancer

Configured a Standard SKU Azure Load Balancer named `LB-Web`.

**Configuration:**

- Name: LB-Web
- Resource Group: RG-CloudTech-Lab
- Region: Central India
- SKU: Standard
- Tier: Regional

### 4.2 Backend Pool Configuration

Created a backend pool named `Backendpool-Web`.

**Purpose:**

- Groups backend resources associated with the load balancer.
- Provides backend targets for load-balancing rules.
- Supports network traffic distribution across configured resources.

### 4.3 Health Probe Configuration

Created an HTTP health probe named `health1`.

**Configuration:**

| Setting | Value |
|---|---|
| Name | health1 |
| Protocol | HTTP |
| Port | 80 |
| Path | / |
| Interval | 5 seconds |

**Purpose:**

The health probe checks the configured backend endpoint and helps Azure Load Balancer determine whether backend instances are healthy enough to receive new connections.

### 4.4 Load Balancing Rule Configuration

Configured a load-balancing rule named `Rule-HTTP`.

**Configuration:**

| Setting | Value |
|---|---|
| Rule Name | Rule-HTTP |
| Protocol | TCP |
| Port | 80 |
| Backend Pool | Backendpool-Web |
| Health Probe | health1 |

**Purpose:**

The load-balancing rule defines how incoming frontend traffic is mapped to the configured backend pool.

## 5. Project Implementation

The project involved the following configuration activities:

1. Created and organized Azure infrastructure resources within a resource group.
2. Configured a Standard Azure Load Balancer.
3. Created a backend pool named Backendpool-Web.
4. Configured an HTTP health probe using port 80.
5. Set the health probe path to `/`.
6. Configured a five-second health probe interval.
7. Created a TCP load-balancing rule named Rule-HTTP.
8. Associated the load-balancing rule with the backend pool and health probe.

## 6. Key Learning Outcomes

Through this project, I gained practical exposure to:

- Microsoft Azure infrastructure administration.
- Azure Load Balancer configuration.
- Backend pool management.
- Health probe configuration and monitoring.
- TCP and HTTP networking fundamentals.
- Load-balancing rule configuration.
- Cloud networking concepts.
- Azure resource organization and management.

## 7. Security Considerations

Important security considerations for Azure infrastructure include:

- Restricting unnecessary inbound network traffic.
- Using Network Security Groups where applicable.
- Avoiding unrestricted administrative access.
- Reviewing backend resource exposure.
- Protecting Azure credentials and subscription information.
- Following the principle of least privilege.

## 8. Conclusion

This capstone project provided practical exposure to Microsoft Azure Load Balancer administration and networking concepts.

By configuring backend pools, health probes and load-balancing rules, I developed a better understanding of how Azure manages network traffic and monitors backend endpoint health.

This project strengthened my foundational knowledge of cloud infrastructure administration and helped me apply concepts covered in the Microsoft Azure Administrator (AZ-104) training.

---

**Project:** Azure Load Balancer Configuration and Network Traffic Management  
**Platform:** Microsoft Azure  
**Certification Preparation:** AZ-104 – Azure Administrator Associate  
**Documentation:** GitHub
