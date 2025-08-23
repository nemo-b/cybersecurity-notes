## **Secure Baselines - CompTIA Security+ SY0-701 - 4.1**

### Secure baselines

- This is just the standard set at a company of how things should be taken care of
    - The Windows website has a list of security baselines to use with tools to deploy them on different Windows devices, which is known as the Security Compliance Toolkit (SCT)
    - After you deploy changes, you generally don't have to touch it again as they are usually never changed

## **Hardening Targets - CompTIA Security+ SY0-701 - 4.1**

### Hardening

- No system is secure with default configurations, so you need guidelines to keep everything safe
- Hardening guides are guides that are specific to individual pieces of software or platforms
- Mobile devices are a good example of something that must be hardened
    - Phones, tablets, etc
    - Hardening checklists are av alible from manufacturers

### Workstations

- This is Windows, macOS, Linus, etc.
- You constantly need to monitor and update every device and automate processes for monthly patches
- Be sure to remove unnecessary software as every software is a risk

### Network infrastructure devices

- Switches, routers, etc
- These are purpose built and need to be configured
- Be sure to change things like default credentials and passwords

### Cloud infrastructure

- The Least privilege
    - Only give people enough control to do their job, no more
- Configure endpoint Detection and Response (EDR)
    - All devices accessing the cloud should be secure
- Always have backups like cloud to cloud (C2C)

### Servers

- Set policies for things like user accounts & limit network access
- Monitor and secure with Anti-virus and Anti-malware
- Update constantly and patch

### SCADA / ICS

- For industrial places, SCADA and ICS are common place for showing real time updates on how the machines are working
- Supervisory Control and Data Acquisition System (SCADA)

### RTOS

- **Real Time Operating System (RTOS)**: This is an operating system with a deterministic processing schedule; no time to wait for other processes and primarily used for industrial equipment
- Should be separated from other areas (Isolate the system)
- Secure the system with a firewall

### Embedded systems

- Hardware or software used for specific function
- Need to be segmented or fire walled

## **Securing Wireless and Mobile - CompTIA Security+ SY0-701 - 4.1**

### Site surveys

- Site surveys determine what areas are reached in an existing wireless landscape
    
    ![This is an example image of what a “Heat map” site survey. Should look familiar upon first look. ](Screenshot_from_2025-06-13_13-54-57.png)
    
    This is an example image of what a “Heat map” site survey. Should look familiar upon first look. 
    
- Checking site surveys on interval can help you work around wireless service issues and finding the best places for certain procedures to happen, as well as locate areas of risk
- Wireless survey tools
    - Signal coverage
    - Potential interference
    - Built-in tools
    - 3rd-party tools
    - spectrum analyzer
- **Mobile Device Manager (MDM):** This is a type of security software that helps IT departments set rules to secure, monitor, and manage mobile devices used by people in a company.
    - One thing you could do with MDM is disable cameras on people's personal phone while on company property, and re-enable it when off of the premises
    - BYOD - Bring your own device
        - this is when people bring their own devices to use for both personal and company purposes
        - These are limited to specific qualifications so that the program to use company services can work on them properly
    - COPE - Company owned, personally enables
        - Organization still has full ownership of the device
        - CYOD -Choose your own device
        - Similar to COPE, but the user picks what type of corporate owned device they'd like

## **Wireless Security Settings - CompTIA Security+ SY0-701 - 4.1**

### Securing

- Securing wireless networks is important because if you don't, it's practically the same as making information completely public to people that can access that network
- You need to authenticate people with things like username and password when first connecting

### The WPA2 PSK problem

- WPA2 has a PSK brute force problem
    - Listen to the four way handshake
        - Some methods derive from the PSK hash without the handshake
    - Capture the hash
- With the hash, attackers can brute force the **pre-shared key (PSK)**
- A weak PSK is easy to brute force
- Cloud based password cracking

### SAE

- WPA3 changes the PSK authentication process
    - This includes mutual authentication
    - Creates a shared session key without sending that key across the network
    - No more four way handshakes, n hashes, no brute force attacks
- Simultaneous Authentication of Equals (SAE)
    - A Diffie-Hellman derived key exchange with an authentication component
    - Everyone uses a different session key, even with the same PSK
    - An IEEE standard - the dragonfly handshake

### Wireless security modes

- Configure the authentication on your wireless access / wireless router
- Open system
    - No authentication password is required
- WPA3-Personal / WPA3-PSK
    - WPA2 or WPA3 with a pre-shared key
    - Everyone uses the same 256-bit key
- WPA3-Enterprise / WPA3-802.1X
    - Authenticates users individually with an authentication server (i.e.. RADIUS)

### AAA framework

- Identification
- Authentication
- Authorization
- Accounting

### IEEE 802.1X

- IEEE 802.1X
    - Port-based Network Access Control (NAC)
    - You don't get access to the network until you authenticate
- Used in conjunction with an access database
    - RADIUS, LDAP, TACACS+

### EAP

- Extensible Authentication Protocol (EAP)
    - An authentication framework
- Many different ways to authenticate based on RFC standards
    - Manufacturers can build their own EAP methods
- EAP integrates with 802.1X
    - Prevents access t the network until the authentication succeeds

### IEEE 802.1X and EAP (Revision because I've written notes already)

- Supplicate - the client
- Authenticator - The device that provides access
- Authentication server - Validates the client credentials

## **Application Security - CompTIA Security+ SY0-701 - 4.1**

### Secure coding concepts

- A balance between time and quality
    - Programming with security in mind is often secondary
- You test ALOT for the Quality Assurance (QA) process
- Vulnerabilities are eventually found and will be exploited

### Input validation

