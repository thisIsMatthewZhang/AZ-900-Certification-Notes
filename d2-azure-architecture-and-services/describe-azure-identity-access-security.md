# Describe Azure identity, access, and security

## Entra ID
Entra is Microsoft’s cloud-based identity and access management service which helps your employees sign in and access resources, including:  
- **Internal resources**, such as apps on your corporate network or custom cloud apps  
- **External resources**, such as Microsoft 365, the Azure portal, and many SaaS apps  

## Single Sign-on (SSO)
User doesn't have to sign into every application they use;  
The user logs in once and that credential is used for multiple apps;  
Single sign-on based authentication systems are often called **“modern authentication”**  

## MFA
In Entra ID works by requiring two or more of the following authentication methods:  
- Something you know **know (pin or password)**  
- Something you **have (trusted device)**  
- Something you **are (biometric)**  
What is an OATH token?  
- Open Authentication (OATH) is an open standard that specifies how **time-based, one-time password codes** are generated
- **Software OATH tokens** are typically applications. Entra ID generates the secret key, or seed, that is input into the app and used to generate each OTP
- **Hardware OATH tokens** are small hardware devices that look like a key fob that displays a code that refreshes every 30 or 60 seconds, with secret key/seed pre-programmed
What is FIDO2?
- Uses public-key (asymmetric) cryptography for user authentication
- User has a physical device (USB or NFC)
- **Authentication Sequence:** Provide Username -> Cryptographic challenge -> Use FIDO2 key to sign challenge -> Service verifies response and grants access
What problems does Windows Hello for Business solve?
- **Strong passwords can be difficult to remember** and users often reuse passwords on multiple sites
- **Server breaches** can expose symmetric network credentials (passwords)
- Passwords are subject to replay attacks
- Users can inadvertently expose their passwords due to **phishing attacks**
***Passwordless is considered the best authentication method** (Windows Hello, Microsoft Authenticator App, FIDO2 Security Key)*

## Conditional Access
Used by Entra ID to bring signals together, to make decisions, and enforce organizational policies


## B2B Collaboration
Enable external users to use their preferred identity to sign into your Microsoft or other enterprise applications (SaaS apps, custom-developed apps, etc.);
Supports Entra ID and social identities

## B2B direct connect
Establish a mutual, two-way trust with another Entra ID organization for seamless collaboration;
Useful for heavy, daily collaboration with close business partners;
Supports multiple two-way trusts

## Business-to-Consumer (B2C)
Publish modern SaaS apps or custom-developed apps to consumers and customers, while using Entra ID B2C for identity and access management;
Supports Entra & social identities

## Entra ID multi-tenant organization
Collaborate with multiple tenants in a single Entra ID organization via cross-tenant synchronization;
Good for conglomerates, mergers, multi-cloud, dept/test/staging tenants

## Azure RBAC (Role Based Access Control)
Azure RBAC helps you manage:
- Who has access to Azure resources
- What they can do with those resources
- Which resources/areas they have access to
Built on Azure Resource Manager and **provides fine-grained access management** of Azure resources;
One element of implementing ‘least privilege’

## Principles of Zero Trust
**Unlike the “trust but verify” approach, no entity is trusted by default;
Trust must be earned, compliance must be proven;
Layered security: Identities, devices, apps, data, infrastructure, networks**
## Verify explicitly
Always authenticate and authorize **based on all available data points**

## Use least privilege access
**Limit user access** with Just-In-Time and Just-Enough-Access (JIT/JEA), risk-based adaptive policies, and data protection

**Assume breach**
Segment networks to limit data access and minimize blast radius/reduce threat exposure;
Verify **end-to-end encryption** and use analytics to get visibility, drive threat detection, and improve defenses

## Defender for Cloud
A unified infrastructure security management system that strengthens the security posture of your cloud and on-premises data centers;  
Provides security guidance for compute, data, network, storage, app and other services;  
Includes support for both Azure and on-premises workloads, as well as other public clouds (AWS, GCP);  
Multi-cloud support  
