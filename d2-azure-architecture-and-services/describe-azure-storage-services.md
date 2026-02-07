# Describe Azure storage services

## Blob Storage
- Storage optimized for storing massive amounts of unstructured data;  
 
## Disk Storage
- Azure managed disks are block-level storage columns that are managed by Azure and used with Azure VMs  

## Table Storage
- A service that stores structured NoSQL data in Azure, including a schemaless key/attribute store;  

## Queue Storage
- A service for storing large numbers of messages, accessible from anywhere via authenticated HTTP or HTTPS calls;  

## File Storage
- Fully managed file shares in Azure accessible via SMB or NFS  

## Storage Tiers
- Azure storage hot, cool, cold, and archive access tiers to store blob object data in a cost-effective manner;  
- Use lifecycle management policies to automate tiers;  
- Storage Cost from Least to Most: Archive -> Cold -> Cool -> Hot;  
- Access Cost from Least to Most: Hot -> Cool -> Cold -> Archive;  
**Archive**  
- An offline tier optimized for storing data that is rarely accessed, and that has flexible latency requirements, on the order of hours;  
- Stored a minimum of 180 days  
**Cold**  
- An online tier optimized for storing data that is rarely accessed or modified, but still requires fast retrieval;  
- Stored a minimum of 90 days  
**Cool**  
- An online tier for storing data that is infrequently accessed or modified;  
- Stored a minimum of 30 days  
**Hot**  
- An online tier optimized for storing data that is accessed or modified frequently;  


## Locally Redundant Storage (LRS)
- Copies your data synchronously three times within a single physical location in the primary region;  

## Zone Redundant Storage (ZRS)
- Copies your data synchronously across three Azure availability zones in the primary region;  
- With LRS and ZRS, redundancy is limited to the primary region only!  

## Geo-Redundant Storage (GRS)
- Copies your data synchronously three times within a single physical location in the primary region using LRS;  
- It then copies it asynchronously to a single physical location in the secondary region (3 copies using LRS)  

## Geo-Zone Redundant Storage (GZRS)
- Copies your data synchronously three times within the primary region using ZRS;  
- It then copies it asynchronously to a single physical location in the secondary region;  
- Recommended by MSET for apps requiring high availability;  
- With GRS and GZRS, redundancy is extended to the secondary region!  


## AzCopy
- A command-line utility that you can use to copy blobs or files to or from your storage account;  

## Azure Storage Explorer
- A standalone app that provides a graphical interface to manage files and blobs in your Azure Storage Account;  
- Supports file and blob upload, download, or move between accounts  

## Azure File Sync
- A tool that lets you centralize your file shares in Azure Files and keep the flexibility, performance, and compatibility of a Windows file server;  
- Once installed on a local Windows server, it will automatically stay bi-directionally synced with your files in Azure  


## Azure Migrate
- A service that provides a simplified migration, modernization, and optimization for Azure;  
- Includes all pre-migration steps such as discovery, assessments, and right-sizing;  
- It is a hub of services and tools designed to detect, analyze and facilitate the migration of any type of workload to Azure  

## Azure Data Box
- A cloud solution that lets you send terabytes of data into and out of Azure in a quick, inexpensive, and reliable fashion;  
- Customers are shipped a proprietary Data Box storage device;  
- Ideally suited to transfer data sizes larger than 40 TBs in scenarios with limited or no network connectivity  