- What's the expected input?
- Normalization is when you check and correct all inputs
    - EX: Zip codes should only be X characters long with a letter X in the column
    - You use this to fix any data with improper input
- Fuzzers will find what you miss
    - **Fuzzers**: A fuzzer in cybersecurity is a tool or technique used to discover vulnerabilities in software applications by inputting random, unexpected, or invalid data, known as "fuzz," into the system. This process aims to uncover flaws in the software's handling of inputs, which can lead to crashes, memory leaks, or security breaches.

### Secure cookies

- Cookies are simply data files that hold valuable information that hackers can and will target. These are used for tracking, personalization, and session management.
- Cookies don't have special securities, and anything put into a cookie is easily read from the browser
    - Because it isn't very protected, application developers don't put sensitive information into cookies, as it could be seen by a third party.

### Static code analyzers*

- **Static Application Security Testing (SAST)**: This is a tool to help identify security flaws
    - These aren't perfect, but it does quickly and notably show what problems are occurring in the systems

### Code signing

- Code signing finds out how to notice if malware is hidden inside an application
- It works by seeing is the application has been modified in any way, and trying to confirm the application was made by a specific developer
- This works like other digital signature process by using asymmetric encryption, and developing a public and private key

### Sandboxing

- When running an application, it could be run in a sandbox, which only gives the application enough information to work
    - These are usually used during development
- They run through many different deployments
    - Virtual machines
    - Mobile devices
    - Browser iframes (Inline Frames)
    - Windows User Account Control (UAC)

## **Asset Management - CompTIA Security+ SY0-701 - 4.2**

### Acquisition/procurement process

- **The purchasing process**: This is a multistep process for requesting and obtaining goods and services from third parties
- This starts with a request from a user, and leads to budgeting information, formal approvals, negotiation, and then purchase & payment

### Assignment/accounting

- A central asset tracking system that can be used from different parts of the organization
- Ownership
    - Associate a person with an asset
    - Useful for tracking a system
    - You also need to classify what type of asset it is
        - Hardware
        - Software
        - Other…

### Monitoring/asset tracking

- Inventory every asset
- Associate a support ticket with a device and make model
    - Can be more detailed than a user's description
- Enumeration
    - List all parts of an asset including CPU, memory, storage drive, keyboard, mouse
- Add an asset tag like bar codes, RFID, visible tracking number, the organization name, etc.
    - (Similar to bar code and number at the bottom of school chromebooks)

### Media sanitation

- This is the cleaning of information ff of a device so that it can be used for a different purpose or disposing
- If you want to make sure nobody ever sees the information in a drive, you should physically destroy the drive
    - This could mean cutting, smashing, and some companies even burn the drives
    - Some companies even rely on outside third parties to destroy the drives
    
    Vulnerability Scanning - CompTIA Security+ SY0-701 - 4.3
    

### Data retention

- This is how you back up and save data
- You should always prepare for the loss of data, and sometimes, even the loss of  backup as well
- Different types of data need different types of retention, so understand clearly what type of backups you need beforehand

## **Vulnerability Scanning - CompTIA Security+ SY0-701 - 4.3**

### Vulnerability scanning

- These are usually minimally invasive unlike penetration testing
- Port scans look around ports to see what is open
- These should be tested from the outside AND the inside
- These are mildly inaccurate, so be sure to double check vulnerabilities

### Static code anylizer

- These are important for the process so go up to “**Application Security - CompTIA Security+ SY0-701 - 4.1**” for those notes

### Dynamic anaysis (fuzzing)

- Send random input to an application
    - Fault-injecting, robustness testing, syntax testing, negative testing
- Carnegie Mellon Computer Emergency Response Team (CERT): this is the certification for basic Fuzzing Frameworking (BFF) and can be found at professor messers website
- Fuzzing is also breifly mentioned in 4.1 so look there for extended notes

## **Threat Intelligence - CompTIA Security+ SY0-701 - 4.3**

### Threat intelegence

- You need to keep an open eyer for every threat or possible threat actor
- Make decisions based on intelegence
- Data is everywhere
    - You may be able to find information on groups of hackers and their motives
    - Tools used by hackers and how they work
    - Etc.

### Oen-source intelegence (OSINT)

- Open-source resources are publicly avalible and a good place to find information
- The internet has disscussion groups and social media with information to look for there
- Government data can be viable to use as it could have informaition on public hearings, reports, websites, and more
- Commercial data from maps, financial reports, and databases could also be useful

Proprietary/third-party intelegence

- People have already compiled the threat information, and all thats left to do is buy it from them
- Threat intelegence services are important because understanding the usage of a threat service is important in solving the issue
- Constant threat monitoring
    - Be sure to have automated prevention workflows

Information-sharing Orginization

- Public threat intelegence
    - Often classified information
- Private threat intelegence
    - Private companies have extensive resources
- Need to share critical security details
    - Real time, high-quality cyber threat information sharing

Dark web intelegence

- Dark web
    - Overlay networkks that use the internet
    - Requires spesific software and configurations to access
- Hacking groups and services are very active on the darkweb, making it a very good place t find information, though also a dangerous place to search
    - Activies of groups can be found
    - Tools and techniques
    - Credit card sales
    - Accounting and passwords

## Penetration Testing - CompTIA Security+ SY0-701 - 4.3

### Penetration testing

- **Penetration testing**, also known as **pentesting**, is a way to test systems and look for vulnerabilities by simulating an attack on your own systems in a controlled way, similarly to vulnerability scanning
- This form of testing is important nd can often be done by a third party
- Keep in mind depending where the service is reuired, your comany may enforce pentesting as a mandate in your feild

### Rules of engagement

- Rules of engagement define the scope, timing, and parameters for how penetration testing will be conducted within our company
- Be sure everyone knows about the test parameters

