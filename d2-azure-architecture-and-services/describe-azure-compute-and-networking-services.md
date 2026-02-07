# Describe Azure compute and networking services

## Azure VMs
- Server virtualization (compute) on-demand without need for hardware purchase  
## VM scale sets: 
- allow you to create and manage a group of identical, load-balanced VMs;  
- The number of VM instances can automatically increase or decrease in response to demand or based on a schedule;  
- Focus = scale (scalability, capacity)  
## VM availability sets:
- Help build a more resilient, highly available environment by staggering VM updates and ensuring varied power and network connection;  
- Focus = resiliency (availability);  
- They do this through two mechanisms: fault domain and update domains  
- Update domains: allows you to apply updates while knowing that only one update domain grouping will be offline at a time  
- Fault domains: groups your VMs by common power and network switch; By default, an availability set will split your VMs across up to three fault domains  

## Azure Kubernetes Services (AKS)
- A hosted Kubernetes service, where Azure handles critical tasks like health monitoring and maintenance for you;  
- You pay only for the agent nodes within your clusters, not for the masters (free tier);  
- For a financially backed SLA, you pay a few cents per hour for cluster management  

## Azure Container Instance (ACI)
- Runs Docker containers on-demand in a managed, serverless Azure environment;  
- A solution for any scenario that can operate in isolated containers, without orchestration  

## Azure App Service
- An HTTP-based service for hosting web applications, REST APIs, and mobile back ends;  
- Types of app service styles include: Web apps, API apps, Web jobs, Mobile apps  

## Azure Virtual Desktop
- A desktop and app virtualization service that runs in Microsoft Azure;  
- Enable IT Pros and MSPs to create Windows 10 & 11 virtual desktops in Azure;  
- If a question mentions ‘Virtual Desktop Infrastructure (VDI)’, Azure Virtual Desktop is likely the answer  

## VM Resource Requirements
- Virtual Disk  
- Virtual Network (VNET)  
- Network Interface (Virtual NIC)  
- Network Security Group  
- Public IP Address  

## Virtual Network (VNET)
- A logical representation of your network in Azure;  
- A VNET contains one or more subnets;  
- VNETs provide logical isolation in Azure dedicated to your subscription;  
- VMs in different VNETs cannot communicate by default  

## Virtual Subnet
- Segment address space of VNET to create sub-networks;  
- Allows Azure resource deployment into a specific subnet;  
- Can affect outbound access and routing traffic between resources;  
- VMs in different subnets within a VNET can communicate by default  

## VPN Gateway
- A virtual network gateway that sends encrypted traffic between an Azure VNET and an on-premises location over the Internet;  
- Site-to-site VPN traffic traverses the internet;  
- Core component of the cloud  

## VNET Peering
- Enables seamless connection of two or more VNETs in Azure;  
- The two networks function as one in terms of connectivity  

## ExpressRoute
- Extends your on-premises networks into Azure over a private connection with the help of a connectivity provider;  
- Traffic does not traverse the internet  

## Azure DNS
- A hosting service for DNS domains that provides name resolution by using Microsoft Azure infrastructure;  
- Can provide internal and external DNS  

## Service Endpoint
- Provides a way to lock down access to all instances of a PaaS service to a VNET;  
- Accessible from public internet  

## Private Endpoint
- Grants access to a specific instance (resource) of a PaaS service in your VNET on a private IP address;  
- Enables access from on-premises without public endpoint  

## Defense in-Depth
- A layered approach that does not rely on one method to completely protect your environment  

## Network Security Group
- Contains security rules that allow or deny inbound network traffic to, or outbound network traffic from, several types of Azure resources;  
- For each rule, you can specify source, destination port and protocol;  

## Azure Firewall
- A managed, cloud-based network security service that protects your Azure Virtual Network resources;  
- It’s a fully stateful firewall as a service with built-in high availability and unrestricted cloud scalability  

## Azure DDoS
- Standard tier provides enhanced DDoS mitigation features to defend against DDoS attacks;  
- Also includes logging, alerting, and telemetry not included in the free Basic tier present by default  
