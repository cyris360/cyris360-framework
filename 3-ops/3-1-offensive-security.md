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

For more details about security testing methodolgies, refer to [[1](../references.md/#31-ptes),[2](../references.md/#32-what-is-pentest),[3](../references.md/#33-pt-mm)].

### 3.1.2 Responsible Disclosure & Bug Bounty Programs
* Define a responsible disclosure policy [[4](../references.md/#34-rd-policy)]. This should include a dedicated contact for reporting security vulnerabilities.
* Create and host security.txt file according to RFC9116 [[5](../references.md/#35-securitytxt)].
* You can leverage a third party provider to help with triage of security report, you can also offer bounties [[6](../references.md/#36-obb)] to attract skilled testers.

### 3.1.3 Security Chaos Engineering
* See security related item in the following repo [[7](../references.md/#37-gh-ace)].