### Exploiting vulnerabilities

- Try to personally break into the system
    - BE CAREFUL; this may cause a DoS or loss of data

## **Analyzing Vulnerabilities - CompTIA Security+ SY0-701 - 4.3**

### Dealing with false information

- **False positive**
    - This is a vulnerability that is identified, that doesnt realy exist
    - These are still notable as valid vunerabilities but arent to the severity that it truly is
- **False negative**
    - A vulnerability exists, but you didnt detect it
    - Ths is dangerous as it leads to exploiting that the cybersecurity team wouldnt even know exists

### Prioritizing vulnerabilities

- Not every vulnerability shares the same priority but are usually broken into a High, medium, and low category
- Every company has different standards of what informations priority to protect is, and this leads to the prioritization of vulnerabilities

### CVSS

- National vulnerability database: [http://nvd.nist.gov/](http://nvd.nist.gov/)
- Common Vulnerability Scoring System (CVSS)
    - Quantative scoring of a vulnerability - 0-10
    - Scoring standards change over time
    - Different scoring for CVSS 2.0 vs CVSS 3.x

### CVE

- Common Vulnerabilities Exposures (CVE): [https://cve.mitre.org/cve/](https://cve.mitre.org/cve/)
- The vulnerabilities can be cross refrenced online
    - Almost all scanners give you a place to go
- Some vulnerabilities cannot be definitively identified
    - Youll have to check manually to see if a system is vulnerable
    - The scanner gives you a heads up

Exposure factor

- Loss of value or buisness activity if the vulnerability is exposed
    - This is usually expressed as a percentage
    - Always remember to consider the worst possible outcome
- Examples
    - A small DDoS may limit access to a service
        - 50% exposure factor
    - A buffer overflow may completly disable a service
        - 100% exposure factor

## Vulnerability Remediation - CompTIA Security+ SY0-701 - 4.3

### Patching

- This is a contiuous way to get rid of vulnerabilities slowly
- Scheduled vulnerabilities.patch notices
    - Monthly or quarterly
- Unscheduled patches
    - Zero-day, often urgent

### Insurance

- A way of mitigating risk, or moving the risk to another company would be to let a third party handing the storage which leads to cybersecurty insurance coverage

### Segementation

- This divides a system into different parts
- While if id does get hacked you may lose a whole segment, you can contain thee damage in that segment to keep the rest of the system up and running
- Next generation fire walls (NGFWs) are good for watching the trafffic between segments
- Air gaps may be required if you cant patch
    - This mens physically seperating devices in systems
- Local segementations with VLANs are okay, and can be used on the same device phisically

### Compensating controls

- Optimal security methods may not be avalible
    - Cant deploy a patch right now
    - No internet firewalls
- Compensate in other ways
    - Disable the problematic service
    - Revoke access to the application
    - Limit eternal access
    - Modify internal security controls and software details
- Provide coverage until a patch is deployed
    - Or a similar optimal security response

### Exemptions and examptions

- When a patch cant be made for a system and compensation doesnt work, you can ethier make an eeption to the rule, or get rid of the sstem that cant be patched
- You may have to provide the service, but also the data and systems
- Removing the vulnerability is optimal, but not everything can be patched

Validation of remedation

- The vulnerability is now patched
    - Does the patch really stop the exploit?
    - Did you patch all vulnerable systems
- Rescanning
    - Preform an extensive security scan
- Audit
    - Check remidiated systems to ensure the patch was successfully deployed
- Verification
    - Manually confirm the security of the system

## **Security Monitoring - CompTIA Security+ SY0-701 - 4.4**

### Security monitoring

- Keep  in mind that attackers don't “sleep”. An attack could happen anytime so people need to secure assets 24/7/365
- Monitor all entry points
- Status dashboards
    - Get the status of all systems at a glance

### Monitoring computing resources

- Systems
    - Authentication - Logins from strange places
    - Server monitoring - Service activity, backups, software versions
- Applications
    - Availability - Uptime and response times
    - Data transfers - Increases or decreases in rates
    - Security notifications - From the developer/manufacturer
- Infrastructure
    - Remote access systems - Employees, vendors, guests
    - Firewall and IPS reports - Increase or type of attack

### Log aggregation

- This is how you can collect information in a simple way, and it's done through a SIEM or SEM
- SIEM or EM (Security Information and Event Manager)
    - These consolidate many different logs to a central database
    - Servers, firewalls, VPN concentrators, SANs, cloud services
- Centralized reporting, and it keeps all information in one place

### Scanning

- You need to keep track of moving devices like laptops and mobile devices so you can be sure they're safe before entering your system as a possible vulnerability
- You have to constantly scan as much information as possible so that you can make detailed reports
    - The reports should hold certain things
        - You must create “actionable” reports, which means you need to be able to use the information given
        - It has to have the number of devices up to date/in compliance
        - Devices running older operating systems
        - Devices that have been off and on your systems
        - Etc.

<aside>
💡

IBM did a study, and concluded that it takes about 9 months for a company to identify and contain a breach. This was the IBM security repost in 2022. This is why long terms backup strategies are important. 

</aside>

## **Security Tools - CompTIA Security+ SY0-701 - 4.4**

### Security tools

- There are many different types of security tools av alible
    - NGFWs, IPs, vulnerability scanners, etc
    - They all have their own way of evaluating a threat
- Different tools may describe the same vulnerability in completely different ways. So you can set the vulnerabilities to have the same names across the board, you should use the Security Content Automation Protocol (SCAP). SCAP is a program run by NIST (National Institute of Standards and Technology) ([http://scap.nist.gov](http://scap.nist.gov))
    - SCAP content can be shard between tools
    - It is especially good to use for large environments
    - Because of the simplification, it leads to automation
        - Automation types
            - Ongoing monitoring
            - Notification and alerting
            - Remediation of non-compliant systems

### Benchmark

- Benchmarks are the bare minimum for security settings
- Some popular benchmarks would be found in the Center for Internet Security (CIS)
    - [https://www.cisecurity.org/cis-benchmarks/](https://www.cisecurity.org/cis-benchmarks/)

### Agents/agentless

- These are used to check and see if a device is in compliance
    - You install a software agent on the device and when needed, run an on-demand agentless check
- Agents can provide more detail as they always monitor in real time, though they must be maintained an updated
- Agentless runs without a formal install
    - Performs the check, then disappears
    - Does not require ongoing updates to an agent
    - Will not inform or alert if not running
- These work well with VPN concentrators

<aside>
💡

Refer to SIEM, Anti-Virus/Anti-Malware notes here.

</aside>

### Data Loss Prevention (DLP)

- You must stop data “leakage” before hackers can get their hands on it
- So many sources, so many destinations
    - Often requires multiple solutions
    - Endpoint clients
    - Cloud-based systems
        - Email, cloud storage, collaboration tools

### SNMP

- Simple Network Management Protocol (SNMP)
    - A database of data (MIB) - Management Information Base
    - The database contains OIDs - Object Identifiers
    - Poll devices over udp/161
- Request statistics from a device
    - Server, firewall, workstation, switch, router, etc.
- Poll devices at fixed intervals create historical performance graphs
- SNMP traps
    - Most SNMP operations expect a poll
    - SNMP traps can be configured on the monitored device, and communicated over udp/162
    - It sets a threshold for alerts

![Here is an example of a vulnerability scan display while working. This is generally easy to understand. ](Screenshot_from_2025-06-18_12-30-52.png)

Here is an example of a vulnerability scan display while working. This is generally easy to understand. 

## **Firewalls - CompTIA Security+ SY0-701 - 4.5**

*This is a huge rerun learn session of what should already be known*

### Next Generation Firewalls (NGFW)

- The OSI Application Layer - Layer 7 Firewall
- Can be called different names
    - Application layer gateway
    - Stateful multilayer inspection
    - Deep packet inspection
- Requires some advanced decodes
    - Every packet much be analyzed, categorized, and a security decisions determined

### Ports and Protocols

- Make forwarding decisions based on protocol (TCP or UDP) and port number
    - Traditional port-based firewalls
    - Add to an NGFW for additional security policy options

![Here is a display of a Firewalls configuration. ](Screenshot_from_2025-06-18_14-43-35.png)

Here is a display of a Firewalls configuration. 

### Firewalls rules

- They are usually listed from top-to-bottom, with more specific rules being near the top
- Most firewalls include a deny at the bottom even if you don't put one so that if it doesn't follow one of the rules above in the list, it is automatically denied to enter

### Screened subnet

- An additional layer of security between the you and the internet
    - Public access to public resources
    - Private data remains inaccessible

### IPS rules

- Intrusion Detection System
    - Usually integrated into a NGFW
- Different ways to find malicious traffic
    - Look at traffic as it passes by
- Signiture-based
    - Look for a perfect match
- Anomaly-based
    - Build a baseline of whats “normal”
    - Unusual traffic patterns are flagged
- You determine what happens when unwanted traffic appears
    - Block, allow, send an alert, etc.
- Thousands of rules or more
- Rules can be customized by group, or as individuals
- This can take time to find the right balance
    - security/alert “noise”/false positives

## **Web Filtering - CompTIA Security+ SY0-701 - 4.5**

### Content filtering

- Content filtering is the control of traffic based on data within the content
- Corporate control of outbound and inbound data like sensitive materials
- Control of inappropriate content
    - Examples of this would be things like Not safe for Work (NSFW) or Parental controls
    - This also helps by blocking bad sites like ones known for viruses and malware

### URL scanning

- This is simply put, when you allow, or deny access to certian Uniform Resource Locations (URLs)
- URLs are categorized, whicch means some certian ways of blocking URLs is simple, ut this could also lead to manua work that could be very tedious
- This may have limited control as URs arent the only wat to surf the internet
- Because their normally integrated into a NGFW, it could be limited to being set by a singular device

### Agent based

- These are restrictions that are downloaded onto users device directly so that it doesnt have to be under a spesfic firewall or anything like that so that it can be under the content filtering

### Proxies

- These sit between the users and the external network
    - Its like a communication that tals for you and makes requests in your name to grant you access to the network
- Proxy servers can be limited to things like IP addresses
- Applications may need to know how to use the proxy (explicit)
- A forward proxyonly sends nformation back to you after making sure the thing your tryiing to access is safe

### DNS filtering

- Before connecting t a website, get the IP adress
    - Perform a DNS lookup
- DNS is updated with real-time threat intelegence
    - Both connercial and public lists
- Harmful sites are not resolved
    - No IP adress, no connection
- This works for any DNS lookup, not just web filtering

## **Operating System Security - CompTIA Security+ SY0-701 - 4.5**

### Active directory

- A data base of everything on the network
    - Computers, user accounts, file shares, printers, groups, and more
    - Primarily Windows based
- Manage authentication where users login using their AD credentials
- Centralized access control
    - This determines users can access resources

- Commonly used by the help desk
    - Reset passwords, add and remove accounts

### Group Policy

- Manage the computers or users with group policies
    - Local and Domain policies
    - Group Policy Management Editor
- A central console
    - Login scripts
    - Network configurations (QoS)
    - Security parameters
- Comprehensive control
    - Hundreds of configuration options

Security-Enhanced Linux (SELinux)

- Security patches for the Linux kernel
    - Adds mandatory access control (MAC) to Linux
    - Linux traditionaly uses Discretionary Access Control (DAC)
- Limits application access
    - Least privledge
    - A potential breach will have a limited scope
- Open source
    - Already included as an option with many linux distributions

## **Secure Protocols - CompTIA Security+ SY0-701 - 4.5**

### Unencrypted network data

- Network traffic is important data, hence, everything should be highly protected
- Some protocols arent protected
    - All trafic sent in the clear
    - Telnet, FTP, SMTP, IMAP
- Verify with packet capture which helps you veiw everything sent ovr the network

### Protocol selection

- Use a secure application protocol WITH built in encryption
- A secure protocol may not be avalible, which is almost always a deal breaker

### Port selection

- secure and insecure application connections may be avalible
    - Its common to run secure and insecure on different ports
- HTTP and HTTPS
    - In-the-clear and encrypted web browsing
    - HTTP: Port 80
    - HTTPS: Port 443
- The port number does not garuntee secureity
    - Confirm the security features are enabled
    - Packer captures may be necessary

### Transport data

- Dont rely on the application
    - Encrypt everything over the current network transport
- 802.11 Wireless
    - Open acess point: No transport-level encryption
    - WPA3: All user data is encrypted
- Virtual Private Network (VPN)
    - Create an encrypted tunnel
    - All traffic is encrypted and protected
    - Often requires third-party services and software

## **Email Security - CompTIA Security+ SY0-701 - 4.5**

### Email security chalenges

- The protocols used to transfer emails include relatively few security checks
    - Its very easy to spoof an email
- Spoofing happens all the time
    - This means the name on the email isnt always who acctually sent the email
- While emails may LOOK like their sent from a cetian source, you have to be sure

### Mail gateways

- This is basically a gateway that allows or doesnt allow traffic to make it to your email
    - It evaluates the source of inbound emails
    - Blocks it at the gateway before it reaches the user
    - On-site or cloud-based
- These are similar to the email services used in school to keep users within the system safe

### Sender Policy Framework (SPF)

- SPF protocol
    - Sender configures a list of all servers authorized to send emails for a domain
- List of authorized mail servers are aded to a DNS TXT record
    - Receiving mail servers perform a check to see if incoming mail really did come from an authorized host
- Simply put, this just lets you keep track and authorize people to send emails on behalf of your company or as a person. This can be verified with a digital signiture or domain keys like Domain Keys Identified Mail (DKIM).

### DMARC

- Domain-based Message Authentication, reporting, and Conformance (DMARC)
    - An extension of SPF and DKIM
    - Here is also a DNS TXT record that decides what should happen to all emails that are received
- Compliance reports are sent to the emial administratos
    - the domain owner can see how many emails are received

![Here is what DMARC reports generally look like when veiwing them. ](Screenshot_from_2025-06-19_14-52-07.png)

Here is what DMARC reports generally look like when veiwing them. 

![Heres an example of how adding a DMARC TXT record works. ](Screenshot_from_2025-06-19_14-53-01.png)

Heres an example of how adding a DMARC TXT record works. 

## **Monitoring Data - CompTIA Security+ SY0-701 - 4.5**

### File Intergrity Monitoring (FIM)

- Some files change all the time
    - Some files should NEVER change
- Monitor important operating system application files and identify when changes occor
- Windows - SFC (System File checker)
- Linux - Tripwire
- Many different host-based IPS options

Data loss prevention (DLP)

- This find sensitive data on your network moving, and stop the traffic in real time
- This stops “leakage” of confidential information
- DLP systems
    - On your computer
        - Data in use
        - Endpoint DLP
    - On your network
        - Data in motion
    - On your server
        - Data at rest

### USB blocking

- DLP on a workstation
    - Allow or deny certian tasks

### Cloud-based DLP

- Located between users and the internet
    - Watch every byte  of network traffic
    - No hardware, no software
- Block custon defined data strings
    - Unique data for your orginization
- Manage acess to URLs
    - Prevent file transfers to cloud storage
- Block viruses and malware
    - Anything traversing the network

### DLP and Email

- Email continues to be the most critical risk vector
    - Inbound threats, outboung data loss
- Check every email inbound and outbound
- Inbound
    - Block keywords, identify importsers, quarintine email messages
- Outbound
    - Fake wire transfers, W-2 transmissions, employee information

<aside>
💡

One BIG thing to watch out for, would be emailing spreadsheet information. Excel spreadsheets can run code for automation, which means it could theoretically automatically steal and hide data from you on your computer in hidden columns.

</aside>

## **Endpoint Security - CompTIA Security+ SY0-701 - 4.5**

### Endpoint

- This is the end of traffic
- Stop the attackers from inbound, and outboung attacks
- Many differnt platforms
    - Mobile
    - Desktop
- Protection is multi-facteted
    - Defense in depth

### Edge vs. access control

- Control at the edge
    - Your internet link
    - Managed primarily through fiewall rules
    - Firewal rules rarely change
- Access control
    - Control from wherever you are; Inside or outside
    - Access can be based on many rules
        - This could be by user, group, location, application, etc
    - Access can be easily revoked or changed
        - Change your security posture at any time

### Posture assesment

- This is practically a full check on all devices to make sure everythings up to date including applications and software
- This is known as a form of health check
    - Here are some serious health and posture assesment notes
        - Persistent agents
            - Permanetly installed onto a system
            - Periodic updates may be required
        - Dissolvable agents
            - No installation is required
            - Runs during the posture assesment
            - Terminates when no longer required
        - Agentless NAC
            - Integrated with Active directory
            - Checks are made during login and logoff
            - Cant be scheduled
- Ask yourself these questions…
    - Is it a trusted device?
    - Is it running a anti-virus? Which one? Is it updated?
    - Are the corporate applications installed?
    - Is it a mobile device? Is the disk encrypted?
    - The type of device doesnt matter - Windows, Mac, Linus, iOS, Android

### Failing your assesment

- While it may be obvious, it must be noted that is a device fails a posture assesment, its up to you or the person in charge to decide if its needing to be fixed or discarded. This means it should be quarintined, then fixed or discarded in whatever way neccesary. The goal ofcorse is to fix as many devices as possible without making a risk to the company.

### Endpoint detection and response (EDR)

- A different method of threat protection that can be scaled to meet the number of threats
- Detects threats, investigates them, and then responds to them in a way that is set.
    - This is usually done by quarintining the system, and rolling back to a previous config.
    - After judgeing the way it handles things, it shouldnt need direct human intervention to run.

### Extended Detection and Response (XDR)

- This is very lierally a better version of EDR
    - It improves missed detactions, false positives, and long investigation times and attacks are more than just the endpoint
- Add network-based decisions
    - Investigate and respond to network anomalies
- Correlateendpoit, network, and cloud data
    - Improves detction rates
    - Simplify security event investigations

## **Identity and Access Management - CompTIA Security+ SY0-701 - 4.6**

### Identity and Access Management (IAM)

- Identity lifecycle management
    - Every entity (human and non-human) gets a digital identity
    - Access control sets the privledges for these entities so they can only access whats neccecary
    - Authenticates them when they try to log in and then authorizes it
    - Identity governance
        - Track an entity’s resource access
        - May be a regulatory requirment
- This is simply the process used to access data from wherever needed
- Applications are avalible everywhere
    - Desktop, browser, mobile device, etc.
- Data can be located anywhere
    - Cloud storage, private data centers, etc
- Many different application users
- Give the right permissions to the right people at the right time
    - This prevents unauthorized access
    - Least privledge

### Provisioning/de-provicion user accounts

- This process starts as a user makes an account
- Provision and de-provision occors for certian events like hiring, transfers, job seperation and things like that
- You have to specify account details
- An important part of the IAM process
    - An initial part of the IAM process
    - Nobody gets Administrator access

### Identify proofing

- IAM conforms who you are, as you COULD be anyonw according to the system
- Resolution
    - Who the system thinks you are
- Validation
    - Gathering information from the user (password, security questions, etc)
- Verification/Attestation
    - Passport, in-person meeting, etc
    - Automated verification is also an option

Single sign-on (SSO)

- Provode credentials one time
    - This gives access to all avalible assigned resources
    - No additional authentication required
- Usually limited by time
    - A single authentication can work for 24 hours
    - Authenticate agian after the time
- The underlying authentication infrastructure must also support SSO, which means its not always an option

### Lightweight Directory Access Protocol (LDAP)

- Protocol for reading and writing directories over an IP network
- X.500 specification was written by the International Telecumunications Union (ITU)
- DAP ran on the OSI protocol stack (its lightweight)

### Security Assertion Markup Language (SAML)

- Open standard for authentication and authorization
    - You can authenticate through a third party to gain access
    - One standard does it all, sort of
- Not orginically designed for mobile apps, which is SAML’s ;argest roadblock

### OAuth

- OAuth is a authorization framework that detemines what resources a user would be able to access
- Created by Google, Twitter, and many others which makes it a significant industry support
- No an authentication protocol
    - OpenID connect handles the single sign-on authentication
    - OAuth provides authorization between applications

### Federation

- Provide network access to others
    - Not just employees - Partners, suppliers, customers, etc.
    - Provides SSO and more
- Third-parties can establish a federated network
    - Authenticate and authorize between the two organizations
    - Login with your Facebook credentials

Interoperability

- Many different ways to communicate with an authentication server
    - More than just a simple login process
- Often determined by what is at hand
    - VPN concentrator can talk to a LDAP server
    - We have an LDAP server
- A new app uses OAuth
    - Need to allow authentication API access
- The inoperability is dependent on the enviornment
    - This is often part of a much larger IAM strategy

## **Access Controls - CompTIA Security+ SY0-701 - 4.6**

This is a unit revwied here before, so expect oversimplification in notes.

### Access control

- Once someone authenticates to a network, we still need to provide them with access to the resources they need to be able to preform their job function. This process is called access control.
- There are alot of access control models, and different orginizations could use any one of these

### Least privledge

- You just give them enough permissions to be able to do their job
- This also means you dont give anyone administrator access

### Mandatory Access Control (MAC)

- The opertating system limits the operation on an object based on security clearance levels
- Every object gets a label
    - Confidential, secret, top secret, etc
- Labeling of objects uses predefined rules, which are set by adminiistrator

### Discretionary Access Control (DAC)

- This is when the creator of the data, decides who can access the data, and at what level
- An example of this would be if you made a spreadsheet personally to use at work, you could share it with your team and boss, but decide for yourself if the other departments should have access to that or not as you were the maker not the company.

### Role-based Access Control (RBAC)

- You have a role in your orginization
    - Manager, director, team lead, project manager
- Administrators provide access based on role of the user
- On Windows, this is called “Groups”

### Rule-based access controls

- Generic term for following rules
- Access is determined through system-enforced rules

### Attribute-based access control (ABAC)

- This is an authorization model that requires many forms of data that leads to giving you access to data
- Things that this could be limited to is the IP adress of your device, the time of day, desired action, relationship to the data, etc.
- Think of this as a “next generation” authorization model

## **Multifactor Authentication - CompTIA Security+ SY0-701 - 4.6**

### Multifactor authentication

- Prove who you are
    - Use different methods
    - A memorized passsword
    - A mobile app
    - Your GPS location
- Authentication Factors
    - Something you know
        - Something personal like a PIN (Personal Identification Number)
        - Phone password
    - Something you have
        - An ID or Smart card
        - A USB security key
        - A Hardware or Software token
        - Phone code through SMS
    - Something you are
        - Biometric authentication, iris scan, voice print
        - This is very difficult to change and is best used with multple forms of authentiction
    - Somewhere you are
        - GPS location
        - IP adress (thouh its not very accurate)
    - Etc.

## **Password Security - CompTIA Security+ SY0-701 - 4.6**

### Password complexity and length

- Make your passwod strng so that it cant be easily guessed or even brute forced
- Increase password entropy
    - No single words, no obvious passwords
    - Mix upper and lowercase letters, numbers, and special characters
- Stronger passwords are commonly atleast 8 characters
    - NOTE: This changes as brute force processing speeds get more efficient

### Password age and expiration

- Password age: How long since a password has been modified
- Password expiration
    - Password works for a certian amount of time, and after the date, it does not work

### Password managers

- Important to use different passwords for different accounts
- Password manager make saving passwords easy as it stores your passwords for you with one form of authentication to access them
- Their built into many operating systems and some browsers
- This is things like LastPass or Bitwarden

### Passwordless authnetication

- Many breaches come from use of poor password control, making the passwords more of a vulnerability than a safe authentication
- Passwordless authentication would be things that are very unreplicatbale like Face ID

### Just in time permissions

- In many orginizations, the IT team is assigned administrator/root elevated account rights, which would be a great account to attack
- This grants admin access for a limited time with no permanent administrator rights
    - This also stays within the principle of least privledge

## **Scripting and Automation - CompTIA Security+ SY0-701 - 4.7**

### **Scripting and Automation**

- Scripting and automation is how you use code to automate systems
    - This makes it so that things can be done one their own without your intervention
- They are very fast and useful as they work as fast as the device theyre run on

### Automation Benefits

- You save alot of ime as typing isnt required and it can be done over and over
- You can do tasks almost automatically and set it to do just about anything, and its with consistency
- It can be scaled securly which can be helpful for things like cloud security
- Employee retention
    - because the script can d boring tasks by itself, your attention can go elsewhere, lightening the workload
- High reaction time. Because the computer runs faster than you, it makes the process much more effieicnt.

### Cases for automation

- Automation can also be used to stop a human from making mistakes, this is caled a **Gaurdrail**.
- Security groups
    - Assign (or remove group access)
    - Constant audits
- Ticket creation
    - Automatically identify issues
    - Script email submissions into a ticket
- Esclation
    - Correct issues before involving a human
    - If issue isnt resolved, contect the on-call tech
- Controlling services and access
    - Automatically enable and disable services
    - No set and forget
- Contiguous integration and testing
    - Constant development and code updates
    - Securely test and deploy
- Integration and Application Programming Interfaces (APIs)
    - Interact with third-party devices and sevices
    - Cloud services, firewalls, operating systems
    - Talk their language

### Scripting considerations

- Complexity
    - many moving parts
    - All the parts have to move smoothly together
- Cost
    - It takes money to create the script
    - It takes money to implement the automation
- Single point of failure
    - What happen if the script stops working?
    - This could be a significant deal breaker
- Technical debt
    - Patching problems may push the isse down the road
    - Its going to be more expensive to fix later
- Ongoing supportability
    - The script works great today
    - The cript may not work great tommorow
    - Plan for changes and updates

## **Incident Response - CompTIA Security+ SY0-701 - 4.8**

### Security incidents

- As you know, these are things that are events where risks come to a system due to an outside threat. This could be things like
    - Phishing, where people send fake emails to bait you to clicking links with malware
    - DDoS, where bots are used to attack a system
    - Stolen information
    - Etc.

### NIST SP800-61

- National Institute of Standards and Technology
    - NIST special Publication 800-61 Revision 2
    - Computer Security Incident handling Guide
- The incident response lifecycle
    - Preperation
    - Detection and Analysis
    - Containment, Eradication, and Recovery
    - Post-incident Activity

### Preparing for an incident

- Communication methods
    - Phones and contact information
- Incident handling hardware and software
    - Laptopps, removable media, forensic software, digital cameras, etc
- Incident analysis resources
    - Documentation, network diagrams, baselines, critical file hash values
- Incident mitigation software
    - Clean OS and application images
    - Its good to have a baseline set for how to deal with alot of different types of incidents, so that when they eventually happen, you can quickly respond in a prepared and confident way

### Analysis

- An incident might occor in the future
    - This is your heads up
- Web server log
    - Vulnerability scanner in use
- Exploit announcement
    - Mothly Microsoft patch release, Adobe PDF software update
- Direct threats
    - A hacking group doesn’t like you
- An attack is underway
    - This could be shown through a intrusion detection system like when a uffer overflow is being attempted
    - Antivirus software detects malware
    - Host-based monitor detects a configuration change and constantly monitors system files
    - Network traffic flows deviate from the norm, so they require constant monitoring

### Isolation and containment

- Generally a bad idea to let things run their course
    - An incident can spread quickly
    - Its your fault at that point boviously
- Sandboxes
    - An isolated operating system
    - Run malware and analyze the results
    - clean out sandbox when done
- Isolation can be sometimes be problematic
    - Malware or infections can monitor connectivity
    - When connectivity is lost, everything could be deleted/encrypted/damaged

### Recovery after an incident

- Get things back to normal
    - Remove the bad, keep the good
- Eradicate the bug
    - remove the malware
    - Disable breached user accouts
    - Fix vulnerabilities
- Recover the system
    - Restore from backups
    - Rebuild from scratch
    - Replace compromised files
    - Tighten down the perimeter

### Things to note

- Try and find out what REALLY happened that led to the incident
- Ask yourself, “How well was our planning?”
    - Try and find out ow you could improve your methoding and what could be done differently next time an incident like that happens agian
- Always be sure to have a post-incident meeting

## **Incident Planning - CompTIA Security+ SY0-701 - 4.8**

### Excercising

- This is how you test yourself before an acctual event
    - Scheduled update sessions (annual, semi-annual, etc)
- Use well defined rule of engagement
- Very spesific scenario, with limited time to run an event
- Evaluate response where you document and discuss

### Tabletop excercises

- Performing a full scale disaster drill can be costly and time consuming so a tabletop event is a downscaled version of that
- Many of the logistics can be determined through analysis
    - You dont physically have to go through a disaster or drill
- This is very literally you and your team sitting at a table together and making a hypothetical situation and discussingw hat you would do if that hypothetical were to really happen

### Simulation

- This is a… well… a simulated event in a controled enviornment like a virtual machine
    - You could do anything like a phishing attack, password requests, data breaches, etc

### Phishing simulation

- This is when someone in your orginization sends a phishing email to see who woul click on it, and reports back to the person who clicked on it
- This is good to test many things like finding out who clicked, how the protections systems are running, how your anti-virus and firewalls restrictions are running, and many more things

### Root cause analysis

- The main thing you wanna deduce after a incident is, why?
    - Why did they attack, was there a goal in mind or was it simply to make money somehow
    - Why did your system not defend to a better extent
    - etc
- Set conclusions to what couldve happened regarding the incident while backing them with facts
- **Mistakes happen, the response to the mistake is what makes the difference**

## **Digital Forensics - CompTIA Security+ SY0-701 - 4.8**

### Digital forensics

- Collect and protect informtion relating to an intrusion
    - Many different data sources and protection mechanisms
- RFC 3227 - Guidelines for Evidence Collection and Archiving
    - A good set of best practices
    - For the Security+ Exam, you dont need to know details of this
- Standard digital forensic process
    - Acquisition, analysis, and reporting
- data collection is imrpotant to track as it could be used in legal procedings one day

### Legal hold

- A legal technique to perserve relevant information
    - Prepare for impending litigation
    - Intended by legal councel
- Hold notification
    - Custodians are instructed to perserve data
- Seperate repository for electronically stored information (ESI)
    - Many different data sources and types
    - Unique workflow and retention requirements

### Chain of custody

- One important thing to note is that the information has to maintain its prestine or unmodified form while its in analysis
- Control evidence to maintain integrity
- Everyone who contacts the evidence
    - Use hashes and digital signitures to avoid tampering
- Label and catalog everything so that its easy to refer back to

### Acquisition

- Obtain the data from where it was (Disk, RAM, firmware, OS files, etc.)
- Some of the data may not have been on a single system
- For virtual systems, get a snapshot

### Reports

- When aquiring data, you also have to save information saying HOW the information was aquired, along with how it was stored
- Detailed explination of data aquisition and a step-by-step method of the process
- The findings and an analysis of the data is important to have, usually leading to a conclusion of the event

### Preservation

- Handing evidence
    - Isolate and protect the data
    - Analyze the data later without any alterations
    - Make backups
- Manage the collection process
    - Work from copies
    - Manage the data colection
- Live connection has become an important skill
    - Data may be encrypted or difficult to colect after powering down
- Follow best practices to ensure admissibility of data in court

## **Log Data - CompTIA Security+ SY0-701 - 4.9**

### Security log files

- These are detailed securiity-related information
    - Blocked and allowed traffic flows
    - Exploit attempts
    - Blocked URL categories
    - DNS Sinkhole traffic
- They also display security information
    - Documentation of every traffic flow
    - Summary of attack info
    - Correlate with other logs

### Firewall logs

- Traffic flows through the firewall
    - This will show you all information about the networks traffic through that port
    - NGFW’s have much more data that can come as logs for documentation

### Application logs

- These logs are spesific to the application their coming from, so they differ greatly
- Windows
    - Event veiwer / Application log
- Linux / macOS
    - /var/log
- Parse the log details on the SIEM
    - Filter out unneeded info

### Endpoint logs

- Attackers often gain access to endpoints
    - Phones, laptops, tablets, desktops, server, etc.
- Theres alot of data on the endpoint
    - Logon events, policy changes, system events, processes, account management, directory services, directory services, etc.
- Everything rolls up to the SIEM
    - Security Information and Event Manager
- Use with correlation of security events
    - combine IPS events with endpoints status

### IPS/IDS logs

- Intrusion prevention system / intrusion detection system
- These are usually integrated into a NGFW
- Logs contail information about predefined vulnerabilities known as OS vulnerabilities, generic security events
- Common data points
    - Timestamp
    - Type or class of attack
    - Source and destination IP
    - Source and destination port

### Network logs

- Switches, routers, access points, VPN concentrators, and other infrastructure devices
- Network changes
    - Routing updates
    - Authentication issues
    - Network security issues

Metadata

- Data that describes other data sources
- Email
    - Header details, sending servers, destination adress
- Mobile
    - Type of phone, GPS location
- Web
    - Operating system, browser type, IP adress
- Files
    - Name, adress, phone number, title

Vulnerability scans

- Lack of security controls
    - No firewall
    - No anti-virus
    - No anti-spyware
- Misconfigurations
    - Open shares
    - Guest access
- Real vulnerabilities
    - Especially newer ones
    - Occationally old ones

<aside>
💡

Others may include…

**Automated reports**, which need to be spesified what to look for, for max capabilities.

**Dashboards**, which give real time status information, in a quick way all in one place

**Packet captures**, This is direcly looking at the system itself. nown for use through wireshark. 

</aside>