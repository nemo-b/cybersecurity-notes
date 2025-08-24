COURSE LEARNINGS:

- Assets organizations protect
- Security systems and controls
- Common vulnerabilities in systems
- Threats to asset security

**Risk**: Anything that can impact the confidentiality, integrity, or availability of an asset

Security risk planning:

- Assets
- Threats
- Vulnerabilities

**Asset**: An item perceived as having value to having an organization

**Threat**: Any circumstance or event that can negatively impact assets

**Vulnerability**: A weakness that can be exploited by a threat

**Asset management**: The process of tracking assets and the risks that affect them

**Asset inventory**: A catalog of assets that need to be protected

**Asset classification**: The practice of labeling assets based on sensitivity and importance to an organization

**Levels of classification**:

- **Public**: Assets that can be shared with anyone
- **Internal-only**: Assets that can be shared with anyone in the organization, but should not be shared outside of it
- **Confidential:** Assets that should only be accessed by people working on a specific property
- **Restricted**: Highly sensitive information that must be protected

**Data**: Information that is transferred, processed, or stored by a computer

**States of data**:

- Data in use: Data being accessed by one or more users
- Data in transit: Data travelling from one point to another
- Data at rest: Data not currently being accessed

**Information security (InfoSec)**: The practice of keeping data in all states away from authorized users

**Types of risk categories**: 

- Damage
- Disclosure
- Loss of information

Elements of a security plan

- Policies: A set of rules that reduces risk and protects information
- Standards: References that inform how to set policies
- Procedures: Step-by-step instructions to preform a specific security task

**Compliance**: The process of adhering to internal standards and external regulations

**Regulations**: rules set by a government or other authority to control the way something is done

**NIST Cybersecurity Framework (CSF)**: A voluntary framework that consists of standards, guidelines and best practices to manage cybersecurity risk

Five functions of the NIST CSF core

- Identify
- Protect
- Detect
- Respond
- Recover

**Security controls**: Safeguards designed to reduce specific security risks

**Information privacy**: The protection of unauthorized access and distribution of data

**Data owner**: The person that decides who can access, edit, use, or destroy their information

**Data custodian**: Anyone or anything that's responsible for the safe handling, transport, and storage of information

**Personally identifiable information (PII)**: Any information that can be used to infer an individual's identity

**Cryptography**: The process of transforming information into a form that unintended readers can't understand

Cryptography process:

- Encryption: Hides the information
- Decryption: Shows the Information

**Algorithm**: A set of rules used that solve a problem

**Cypher**: An algorithm that encrypts information

**Cryptographic key**: A mechanism that decrypts cypher text

**Brute force attack**: A trial and error process of discovering private information

**Public Key Infrastructure (PKI)**: An encryption framework that secures the exchange of information online

**Public key infrastructure process**: 

- Exchange of encrypted information
    1. Asymmetric encryption: the use of a public and private key pair for encryption and decryption of data
    2. Symmetric encryption: The use of a single secret key to exchange. Information
- Establish trust using a system of digital certificates

**Digital certificate**: A file that verifies the identity of a public keyholder

**Hash function**: An algorithm that produces a code that can't be decrypted

**Non-reputation**: The concept that the authenticity of information can't be denied

**Access controls**: Security controls that manage access, authorization, and accountability of information

**Single sign-on (SSO)**: A technology that combines several different logins into one

**Multifactor authentication (MFA)**: A security measure which requires a user to verify their identity in two or more ways to access a system or network

**AAA framework**

- Authentication
- Authorization
- Accounting

**Separation of duties**: The principle that users should not be given levels of authorization that would allow them to misuse a system

**Basic auth**: The technology used to establish a user’s request to access a server

**OAuth**: An open-standard authorization protocol that shares designated access between applications

**API token**: A small block of encrypted code that contains information about a user

**Session**: A sequence of networking HTTP basic auth requests and responses associated with the same user

**Session ID**: A unique token that identifies a user and their device while accessing the system

**Session cookie**: A token that websites use to validate a session and determine how long that session should last

Session hijacking: An event when attackers obtain a legitimate user’s session ID

**Vulnerability**: A weakness that can be exploited by a threat

**Exploit**: A way of taking advantage of a vulnerability

**Vulnerability management**: The process of finding and patching vulnerabilities

**Vulnerability management steps**:

1. Identify vulnerabilities
2. Consider potential exploits
3. Prepare defenses against threats
4. Evaluate those defenses

**Zero-day**: an exploit that was previously unknown

**Exposure**: A mistake that can be exploited by a threat

**Common Vulnerabilities and Exposures list (CVE™ list)**: An openly accessible dictionary of known vulnerabilities and exposures

