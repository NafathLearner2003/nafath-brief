Version: NAFATH-V3

Track: Networking

##Overview

A government AI assistant in a mobile app depends on six IT fields working together. Software engineering provides reliable application features and manages changes to the assistant’s API. Artificial intelligence helps the assistant understand questions and retrieve relevant information to generate useful answers. Mobile engineering makes the assistant accessible through a convenient app and protects communication with secure connections. Networking allows the app, servers, and data sources to communicate efficiently as more citizens use the service. Cybersecurity protects the assistant and its users from attacks, unauthorized access, and malicious instructions. Data engineering supports the responsible storage, organization, and protection of chat logs while respecting privacy. These fields are connected: the mobile app sends requests through the network, software processes them, AI generates responses using data, and security controls help protect every stage. Together, they support a dependable public service that citizens can use with confidence. The Networking research question focuses on IPv6 addressing and its importance as connected devices increase.

##Software

Under Semantic Versioning, the assistant’s public API must increase its MAJOR version when incompatible changes are introduced, such as removing or changing an existing endpoint or parameter. A MINOR version increase is required when new functionality is added in a backward-compatible way, such as introducing a new endpoint. A PATCH version increase is used for backward-compatible bug fixes that do not change the API’s expected behavior. Following these rules helps developers understand the impact of updates and maintain compatibility between the assistant and its clients.

Resource: Semantic Versioning 2.0.0 — https://semver.org/

##AI

Retrieval-Augmented Generation (RAG) is a technique that allows an AI system to retrieve relevant information from trusted external sources before generating an answer. Instead of relying only on information learned during training, the assistant uses retrieved documents or data to support its response. RAG can reduce incorrect answers by grounding responses in relevant evidence and helping the model provide more accurate, up-to-date information. However, its reliability still depends on the quality of the retrieved sources and how well the assistant uses them.

Resource: What Is Retrieval-Augmented Generation (RAG)? — https://aws.amazon.com/what-is/retrieval-augmented-generation/

##Mobile

App Transport Security (ATS) is an iOS security feature that requires apps to use secure network connections that meet Apple’s security standards, typically HTTPS with modern TLS settings. It helps protect data while it travels between the app and a server. If an app tries to connect to a plain HTTP endpoint, ATS normally blocks the connection because it is not secure. The developer must use HTTPS or configure a specific exception when there is a justified need, rather than weakening security for all connections.

Resource: Preventing Insecure Network Connections — https://developer.apple.com/documentation/bundleresources/information-property-list/nsapptransportsecurity

##Networking

IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses, providing a much larger address space. IPv4 has about 4.3 billion possible addresses, whereas IPv6 supports an enormously larger number. This matters as more phones, computers, sensors, and other connected devices need unique addresses. IPv6 helps support this growth and improves address allocation and network scalability, reducing the limitations caused by the shortage of IPv4 addresses.

Resource: RFC 8200 — Internet Protocol, Version 6 (IPv6) Specification — https://www.rfc-editor.org/rfc/rfc8200

##Cybersecurity

Prompt injection is an attack that attempts to manipulate an AI system into ignoring its intended instructions or performing unintended actions. Direct prompt injection comes from instructions entered directly by a user. Indirect prompt injection is hidden in external content, such as a webpage or document that the AI processes. Two ways to reduce risk are to limit the AI’s permissions using the principle of least privilege and to separate untrusted external content from trusted instructions while validating sensitive actions.

Resource: OWASP — LLM Prompt Injection Prevention Cheat Sheet — https://cheatsheetseries.owasp.org/cheatsheets/LLM_Prompt_Injection_Prevention_Cheat_Sheet.html

##Data

Anonymization removes identifying information so that data can no longer reasonably be linked to an individual. Pseudonymization replaces direct identifiers with artificial labels or codes, but the data may still be linked to a person using additional information kept separately. Therefore, pseudonymized chat logs are still considered personal data under the GDPR. Truly anonymized data falls outside the scope of EU data protection law because individuals can no longer be identified from it.

Resource: European Data Protection Board — Anonymisation / Pseudonymisation — https://www.edpb.europa.eu/topics/ai-and-technology/anonymisation-pseudonymisation_en


##Misconception in My Track

A common misconception is that IPv6 is simply a faster version of IPv4. In reality, the main difference is the address size: IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses. IPv6 provides a much larger address space to support the growing number of connected devices. The Internet Protocol, Version 6 (IPv6) Specification explains the IPv6 protocol and its addressing structure. This shows that IPv6 is mainly important for addressing capacity and network scalability, not just speed.

Resource evidence: RFC 8200, “Internet Protocol, Version 6 (IPv6) Specification,” sections 2 and 3 — https://www.rfc-editor.org/rfc/rfc8200

##Open Question

How can organizations migrate from IPv4 to IPv6 while keeping existing services available and secure?
