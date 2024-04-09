# 2. Cyber Risk Implementation

Traditionally, security engineering usually refer to keeping malicious actors away from your organization's infrastructure. This usually refers to corporate security. Another aspect of cybersecurity emerges from the need to design, implement and release secure product, with an additional focus on the security from the end-user's perspective. Depending on your organization and the type of products delivered, the these domains might partially overlap [[1](../references.md#21-corp-vs-prod-security-sans)].

## [2.1 Corporate security](2-1-corporate-security.md)
Regardless of whether your infrastrcture is hosted on the cloud or on premises, there are some generic security considerations. When your infrastrure is hosted on the cloud, the shared responsability model specifies the scope of each party. 

The following activities are part of the responsability of corporate security: 
* 2.1.1 Network & Infrastructure Security
* 2.1.2 Enterprise Identity and Access Management
* 2.1.3 Data Loss Prevention (DLP)
* 2.1.4 Building a Security Operation Center (SOC)

## [2.2 Product security](2-2-product-security.md)
A product might be running entirely in your own environment (API/Online service), in an external environment (Offline mobile app) or a combination of both (Web application/Connected mobile app). In all cases, you need to adopt a secure software development lifecycle specific to your product portfolio. The main difference lies in the operation step. 

The following activities are part of product security: 
* 2.2.1 Security Requirements
* 2.2.2 Secure Build Environment
* 2.2.3 Secure Design & Reusable Reference Architcture
* 2.2.4 Secure Implementation 
* 2.2.5 Secure Testing 
* 2.2.6 Secure Release and Deployment
