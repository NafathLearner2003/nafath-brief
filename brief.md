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
##Cybersecurity
##Data
##Misconception in My Track
##Open Question
