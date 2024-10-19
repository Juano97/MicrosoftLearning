# Describe the concepts of security compliance and identity 

## Concepts Learned

### Areas of responsibility between the customer and the cloud provider, according to where data is held

![alt text](image.png)

>`On-premises datacenters.` In an on-premises datacenter, you have responsibility for everything from physical security to encrypting sensitive data.>

>`Infrastructure as a Service (IaaS).` Of all cloud services, IaaS requires the most management by the cloud customer. With IaaS, you're using the cloud provider’s computing infrastructure. The cloud customer isn't responsible for the physical components, such as computers, the network, or the physical security of the datacenter. However, the cloud customer st>ll has responsibility for software components running on that computing infrastructure such as operating systems, network controls, applications, and protecting data.

>`Platform as a Service (PaaS).` PaaS provides an environment for building, testing, and deploying software applications. The goal of PaaS is to help you create an application quickly without managing the underlying infrastructure. With PaaS, the cloud provider manages the hardware and operating systems, and the customer is responsible for applications and dat>a

>`Software as a Service (SaaS).` SaaS is hosted and managed by the cloud provider, for the customer. It's usually licensed through a monthly or annual subscription. Microsoft 365, Skype, and Dynamics CRM Online are all examples of SaaS software. SaaS requires the least amount of management by the cloud customer. The cloud provider is responsible for managing e>verything except data, devices, accounts, and identities

### Defense in Depth Layers of Security:

> `Physical` security such as limiting access to a datacenter to only authorized personnel.

> `Identity and access` security controls, such as multifactor authentication or condition-based access, to control access to infrastructure and change control.

> `Perimeter` security of your corporate network includes distributed denial of service (DDoS) protection to filter large-scale attacks before they can cause a denial of service for users.

> `Network` security, such as network segmentation and network access controls, to limit communication between resources.

> `Compute` layer security such as securing access to virtual machines either on-premises or in the cloud by closing certain ports.

> `Application` layer security to ensure applications are secure and free of security vulnerabilities.

> `Data` layer security including controls to manage access to business and customer data and encryption to protect data.

### Confidentiality, Integrity, Availability (CIA)

> `Confidentiality` refers to the need to keep confidential sensitive data such as customer information, passwords, or financial data. You can encrypt data to keep it confidential, but then you also need to keep the encryption keys confidential. Confidentiality is the most visible part of security; we can clearly see need for sensitive data, keys, passwords, and other secrets to be kept confidential.

> `Integrity` refers to keeping data or messages correct. When you send an email message, you want to be sure that the message received is the same as the message you sent. When you store data in a database, you want to be sure that the data you retrieve is the same as the data you stored. Encrypting data keeps it confidential, but you must then be able to decrypt it so that it's the same as before it was encrypted. Integrity is about having confidence that data hasn't been tampered with or altered.

> `Availability` refers to making data available to those who need it, when they need it. It's important to the organization to keep customer data secure, but at the same time it must also be available to employees who deal with customers. While it might be more secure to store the data in an encrypted format, employees need access to decrypted data.

### Zero Trust guiding principles

> `Verify explicitly.` Always authenticate and authorize based on the available data points, including user identity, location, device, service or workload, data classification, and anomalies.

> `Least privileged access.` Limit user access with just-in-time and just-enough access (JIT/JEA), risk-based adaptive policies, and data protection to protect both data and productivity.

> `Assume breach.` Segment access by network, user, devices, and application. Use encryption to protect data, and use analytics to get visibility, detect threats, and improve your security.

#### Six foundational pillars

> `Identities` may be users, services, or devices. When an identity attempts to access a resource, it must be verified with strong authentication, and follow least privilege access principles.

> `Devices` create a large attack surface as data flows from devices to on-premises workloads and the cloud. Monitoring devices for health and compliance is an important aspect of security.

> `Applications` are the way that data is consumed. This includes discovering all applications being used, sometimes called Shadow IT because not all applications are managed centrally. This pillar also includes managing permissions and access.

> `Data` should be classified, labeled, and encrypted based on its attributes. Security efforts are ultimately about protecting data, and ensuring it remains safe when it leaves devices, applications, infrastructure, and networks that the organization controls.

> `Infrastructure`, whether on-premises or cloud based, represents a threat vector. To improve security, you assess for version, configuration, and JIT access, and use telemetry to detect attacks and anomalies. This allows you to automatically block or flag risky behavior and take protective actions.

