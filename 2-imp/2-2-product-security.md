# 2.2. Product Security

## Content
* 2.2.1. [Security Requirements](#221-security-requirements)
* 2.2.2. [Secure Build Environment](#222-secure-build-environment)
* 2.2.3. [Secure Design](#223-secure-design)
* 2.2.4. [Secure Implementation](#224-secure-implementation)
* 2.2.5. [Secure Testing](#225-secure-testing)
* 2.2.6. [Secure Release and Deployment](#226-secure-release-and-deployment)

## 2.2.1. Security Requirements
**Objectives**:
* Define a set of security requirements for each product. 
  * You can start with a subset of generic security requirements from OWASP [[1](../references.md#24-owasp-asvs),[2](../references.md#25-owasp-masvs)]. 
  * Create your custom set requirements derived from your security policies & guidelines.
* Define a process to verify the requirements are validated manually or automatically before the public release and periodically thereafter.

**Rational**: The security requirements can be used to implement the approporiate security measure against known attack scenarios.

**Hint/Caveat**: Some security requirements can be tested and validated using automated checks (same as QA testing), make sure your take advantage of that.

## 2.2.2. Secure Build Environment

**Objectives**:
* Define the appropriate security measures to protect access to the build toolchain and environment.
* Access and contribution to source code shall be formally defined.
* Make sure all secrets are fetched from secure location and protected against excessive exposure.
* Backup your source code periodically. 

**Rational**: Prevent the introduction of malicious code or loss of the code partially or entirely, accidentally or by rogue employee. 

## 2.2.3. Secure Design

**Objectives**:
* Create threat models and update them regurargly or after every major or security-relevant change [[3](../references.md#26-threat-modeling-manifesto)].
* Promote the use of reusable reference architecture that are secure by design, based on best practices from your cloud provider [[4](../references.md#27-aws-wat-security),[5](../references.md#28-microsoft-waf-security),[6](../references.md#29-google-caf-security)].

## 2.2.4. Secure Implementation
**Objectives**:
* Create a code review checklist, and include the relevant security checks. 
* Use a secret scanner, code quality, and Static Application Security Testing (SAST) tools to scan your code for potentially vulnerable code patterns.

**Hint/Caveat**: Many security scanning tools might wrongly raise false alerts, and reviewing all findings might be time consuming, particurarly with products with large code base. Make sure you don't train your developers to ignore all findings alltogether.  

## 2.2.5. Secure Testing
**Objectives**:
* Elaborate a security testing strategy depending on the risk and available budget.
* Create sceanrio-based test plans based on the predefined threat model, or threats scenarios applicable to similar products.
* Perform generic testing (such as fuzzing) to address residual risk from scenarios that are not addressed in existing test plans. 

**Hint/Caveat**: In case of products running on external (untrusted) environment (such as mobile app running on end-user's device) make sure you address test scenarios related to reverse engineering, physical attack, fault injection and side channel attack.

## 2.2.6. Secure Release and Deployment

**Objectives**:
* Define a formal release process with a checklist of relevant preconditions prior to promoting the application to public use.
* Sign the deliverable code using the organization's cryptographic key and make sure it is verified before processing any senstive data.
* Ensure secure operation of customer identity and access management (CIAM) [[7](../references.md#30-ciam)]
* Set up the approporiate security logging and monitoring. 
