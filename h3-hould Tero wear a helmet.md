# Threat Modeling Manifesto
Threat modeling is a process of analyzing a system to identify security and privacy concerns. It involves four key questions: What are we working on? What can go wrong? What are we going to do about it? Did we do a good enough job? This process helps recognize potential issues and informs decisions throughout a system's development.

Anyone concerned about system privacy and security should engage in threat modeling. The Threat Modeling Manifesto provides guidance for developing a methodology tailored to specific needs. It emphasizes values like finding and fixing design issues, collaboration, and continuous improvement, while its principles highlight the importance of early and frequent analysis aligned with development practices and meaningful outcomes for stakeholders.

In summary, threat modeling is a crucial practice for enhancing system security and privacy, applicable to everyone, and the Threat Modeling Manifesto offers valuable guidance based on core values and principles.

### Reference https://www.threatmodelingmanifesto.org/

# World shortest threat modeling courses
The basic information about treat modeling, what is threating modeling. We threat model to anticipate problems when it's inexpensive to deal with.
Assess threats holistically
Often, a threat to one resource may result in an indirect threat to downstream resources. For example, if an attacker compromises an application, a threat to the application may also compromise the data the application accesses.

For this reason, it is important to assess threats holistically rather than in isolation. Assess the potential severity of each threat not only in terms of the primary resources it threatens, but also in terms of the overall damage it could cause to the business.

Likewise, measures need to be taken to mitigate threats at multiple levels. For example, if a threat to application security causes collateral damage to data security, you can take steps in the application and data to help mitigate the threat. You may need to implement two-factor authentication on your application to reduce the risk of a breach, and also implement off-site backups of your data so that if an application breach allows an attacker to access your data, you have a clean copy to deny Ransom extortion.

Think holistically about threats
It might sound reasonable to focus your threat modeling on threats related to recent high-profile attacks, or threats your business has faced in the past. However, the best threat modeling strategies need to cover every threat that could impact the business—regardless of its newsworthiness or whether it has translated into a real-world attack in the past. When identifying threats, check not only cybersecurity blogs for recent breaches, but also threat databases and threat intelligence reports to gain insight into the types of threats your team may not otherwise consider.