> `Networks` should be segmented, including deeper in-network micro segmentation. Also, real-time threat protection, end-to-end encryption, monitoring, and analytics should be employed.

### Encryption and Hashing

#### Encryption for data at rest
Data at rest is the data that's stored on a physical device, such as a server. It may be stored in a database or a storage account but, regardless of where it's stored, encryption of data at rest ensures the data is unreadable without the keys and secrets needed to decrypt it.

If an attacker obtained a hard drive with encrypted data and didn't have access to the encryption keys, they would be unable to read the data.

#### Encryption for data in transit
Data in transit is the data moving from one location to another, such as across the internet or through a private network. Secure transfer can be handled by several different layers. It could be done by encrypting the data at the application layer before sending it over a network. HTTPS is an example of encryption in transit.

Encrypting data in transit protects it from outside observers and provides a mechanism to transmit data while limiting the risk of exposure.

#### Encryption for data in use
A common use case for encryption of data in use involves securing data in nonpersistent storage, such as RAM or CPU caches. This can be achieved through technologies that create an enclave (think of this as a secured lockbox) that protects the data and keeps data encrypted while the CPU processes the data.

#### Hashing
Hashing uses an algorithm to convert text to a unique fixed-length value called a hash. Each time the same text is hashed using the same algorithm, the same hash value is produced. That hash can then be used as a unique identifier of its associated data.

Hashing is different to encryption in that it doesn't use keys, and the hashed value isn't subsequently decrypted back to the original.

Hashing is often used to store passwords. When a user enters their password, the same algorithm that created the stored hash creates a hash of the entered password. This is compared to the stored hashed version of the password. If they match, the user has entered their password correctly. This is more secure than storing plain text passwords, but hashing algorithms are also known to hackers. Because hash functions are deterministic (the same input produces the same output), hackers can use brute-force dictionary attacks by hashing the passwords. For every matched hash, they know the actual password. To mitigate this risk, passwords are often “salted”. This refers to adding a fixed-length random value to the input of hash functions to create unique hashes for same input.

### Governance, Risk, and Compliance (GRC)

#### Governance
Governance is the system of rules, practices, and processes an organization uses to direct and control its activities. Many governance activities arise from external standards, obligations, and expectations. For example, organizations establish rules and process that define the who, what, where, and when users and applications can access corporate resources and who has administrative privileges and for how long.

#### Risk
Risk management is the process of identifying, assessing, and responding to threats or events that can impact company or customer objectives. Organizations face risk from both external and internal sources. External risks can come from political and economic forces weather related events, pandemics, and security breaches to name just a few sources. Internal risks are risks that come from within the organization itself. Examples include leaks of sensitive data, intellectual property theft, fraud, and insider trading.

#### Compliance
Compliance refers to the country/region, state, or federal laws or even multi-national regulations that an organization must follow. These regulations define what types of data must be protected, what processes are required under the legislation, and what penalties are issued to organizations that fail to comply.

It's important to note that compliance is not the same as security. But, security should be considered when building a compliance plan as effective security is frequently a compliance requirement. Compliance requires only that the legally mandated minimum standards are met whereas data security covers all the processes, procedures, and technologies that define how you look after sensitive data and guard against breaches.

Some compliance-related concepts include:

Data residency - When it comes to compliance, data residency regulations govern the physical locations where data can be stored and how and when it can be transferred, processed, or accessed internationally. These regulations can differ significantly depending on jurisdiction.
Data sovereignty - Another important consideration is data sovereignty, the concept that data, particularly personal data, is subject to the laws and regulations of the country/region in which it's physically collected, held, or processed. This can add a layer of complexity when it comes to compliance because the same piece of data can be collected in one location, stored in another, and processed in still another; making it subject to laws from different countries/regions.
Data privacy - Providing notice and being transparent about the collection, processing, use, and sharing of personal data are fundamental principles of privacy laws and regulations. Personal data means any information relating to an identified or identifiable natural person. Privacy laws encompass any data that is directly linked or indirectly linkable back to a person. Organizations are subject to, and must operate consistent with, a multitude of laws, regulations, codes of conduct, industry-specific standards, and compliance standards governing data privacy.
All organizations manage data so understanding terminology and concepts related to compliance is important as they work to meet the minimum, mandated laws and/or regulations.

