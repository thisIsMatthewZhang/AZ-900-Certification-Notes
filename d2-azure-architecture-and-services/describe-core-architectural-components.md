# Describe core architectural components of Azure

## Azure Geography
A **discrete market**, typically containing two or more regions, that preserves data residency and compliance boundaries
## Azure Regions  
A **set of datacenters** deployed within a latency-defined perimeter and connected through a dedicated regional low-latency network.  
## Azure Sovereign Region
Special regions that you might need for compliance or legal purposes: Government (Fed govt, DoD), China;  
Operated by social trustees  
## Region Pairs
A relationship between 2 Azure Regions within the same geographic region for **disaster recovery purposes**;  
**Chosen by Microsoft (typically 300+ miles apart)**  
## Management Groups
A level of scope above subscriptions;  
Each directory is given a single top-level management group called the “Root”;  
A boundary for management and application of policy;  
Can be used to **aggregate policy and initiative assignments** via Azure Policy;  
Can contain **multiple subscriptions;**  
All new subscriptions will be placed under the **root management group** by default  
## Subscriptions
**Why use multiple subscriptions?**  
- When subscription limits are reached  
- To use different payment methods  
- To isolate resources between departments, projects, etc.  
Unit of management, billing, and scale within Azure;  
Serve as a management boundary for assigning Azure policies, governance, and isolation  
## Resource Groups
A container that holds related resources for an Azure solution;  
Used to group resources that share a **common resource lifecycle;**  
One-to-one relationship with Subscriptions  
## Resources
An entity managed by Azure, like a VM, virtual network, or storage account;  
One-to-one relationship with Resource groups  
## Availability Zones 
**Unique physical locations** within a region with independent power, network, and cooling;  
Comprised of one or more datacenters;  
Tolerant to datacenter failures via **redundancy and isolation**  
## Azure Datacenters
Physical buildings that contain thousands of servers and other hardware to provide cloud computing services;  
Azure datacenters are located all over the world and are organized into regions;  
Designed to be secure, reliable, and efficient, leveraging economies of scale, multi-tenant;  
**Consists of multiple physical buildings, redundant power, ISPs, etc.**  