![Table_1 original](https://github.com/bga651/Information-Security/assets/114089466/b747b066-2bc8-463d-994a-b445224e82f5)

### Reference https://www.youtube.com/watch?v=0FoesyawfPU&list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf&index=7


# OWASP Threat Modeling Cheat Sheet
The article provides a concise overview of threat modeling, a structured approach for identifying and prioritizing potential threats to a system, along with guidance on creating threat models for both existing and new systems. The key points in the article are as follows:

Accessible to All: Threat modeling is not exclusive to security experts; it's a practice that should involve developers, software and system designers, and architects. It can be implemented at any stage of the software development life cycle.

Early Detection and Cost Savings: Creating threat models early in the development process helps identify potential vulnerabilities and security issues before they become costly problems during later phases.

Key Objectives of Threat Modeling: When producing a threat model, the objectives are to document data flows within a system, identify potential threats, and document security controls or mitigations that can reduce the impact or likelihood of these threats.

Applicability: The principles of threat modeling are applicable not only to software applications but also to designing network infrastructures and server clusters.

The article introduces several important terms related to threat modeling, including:

Threat Agent: Individuals or groups capable of carrying out specific threats.
Impact: The potential damage caused by a threat, which can include physical, financial, and reputational harm.
Likelihood: The probability of a threat being carried out, influenced by factors such as the difficulty of execution and potential rewards for attackers.
Controls: Safeguards or countermeasures implemented to protect information and assets.
Preventions: Controls that completely prevent specific attacks.
Mitigations: Controls that reduce the likelihood or impact of a threat without necessarily preventing it.
Data Flow Diagram: A visual representation of how information flows within a system.
Trust Boundary: A point on the data flow diagram where data changes its level of trust, often occurring when data is passed between processes or subsystems.
The article also emphasizes the importance of understanding these terminologies and introduces the Threat Modeling Manifesto project's key principles, which guide the steps in the threat modeling process.

Serves as a foundational guide to threat modeling, making it accessible to a broader audience beyond security experts. It provides essential terminology and principles to help individuals and teams systematically identify and address security threats in their systems and applications.

Also provides a step-by-step guide to getting started with threat modeling for software applications. It emphasizes the importance of understanding business objectives and compliance requirements before embarking on the threat modeling process. Here's a summary of the key points:

Define Business Objectives: Start by identifying the business objectives of the applications you are assessing and any security and compliance requirements driven by business or government regulations. This ensures that the threat assessment aligns with the broader goals of the organization.

Identify Application Design: Understand the design of the application, including its data flow and trust boundaries. Creating a data flow diagram of the system is essential for the threat modeling process. Even if you are familiar with the design, additional data flows and trust boundaries may emerge during the analysis.

Create Design Documents: Generating design documents is crucial. The article mentions the 4+1 view model as one approach, but it also acknowledges the flexibility to use other design models. These documents help capture the architecture and structure of the application.

Decompose and Model the System: Develop a high-level information flow diagram that highlights trusted boundaries, actors, information flows, and assets within the system. Understanding how the system operates is vital for effective threat modeling.

Define and Evaluate Assets: Define and evaluate assets based on their confidentiality, integrity, and availability. Consider data in transit and data at rest, as protecting data in both states is essential.

Create an Information Flow Diagram: Create a visual representation of how information flows through the system. This diagram helps identify potential threats and attack vectors.

Whiteboard Your Architecture: Whiteboarding the system architecture is essential for communication and understanding. It helps frame discussions and ensures that the architecture is well-understood.

Manage DFD in the Context of MVC: Divide the Data Flow Diagram into the Model, View, Controller (MVC) context to better understand the system's components.

Use Tools for Diagrams: Various tools, such as OWASP Threat Dragon, Poirot, MS TMT, and OWASP PYTM, can be used to draw diagrams and visualize the threat model.

Define Data Flow Over DFD: Clearly define data flows within the organization's Data Flow Diagram to understand how data moves through the system.

Define Trust Boundaries: Identify and define trust boundaries within the system, differentiating between external and internal boundaries.

Define Application User Roles and Trust Levels: Specify access rights and trust levels granted to external and internal entities within the application.

Highlight Authorization per User Role: Highlight the authorization levels associated with user roles in the Data Flow Diagram.

Define Application Entry Points: Identify interfaces through which potential attackers can interact with the application or supply data.

Identify Threat Agents: Identify possible threat agents and understand their motivations, means, and opportunities to carry out attacks.

Map Threat Agents to Entry Points: Associate threat agents with application entry points, considering insider threats as well.

Draw Attack Vectors and Attack Trees: Create attack vectors and attack trees to understand the potential paths attackers could take.

Mapping Abuse Cases to Use Cases: Develop abuse cases for each application use case to identify logical threats and vulnerabilities.

Re-Define Attack Vectors: After defining initial attack vectors, consider how compromising user roles might lead to further attacks and redefine vectors accordingly.

Write Threat Traceability Matrix: Document threats and their relationships with assets, entry points, and attack vectors.

Define Impact and Probability for Each Threat: Evaluate threats by assessing their potential impact and likelihood using risk management methodologies like DREAD or PASTA.

By following these steps, organizations can establish a comprehensive threat model for their applications, enabling them to proactively identify and mitigate potential security threats and vulnerabilities.


# Security Hygiene

Maintaining good security hygiene is essential for everyone, whether you're an individual, a business owner, or an average computer user. While some security practices may require a bit more technical knowledge, many fundamental principles can be followed by anyone. Here's a list of basic security practices that everyone should follow, along with some practices that might be considered useful but could be slightly more advanced:

Basic Security Practices for Everyone:

1. Use Strong, Unique Passwords: Create complex passwords for your accounts and avoid using the same password for multiple accounts. Consider using a reputable password manager to store and generate secure passwords.

2. Keep Software Updated: Regularly update your operating system, applications, and antivirus software. These updates often include security patches that protect against known vulnerabilities.

3. Beware of Phishing: Be cautious of unsolicited emails, messages, or phone calls asking for personal information or urging immediate action. Verify the sender's identity before responding or clicking on any links.

4. Secure Your Wi-Fi Network: Use strong encryption (WPA3) for your Wi-Fi network and change the default router login credentials. Avoid sharing your Wi-Fi password with others unless necessary.

5. Regular Backups: Back up important data regularly to an external device or a secure cloud service. This helps protect against data loss from hardware failures or ransomware attacks.

6. Use Antivirus and Anti-Malware Software: Install reputable antivirus and anti-malware software to protect your devices from malware and viruses. Keep these programs up to date.

7. Practice Safe Web Browsing: Be cautious of suspicious websites and only download files or click on links from trusted sources. Use a modern web browser with built-in security features.

8. Lock Your Devices: Set up screen locks or passwords on your devices, including smartphones, tablets, and computers, to prevent unauthorized access.

9. Educate Yourself: Stay informed about common online threats and scams. Educate yourself and your family about safe online practices.

Security Practices That Might Be Slightly More Advanced:

1. Network Firewall Configuration: Adjusting firewall settings on your home router can provide an extra layer of security. This might require some technical knowledge.

2. Regular Security Audits: Conducting periodic security audits of your devices and accounts can help identify vulnerabilities. While anyone can perform basic checks, in-depth audits may require more expertise.

3. Use a Virtual Private Network (VPN): VPNs can enhance privacy and security when browsing the internet. Setting up and configuring a VPN may be slightly more advanced for some users.

4. Secure Email Communication: Implementing encryption for email communication (PGP/GPG) can protect sensitive information but may require technical setup.

5. Secure File Sharing: For those handling sensitive data, using encrypted file-sharing methods like end-to-end encrypted messaging apps or secure cloud storage can be valuable but may involve more complexity.

6. Hard Drive Encryption: Encrypting your hard drive ensures data remains protected if your device is lost or stolen. This process can be more involved for average users.

In conclusion, security hygiene is crucial for everyone's online safety. While many basic security practices can be followed by anyone, some practices may require a bit more technical knowledge or effort. It's essential to strike a balance between implementing robust security measures and ensuring they are practical and manageable for your individual or organizational needs.


# Make-belief boogie-man - a treath model for imaginary company
Threat Model for Imaginary Company: TechSecure Solutions Oy.

Background:
TechSecure Solutions Oy is an imaginary company specializing in providing cutting-edge cybersecurity solutions to various organizations. The company's primary business objective is to develop and offer innovative security software and services to protect client data and systems from cyber threats. As the company deals with sensitive information and operates in the cybersecurity sector, security is at the core of its operations.

What Are We Working On?

In this threat model, we will assess TechSecure Solutions Oy's assets, prioritize them, and understand how security supports the business.

Assets:

Customer Health Data: TechSecure Solutions Oy stores health data for healthcare clients. This is considered a crown jewel asset due to its sensitivity and regulatory requirements.

Proprietary Source Code: The company's intellectual property includes proprietary source code for its cybersecurity solutions. Protecting this code is essential to maintaining a competitive edge.

Client Contracts: The contracts and agreements with clients are crucial assets that must be safeguarded to maintain business trust.

Employee Data: Employee information, including payroll and personal data, is sensitive and must be protected.

Infrastructure: The company's server infrastructure and cloud resources are essential for service delivery and must be secured.

Business and Security Alignment:

The company's core business is to provide cybersecurity solutions to clients. Therefore, security directly supports its business objectives. Ensuring the confidentiality, integrity, and availability of client data and maintaining trust are paramount.

What Can Go Wrong?

We will use the STRIDE model to identify potential threats and analyze the risks associated with them.

STRIDE Analysis:

Spoofing: Unauthorized access to systems or data through identity theft. Example: A malicious actor impersonates an employee to gain access to sensitive data.

Tampering: Unauthorized modification of data or systems. Example: A hacker alters client health records stored on the company's servers.

Repudiation: The inability to verify the origin or authenticity of actions or data. Example: An employee disputes a transaction, and there is no way to prove or disprove their claim.

Information Disclosure: Unauthorized access leading to the exposure of sensitive information. Example: A data breach exposes client health data, leading to regulatory fines.

Denial of Service (DoS): Attackers disrupt services, causing system unavailability. Example: A DoS attack on the company's servers disrupts client services.

Elevation of Privilege: Unauthorized users gain elevated access rights. Example: A hacker exploits a vulnerability to gain admin-level access to the system.

Identified Risks:

Risk 1: Data breach leading to customer health data exposure.
Risk 2: Intellectual property theft of proprietary source code.
Risk 3: Unauthorized access to employee payroll data.
Risk 4: Service disruption due to DoS attacks.
Risk Prioritization:

Risk 1 is of high concern due to its potential legal and reputational consequences. Risk 2 is also critical as it can impact the company's competitive advantage. Risks 3 and 4 are significant but are prioritized lower.

What Are We Going to Do About It?

To mitigate the identified risks:

Reduce Attack Surface: Implement strict access controls and authentication mechanisms to prevent unauthorized access.
Limit Entry Points: Employ firewalls, intrusion detection systems, and secure coding practices to reduce the attack surface.
Continuous Monitoring: Implement continuous threat monitoring to detect and respond to threats in real-time.
Data Encryption: Encrypt sensitive data at rest and in transit.
Regular Security Audits: Conduct regular security audits and penetration tests to identify vulnerabilities.

Did We Do a Good Enough Job?

To evaluate the effectiveness of security measures:
Security Audits: Regular security audits will be conducted to assess the effectiveness of security controls.
Penetration Testing: External penetration testing will be performed annually to identify weaknesses.
Continuous Threat Modeling: Continuously update and refine the threat model to adapt to evolving threats.
In conclusion, TechSecure Solutions Oyhas identified and prioritized potential threats and developed a plan to mitigate them effectively. By aligning security with business objectives and continuously evaluating the threat landscape, the company aims to maintain a high level of security and protect its critical assets.


