# Describe cloud service types
*A walkthrough of the Shared Responsibility Model*

## Cloud Models and Services
1) IaaS  
**Hybrid model**  
**CSP provides** building blocks like networking, storage, and compute  
**CSP manages** staff, HW, and datacenter  
**Azure services:**  
**Use cases:**  
When to use virtual machines?  
  - **During test and development,** VMs provide a quick and easy way to create different OS and application configurations.  
  - Test and dev teams can **easily deploy and then delete the VMs** when they no longer need them.  
  - **When running applications in the cloud**, can provide technical and financial benefits, as when an application might need to handle fluctuations in demand.  
  - **When extending your datacenter to the cloud**, can extend the capabilities of its own on-premises network by creating a virtual network in Azure and adding VMs to that virtual network.  
  - Makes it easier/less expensive to deploy than on-premises  
  - During disaster recovery, enables significant cost savings by using an IaaS-based approach to disaster recovery  
  - Enables push button, automated VM spin up and shutdown in a disaster  

2) PaaS  
- **Customer is responsible** for deployment and management of apps  
- **CSP manages** provisioning, configuration, hardware, and OS  
- **Azure services under PaaS:** Azure SQL Database, API Management, Azure App Service, and many more…  
**Use cases**  
**Development framework**    
- PaaS provides a framework that developers can build upon to develop or customize cloud-based applications  
- PaaS lets developers **create applications using built-in software components**  
- Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do  
- BOTTOM LINE: reduces developer effort and increases solution quality  
**Analytics or business intelligence**    
- Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes  
- Improves forecasting, product design decisions, investment returns, and other business decisions  
- BOTTOM LINE: simplifies data analysis and improves business outcomes  

3) SaaS  
- Customer just **configures features**  
- **CSP is responsible for** management, operation, and service availability  
- Customer has some responsibility in **access management and data recovery**  
- Azure services under SaaS: Office 365 (now Microsoft 365), Service Now, Salesforce, and many more…  
**Uses cases:**  
- Email and messaging  
- Business productivity applications  
- Finance and expense tracking  
- BOTTOM LINE: these are important utility functions **not core to the company’s purpose**  
