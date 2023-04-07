## 3.1 Offensive Security

### Content
* [3.1.1 Infrastructure & Application Testing](#311-infrastructure--application-testing)
* [3.1.2 Responsible Disclosure & Bug Bounty Programs](#312-responsible-disclosure--bug-bounty-programs)
* [3.1.3 Security Chaos Engineering](#313-security-chaos-engineering)

### 3.1.1 Infrastructure & Application Testing
* Define a standardized test plan template, where you specify the scope and test scenario(s), as well as potential assumptions. 
  * The scope shall clearly define the testing perimeter (example: specific domain name, dedicated test vs production environment)
  * The test scenario can be mapped to potential threats from threat modeling, or generic scenario (examples: OWASP Top 10, MITRE CWE, etc).
  * Assumptions might include information that a tester should take into account to skip specific attack paths. This can be an actual risk that your organization is willing to accept (example: distributed denial of service attack or reverse engineering are out of scope)
* Identify the skills required for for the target system. The skills needed to perform testing on web or mobile application usually differ from skills needed to test a corporate network. 
* Run time boxed tests: given enough time, almost any system can be broken. In order to make test results comparable (to some extent), it is important to agree upfront on the test duration.

For more details about security testing methodolgies, refer to [[1](#1-ptes),[2](#2-what-is-pentest),[3](#3-pt-mm)].

### 3.1.2 Responsible Disclosure & Bug Bounty Programs
* Define a responsible disclosure policy [[4](#4-rd-policy)]. This should include a dedicated contact for reporting security vulnerabilities.
* Create and host security.txt file according to RFC9116 [[5](#5-securitytxt)].
* You can leverage a third party provider to help with triage of security report, you can also offer bounties [[7](#7-obb)] to attract skilled testers.

### 3.1.3 Security Chaos Engineering
* See security related item in the following repo [[6](#6-gh-ace)].


## References
#### 1. [PTES](http://www.pentest-standard.org/index.php/PTES_Technical_Guidelines)
#### 2. [What is pentest](https://www.synopsys.com/glossary/what-is-penetration-testing.html)
#### 3. [PT MM](https://github.com/5bhuv4n35h/pentestmindmap)
#### 4. [RD Policy](https://responsibledisclosure.nl/en/)
#### 5. [Security.txt](https://securitytxt.org)
#### 6. [GH ACE](https://github.com/dastergon/awesome-chaos-engineering)
#### 7. [OBB](https://www.openbugbounty.org/)
