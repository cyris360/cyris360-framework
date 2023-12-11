# 2.2. Product Security

## Content
* 2.2.1. [Cloud Security Posture Management](#221-cloud-security-posture-management)
* 2.2.2. [Secure Software Lifecycle](#222-secure-software-lifecycle)
* 2.2.3. [Secure Release and Deployment](#223-secure-release-and-deployment)

## 2.2.1 Cloud Security Posture Management
**Objectives**:
* Manage the security posture of the infrastructure hosting the product or service [[7](../references.md#27-cspm)].
  
## 2.2.2. Secure Software Lifecycle
**Objectives**:
* Define a set of security requirements for each product. 
  * You can start with a subset of generic security requirements from OWASP [[8](../references.md#28-owasp-asvs),[9](../references.md#29-owasp-masvs)]. 
  * Create your custom set requirements derived from your security policies & guidelines.
* Define a process to verify the requirements are validated manually or automatically before the public release and periodically thereafter.
* Define the appropriate security measures to protect access to the build toolchain and environment.
* Access and contribution to source code shall be formally defined.
* Make sure all secrets are fetched from secure location and protected against excessive exposure.
* Create threat models and update them regurargly or after every major or security-relevant change [[10](../references.md#210-threat-modeling-manifesto),[11](../references.md#211-stride-lm),[12](../references.md#212-stride-gpt)].
* Promote the use of reusable reference architecture that are secure by design, based on best practices from your cloud provider [[13](../references.md#213-aws-wat-security),[14](../references.md#214-microsoft-waf-security),[15](../references.md#215-google-caf-security)].
* Use a secret scanner, code quality, and Static Application Security Testing (SAST) tools to scan your code for potentially vulnerable code patterns.
* Ensure your source code is saved in alternate location periodically, with equivalent controls.
* Elaborate a security testing strategy depending on the risk and available budget.
* Create sceanrio-based test plans based on the predefined threat model, or threats scenarios applicable to similar products.
* Perform generic testing (such as fuzzing) to address residual risk from scenarios that are not addressed in existing test plans. 

**Hint/Caveat**: In case of products running on external (untrusted) environment (such as mobile app running on end-user's device) make sure you address test scenarios related to reverse engineering, physical attack, fault injection and side channel attack.

## 2.2.3. Secure Release and Deployment

**Objectives**:
* Define a formal release process with a checklist of relevant preconditions prior to promoting the application to production environment.
* Sign the deliverable code and make sure any code running on external environment is verified (for integrity & authenticity) before processing any senstive data.
* Ensure secure operation of customer identity and access management (CIAM) [[16](../references.md#216-ciam)]
* Set up the approporiate security logging and monitoring.
* Define the appropriate protection layers for APIs, including use of CDN with Web Application and API Protection (WAAP). 