**CVE™ list criteria**

1. Independent of other issues
2. Recognized as a potential security risk
3. Submitted with supporting evidence
4. Only affect one codebase

**Common Vulnerability Scoring System (CVSS)**: A measurement system that scores the severity of a vulnerability

**Vulnerability assessment**: The internal review process of an organization’s security systems

Vulnerability assessment process

1. Identification
2. Vulnerability analysys
3. Risk asesment
4. Remediation

**Attack surface**: All the potential vulnerabilities that a threat actor could exploit

**Security hardening**: The process of strengthening a system to reduce its vulnerabilities and attack surface

**Attack vectors**: The pathways attackers use to penetrate security defenses

**Practicing an attacker mindset**:

1. Identify a target
2. Determine how the target can be accessed
3. Evaluate attack vectors that can be exploited
4. Find the tools and methods of attack

**Defending attack vectors**

1. Educating users
2. Applying the principle of the least privilege
3. Using the right security controls and tools

**Threat**: Any circumstance or event that can negatively impact assets

**Social engineering**: A manipulation that exploits human error to gain private information, access, or valuables

**Phishing**: The use of digital communications to trick people into revealing sensitive data or deploying malicious software

**Phishing kit tools**

- Malicious attachments
- Fake data-collection forms
- Fraudulent web links

**Smishing**: The use of text messages to obtain sensitive information or to impersonate a known source

**Malware**: Software designed to harm devices or networks

**Types of malware**:

1. **Virus**: malicious code written to interfere with computer operations and cause damage to data and software
2. **Worm**: Malware that can duplicate and spread itself across a system on its own
3. **Trojan** (or Trojan horse): Malware that looks like a legitimate file or program
4. **Ransomware**: A type of malicious attack where attackers encrypt an organizations data and demand payment to restore access
5. **Spyware**: Malware that's used to gather and sell information without consent

**Cryptojacking**: A form of malware that installs software to illegally mine cryptocurrencies

**Intrusion detection systems (IDS)**: An application that monitors system activity and alerts on possible intrusions

**Signs of crypojacking**:

- slowdown
- Increased CPU usage
- Sudden system crashes
- Fast draining batteries
- Unusually high electricity costs

**Web-based exploits**: Malicious code or behavior that’s used to take advantage of coding 

**Injection attack**: Malicious code inserted into a vulnerable application

**Cross-site scripting (XSS)**: An injection attack that inserts code into a vulnerable website or web application

**Reflected XSS attack**: An instance when malicious script is sent to a server and activated during the server's response

**Stored XSS attack**: An instance when malicious script is injected directly on the server

**DOM-based XSS attack**: An instance when malicious script exists in the webpage a browser loads

**SQL (Structured Query Language)**: A programming language used to create, interact with, and request information from a database

**SQL injection**: An attack that executes unexpected queries on a database

**Prepared statement**: A coding technique hat executes SQL statements before passing them onto the database

**Threat modeling**: The process of identifying assets, their vulnerabilities, and how each is exposed to threats

**Threat modelling**: The process of identifying assets, their vulnerabilities, and how each is exposed to threats

**Threat modelling steps**: 

1. Define the scope
2. Identify threats
    - **Threat actor**: Any person or group who presents a security risk
    - **Attack tree**: A diagram that maps threats to assets
3. Characterize the environment
4. Analyze threats
5. Mitigate risks
6. Evaluate findings

**PASTA**: A popular threat modeling framework that’s used across many industries

**P**rocess for

**A**ttack

**S**imulation and

**T**hreat

**A**nalysis

PASTA threat model framework

1. Define business and security objectives components that must be values
2. Define the technical scope
    - Teams focus is on identifying the application
3. Decompose the application
    - Identifying the existing controls that will protect user data from threats. Normally means working with the application developers to produce a data flow diagram to show how data gets from a user's device, to the companies database. It also identifies controls in place to protect the data along the way.
4. Perform a threat analysis
    - This is where the team gets into their attacker mindset. Here research is done to collect the most up-to-date information on the type of attacks being used.
5. Perform a vulnerability analysis
    - Here the team works deeply to investigate potential vulnerabilities
6. Conduct attack modeling
    - Here is where the team tests the vulnerabilities that were analyzed in stage five by simulating attacks. This is done by creating an attack tree, which looks like a flow chart. here is an example below.
        
        ![Screen Shot 2024-03-25 at 10.47.48 PM.png](Screen_Shot_2024-03-25_at_10.47.48_PM.png)
        
7. Analyze risk and impact
    - Here, the team assembles all the information collected through steps 1 - 6. By now, the team is in position to make informed risk management recommendations to buisness stakeholders that align with their goals.
