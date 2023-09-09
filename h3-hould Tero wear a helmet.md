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
