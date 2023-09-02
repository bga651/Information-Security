# h1 - Summarize

# h2 Security Misconfiguration

The article highlights the critical issue of security misconfiguration, which has become increasingly prevalent in software applications. In the latest edition, it moved up to the 5th position among the top security concerns. The analysis found that 90% of applications were tested for misconfigurations, with an average incidence rate of 4.%, resulting in over 208,000 instances of Common Weakness Enumeration (CWE) in this category. Notable CWEs in this context are CWE-16 Configuration and CWE-611 Improper Restriction of XML External Entity Reference.

Security misconfiguration arises when various aspects of an application's configuration are not set securely, leaving vulnerabilities that attackers can exploit. These vulnerabilities can manifest in several ways:

1. Lack of security hardening across the application stack or improper cloud service permissions.
2. Enabling unnecessary features or components.
3. Failure to disable default accounts and passwords.
4. Revealing overly informative error messages.
5. Disabling or not configuring the latest security features in upgraded systems.
6. Insecure settings in application servers, frameworks, libraries, databases, and more.
7. Missing or insecure security headers and directives.
8. Use of outdated or vulnerable software components.

To prevent security misconfigurations, organizations should implement secure installation processes:
1. Implement a repeatable hardening process that automates the deployment of secure environments across development, QA, and production.
2. Deploy a minima platform, avoiding unused features and frameworks.
3. Regularly review and update configurations for security patches and updates.
4. Implement a segmented application architecture for effective separation and security.
4. Send security directives to clients through security headers.
5. Automate configuration and setting verification in all environments.
The article also provides several example attack scenarios to illustrate the dangers of security misconfigurations. These include unauthorized access through default accounts, directory listing vulnerabilities, exposure of sensitive information due to detailed error messages, and cloud storage data leaks caused by default sharing permissions.

In conclusion, security misconfiguration poses a significant risk to modern software applications. To mitigate these risks, organizations must prioritize secure configuration practices, automate processes, and maintain up-to-date security measures to protect against potential attacks.

## Reference https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

# h2 Vulnerable and Outdated Componentsicon

The article discusses the critical issue of vulnerable and outdated software components, which ranked as the second most concerning threat in community surveys and data analysis. Unlike other categories, this one lacks Common Vulnerability and Exposures (CVEs) mapped to the included Common Weakness Enumerations (CWEs), necessitating a default exploits/impact weight of 5.0.

Key points regarding vulnerable components include:

1. Lack of Version Awareness: Organizations are vulnerable if they don't know the versions of all their components, including nested dependencies.
2. Outdated Software: Vulnerabilities often arise from using unsupported or out-of-date software, covering operating systems, servers, databases, applications, APIs, and more.
3. Inadequate Vulnerability Scanning: Failing to regularly scan for vulnerabilities and subscribe to security bulletins can leave systems exposed.
4. Delayed Patching: Organizations that don't promptly fix or upgrade their underlying platforms, frameworks, and dependencies are at risk. In many cases, patching occurs on a monthly or quarterly basis, creating unnecessary exposure.
5. Compatibility Testing: Failing to test the compatibility of updated or patched libraries can lead to unexpected issues.

To prevent such vulnerabilities, organizations should:

1. Implement Patch Management: This process should include removing unused dependencies and continuously monitoring component versions using tools like OWASP Dependency Check and monitoring vulnerability databases like CVE and NVD.
2. Source Security: Only obtain components from official sources through secure links to minimize the risk of including malicious components.
3. Monitor Maintenance: Keep an eye on libraries and components that are unmaintained or lack security patches for older versions, and consider deploying virtual patches if necessary.
4. Continuous Vigilance: Maintain an ongoing plan for monitoring, triaging, and applying updates or configuration changes for the entire application or portfolio.

The article illustrates the significance of vulnerable components with attack scenarios, such as the Struts 2 remote code execution vulnerability, emphasizing the far-reaching impact of component flaws. Additionally, it warns of automated tools used by attackers to identify unpatched systems, underlining the importance of proactive patch management.

## Reference https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

# h2 Injection

The article discusses the critical security issue of injection attacks, which have moved to the third position in the top security concerns. It reveals that 94% of applications were tested for various forms of injection vulnerabilities, with a notable incidence rate. The most significant Common Weakness Enumerations (CWEs) associated with injection attacks include CWE-79 (Cross-site Scripting), CWE-89 (SQL Injection), and CWE-73 (External Control of File Name or Path).

Key points regarding injection vulnerabilities are as follows:

1. Vulnerability Causes: Applications are susceptible to injection attacks when they fail to validate, filter, or sanitize user-supplied data. Dynamic queries without proper escaping, object-relational mapping (ORM) misuse, and direct hostile data usage in dynamic queries, commands, or stored procedures can all lead to vulnerabilities.
2. Types of Injections: Injection attacks come in various forms, including SQL, NoSQL, OS command, ORM, LDAP, and Expression Language (EL) or Object Graph Navigation Library (OGNL) injection. The underlying concept is consistent across all interpreters.
3. Prevention Measures: Preventing injection attacks involves keeping data separate from commands and queries. Recommended prevention methods include using safe APIs, parameterized interfaces, or ORM tools. Positive server-side input validation and escaping special characters for dynamic queries are also essential. SQL controls like LIMIT can be used to limit mass data disclosure during SQL injection.

The article emphasizes the importance of source code review and automated testing for identifying injection vulnerabilities. It also suggests incorporating static (SAST), dynamic (DAST), and interactive (IAST) application security testing tools into the CI/CD pipeline to catch injection flaws before they reach production.

To illustrate the severity of injection attacks, the article presents attack scenarios. In these scenarios, attackers manipulate input data to exploit vulnerabilities in SQL queries, potentially gaining unauthorized access, modifying data, or invoking malicious procedures. These examples highlight the real-world risks associated with injection vulnerabilities and the critical need for effective prevention measures.

## Reference https://owasp.org/Top10/A03_2021-Injection/

