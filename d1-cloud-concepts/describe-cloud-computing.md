# Describe Cloud Computing

**NIST definition of cloud computing** : model for enabling universal, convenient, on-demand network access … to a shared pool of configurable computing resources (e.g. networks, servers, storage, apps, and services) … that can be rapidly provisioned and released with minimal management effort or service provider interaction.

## Shared responsibility model
Question: Is there better security in the cloud?  
- Yes; cloud technology enables security to  
- Shift commodity responsibilities to provider and re-allocate your resources  
- Leverage cloud-based security capabilities for more effectiveness  
- Use cloud intelligence to improve detection/response time  

## Public Cloud
- Everything runs on the cloud provider’s hardware.  
- Advantages: scalability, ability PAYG, no maintenance and low skills  
## Private Cloud
- A cloud environment in your own datacenter.  
- Advantages: legacy support, control, and compliance  
## Hybrid Cloud
- Combines public and private clouds, allowing you to run your apps in the right location.  
- Advantages: flexibility in legacy, compliance, and scalability scenarios  

## Economies of Scales
- The ability to do things more efficiently or at a lower-cost per unit when operating at a larger scale.  
## Capital Expenditure (CapEx)
- Spending money on physical infrastructure up front.  
- Associated with legacy on-premises datacenter scenarios  
## Operational Expenditure (OpEx)
- Spending money on services or products now and being billed as you go.  
- Associated with public cloud consumption  
- The cloud increases OpEx spending and decreases CapEx spending  

## Consumption-based model
- Pay for what you use, typically per unit of time or capacity (per-minute, per-GB, per-execution)  
## Fixed-price model  
- You provision resources and pay for those instances whether you use them or not  
- Ensures predictable costs for your cloud services  

## Serverless Architecture
- A cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.  
- PAYG model based on use.  
- Resources are stateless, servers ephemeral and often capable of being triggered.  
- Example: Function-as-service  

## Question: How is serverless different from PAAS in terms of responsibility? 
**Both:** 
Devs have to write code, no server management  
**PaaS:** 
More control over deployment environment, application has to be configured to auto-scale, application takes a while to spin up  
**Serverless:** 
Less control over deployment environment, application scales automatically, application code only executes when invoked  

## Three Common Serverless Azure Services:
**1) Logic App** (most common): 
Cloud service that helps you schedule, automate and orchestrate tasks, business processes, and workflows; 
You can choose from a gallery of hundreds of pre-built connectors  
**2) Functions:** 
Event driven, compute-on-demand experience that extends the existing Azure application platform with capabilities to implement code triggered by events in Azure as well as on-premises systems; 
This enables billing per execution rather than by time  
**3) Event Grid:**
Enables you to easily manage events across many different Azure services and applications; 
Once a subscription is created, Event Grid will push events to the configured destination;
Makes it easy for any developer to utilize the “push” model instead of the inefficient “pull” across their Serverless architecture;
Pay per use like Azure Functions

