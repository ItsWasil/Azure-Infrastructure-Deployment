# Azure Infrastructure Implementation

## 1. Environment

Cloud Platform: Microsoft Azure  
Resource Group: RG-CloudTech-Lab  
Region: Central India

## 2. Load Balancer

Created a Standard SKU Azure Load Balancer named LB-Web.

Configuration:
- Resource Group: RG-CloudTech-Lab
- Region: Central India
- SKU: Standard
- Tier: Regional

## 3. Backend Pool

Created a backend pool named Backendpool-Web.

Purpose:
- Group backend resources.
- Associate backend resources with load-balancing rules.
- Provide a backend target for incoming traffic.

## 4. Health Probe

Created an HTTP health probe named health1.

Configuration:
- Protocol: HTTP
- Port: 80
- Path: /
- Interval: 5 seconds

Purpose:

The health probe checks backend endpoint availability and helps the load balancer identify unhealthy instances.

## 5. Load Balancing Rule

Configured a load-balancing rule named Rule-HTTP.

Configuration:
- Protocol: TCP
- Port: 80
- Backend Pool: Backendpool-Web
- Health Probe: health1

Purpose:

The rule defines how incoming frontend traffic is forwarded to the configured backend pool.

## 6. Implementation Evidence

Configuration evidence is available in the screenshots folder.

## 7. Summary

This implementation provided practical exposure to Azure Load Balancer administration and cloud networking configuration.
