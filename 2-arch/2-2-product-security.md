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
  * You can start with a subset of generic security requirements from OWASP [[1](#1-owasp-asvs),[2](#2-owasp-masvs)]. 
  * Create your custom set requirements derived from your security policies & guidelines.
* Define a process to verify the requirements are validated manually or automatically before the public release and periodically thereafter.

**Rational**: The security requirements can be used to implement the approporiate security measure against known attack scenarios.

**Caveat**: 

## 2.2.2. Secure Build Environment

**Objectives**:
* Define the appropriate security measures to protect access to the build toolchain and environment.
* Access and contribution to source code shall be formally defined.
* Make sure all secrets are fetched from secure location and protected against excessive exposure.
* Backup your source code periodically. 

**Rational**: Prevent the introduction of malicious code or loss of the code partially or entirely, accidentally or by rogue employee. 

## 2.2.3. Secure Design

**Objectives**:
* Perform threat modeling [[3](#3-threat-modeling-manifesto)].

## 2.2.4. Secure Implementation
**Objectives**:
* Create a code review checklist, and include the relevant security checks. 
* Use a secret scanner, code quality, and Static Application Security Testing (SAST) tools to scan your code for potentially vulnerable code patterns.

**Hint/Caveat**: Many security scanning tools might wrongly raise false alerts, and reviewing all findings might be time consuming, particurarly with products with large code base. Make sure you don't train your developers to ignore all findings alltogether.  

## 2.2.5. Secure Testing

TBD

## 2.2.6. Secure Release and Deployment

TBD

## Reference
#### 1. [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)
#### 2. [OWASP MASVS](https://mas.owasp.org/MASVS/)
#### 3. [Threat Modeling Manifesto](https://www.threatmodelingmanifesto.org/)
