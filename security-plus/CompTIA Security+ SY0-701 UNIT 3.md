## **Cloud Infrastructures - CompTIA Security+ SY0-701 - 3.1**

### Cloud infrastructures

- Cloud infrastructures are simply the different ways you use cloud access in a company. Here are a few examples (don't stress it's really not that bad)
    - Infrastructure as a service (IaaS)
    - Platform as a service (PaaS)
    - Software as a service (SaaS)
    - Infrastructure as code
        - The code is treated as a mold that sets clouds parameters in a way that is transferable to other systems
        - It's treated as a large benefit (SO STUDY UP ON IT)
    - etc…
- Responsibility matrixes are used to show what services certain infrastructures do. These are usually given by cloud service providers.

### Hybrid considerations

- Cloud providers don't really work together, so if you want consistencies between different forms of clouds you need to do it manually
- For third party processes, you need to be sure they are always working as expected and make sure the information gets o the servers, as it is your responsibility (I think)

### Serverless architecture

- Function as a Service (FAAS)
    - This means your applications are separated into individual, autonomous functions, and it removes the operating system from the equation
- Serverless architecture saves time and money because it only runs when needed and not all the time constantly
- It runs in a stateless compute container, so the developer still creates the server-side logic
- It's managed by a third party

### Microservers and APIs

- This is usually done with **monolithic applications**, which means it's a single large application that does everything
    - Usually bad because it takes a lot of effort and time to keep up with such large programs
- Application Programming Interfaces (APIs) is treated as the “glue” for the microservices
    - They are scalable for whatever size project you need
    - Resilient and contains outages
    - Well secure and containment is built in

## **Network Infrastructure Concepts - CompTIA Security+ SY0-701 - 3.1**

### Physically isolation

- Be sure to physically isolate different devices so that they can't communicate, making them harder to access for hackers going for large scale systems
- Instead of making one server for every individual “customer”, you could use **Virtual Local Area Networks (VLANs)**. They make one system work as if they were two physically separate channels.
- Software Defined Networking (SDN)
    - This is broken into just about three parts.
        - Data
            - This is also known as the Infrastructure layer or the Data plane
            - It processes the network frames and packets, and pretty important to note, this is where encrypting happens
        - Control
            - Also known as the Control layer or Control plane
            - This layer manages the actions of the data plane
            - This gets information from point A, to point B
        - Management
            - Also known as the Application layer or Management plane
            - This plane configures and manages the device
            - SSH, browser, API

## **Other Infrastructure Concepts - CompTIA Security+ SY0-701 - 3.1**

### Attacks can happen anywhere

- One thing to note, is that many IT professionals would say the safest place for information to be left would either be on-premises or in the cloud. It differs between the two of them because they are better at different things
- **On-premises security**
    - Pros:
        - You can customize your security posture (full control when everything is in-house)
        - On-site IT team can manage security better
        - Local team maintains uptime availability
    - Cons:
        - a local team can be very expensive and difficult to staff
        - Security changes can take a lot of time

### Centralized vs. decentralized

- Most companies use decentralized information, meaning it's all stored in different places and is very hard to monitor for security
- Keep in mind centralized isn't perfect, so pick what's best for your conditions
- Virtualization
    - This helps you run many different operating systems on the same hardware
- Application containerization
    - This basically is just how you group information in a way that's easily accessible after understanding the grouping. Like a file cabinet.

![Here is a visual of how containerized and virtual systems would look to be used](Screenshot_from_2025-06-07_15-23-19.png)

Here is a visual of how containerized and virtual systems would look to be used

- Internet of things (IOT)
    - Sensors
    - Smart devices
    - wearable technology (like smartwatches or health monitors)
    - Facility automation
    - Just as a note: They usually have weak defaults and are very convenient to use. It only takes a single IOT device to get into a large system

SCADA / ICS

**Real-Time Operating System (RTOS)**: An operating system with a deterministic processing schedule

**Embedded systems**: Hardware and software deigned for a specific function

- Smartwatches
- Traffic light controllers
- Medical imaging systems

## **Infrastructure Considerations - CompTIA Security+ SY0-701 - 3.1**

### Availability

- Stay available as much as possible but only to the right people
- Resilience
    - “Eventually something will happen.”
    - Can you maintain availability?
    - Can you recover? How Quickly?
    - Mean Time to Repair (MTTR) - this is a term for the amount of time needed to repair systems

### Responsiveness

- Ask for things and get answers
- Try not to get too worried from delayed responses

### Scalability

- You only expand as much as you need because it costs money to do it and doing it too much would be a waste
- How quickly and easily can we increase or decrease capacity?

### Ease of deployment

- There are many parts in getting something working as it needs many things like the sever, database, cashing service, firewall, etc.
- This may be easy, but it isn't always. This can sometimes be done with automation.

### Risk Transference

- When your company doesn't want to risk something themselves, they may use risk transference so they can let a third party take care of the risk
- There is cybersecurity insurance
    - Attacks and downtime can be recovered
- Recovering internal losses
- Protect against legal issues from customers
    - Limit the costs associated with legal proceedings

### Ease of recovery

- Be as efficient as possible
    - Time is money
- Make procedures for specific events to fix issues as quick, and well as possible

### Inability to patch

- What if patching wasn't an option?
- Embedded systems
    - HVAC controls
    - Time clocks
- Not designed for end-user updates

### Power

- Most places have one source of power for a facility, bigger places have multiple
- Overall power requirements
    - Data center vs. office building
- Backup services
    - Uninterruptible Power Supply (UPS)
    - Generators

### Compute

- An applications heavy lifting
    - More than a single CPU
- In the cloud, it's usually referred to as a compute engine
- Maybe limited to a single processor

## **Secure Infrastructures - CompTIA Security+ SY0-701 - 3.2**

### Device placement

- Every network is different, but there are often similarities
- Firewalls separate trusted from untrusted and provide additional security checks
- Other services may require their own security technologies
    - Honeypots, Jump server, Load balancers, Sensors

Security zones

- Zone-based security technologies are more flexible and secure than IP address ranges
- Each area of the network is associated with a zone
    - Trusted, untrusted
    - Internal external
    - Inside, Internet, Servers, Databases, Screened
- This simplifies security policies. Here is an example as how.
    - It allows movement of data to look more like this
        - Trusted to Untrusted
        - Untrusted to Screened
        - Untrusted to Trusted

![Here is an example of how a system could be divided into different zones](Screenshot_from_2025-06-09_11-17-11.png)

Here is an example of how a system could be divided into different zones

### Connectivity

- Everything contributed to security
    - Including the network connection
- Secure network cabling and protect the physical drops
- Application-level encryption
    - The handwork has already been done
- Network level encryption
    - IPsec tunnels, VPN connections

## **Intrusion Prevention - CompTIA Security+ SY0-701 - 3.2**

### Intrusion Prevention System (IPS)

- IPS’s are made to watch the network traffic and protect the system by blocking traffic in vulnerable locations
- Intrusions include things like OS and application exploiting, buffer overflow, cross site scripting and other vulnerabilities
- **Detection vs. Prevention**
    - Intrusion Detection System (IDS), these simply find threats without doing anything to stop them
    - IPS stop the system from taking any serious damage
    - IPS are practically the better version of IDS

### Failure modes

- This simply discusses what happens when a system
- Fail-open
    - When a system fails, data continues to flow
    - This is a big plus in high availability needed areas
- Fail-closed
    - When a system fails, data does not flow

### Device connections

- Active monitoring
    - System is connecting to a line
    - Data can be blocked in real-time as it passes by
    - Intrusion prevention is commonly active
- Passive monitoring
    - A copy of the network traffic is examined using a tap or monitor
    - Data cannot be blocked in real time
    - Intrusion detection is commonly passive
- **In Active Monitoring**: The information goes first from the internet, to a fire wall, then through an IPS, with the core switch being the last thing in the setup. The switch isn't very useful in the process, but active monitoring has its advantages.
- In **Passive Monitoring**: Switches are used as in-between for traffic. They sit between one place and another so that when information is sent along the line the switch can copy the information, send the copy to an IPS, and send the original information to its normal location. This is good for identifying something in the system but is bad a stopping it as it still lets a copy through the system anyway.

## **Network Appliances - CompTIA Security+ SY0-701 - 3.2**

### Servers

- **Jump servers** are servers inside of a network that can be accessed from the outside. These are highly secured and are very important to watch.
- **Proxy servers** are meant to sit between two devices conversation and make requests on behalf of one of the users
    - If two people make the same request in a proxy server, even on different devices, will send the same copied result instead of the proxy needing to scower the internet again for the same answer. This saves a lot of time in the long run.
    - Proxies also alow URL filtering, limiting what sites can be reached
    - Two different proxies that are used are Expilicit proxies and Transparent proxies

### Proxies

- One of the simplest proxies are Network-Level Proxies; NAT
- Forward proxies are “internal proxies”
    - These are used to protect and control user acess to the internet
- Reverse proxies
    - Inbound traffic from the internat to your internal service
    - SIMILAR TO BEFORE: If two people make the same request in a proxy server, even on different devices, will send the same copied result instead of the proxy needing to scower the internet again for the same answer. This saves a lot of time in the long run.
- Open proxies
    - These are proxies that are run by third parties that we dont acctually know
    - These can cause significant security concern and are often used to circumvent existing security controls
    - One thing that the proxy owner could do is add malicious code, ads, or other things

Balancing the load

- Load balancers distribute information along multiple servers so that no one server is overworked
- Many servers are run with an Active/active load balancer
- Some that dont have Active/Active use Active/Passive load balancing

## **Port Security - CompTIA Security+ SY0-701 - 3.2**

### Port security

- This referes to security on the individual interfaces that are on a switch, or wireless access points
    - This is commonly seen in places that when you connect to wired, or wireless networks, and it asks for a username and password, that is an example of port security.
- Port security runs on Extensible Authentication Protocol (EAP), which is an authentication framework. This is a  transferable standard.
    - The most well known standard is IEEE 802.1X, which is a framework that prevents access to the network until authentication succeeds
- The parts of the IEE 802.1X and EAP
    - Supplicant - The client
    - Authenticator - The device that provides access
    - Authentication server - Validates the client credentials

## **Firewall Types - CompTIA Security+ SY0-701 - 3.2**

### The universaval security controls

- If you speak over the internet, your most likely communicating through a firewall
- Firewalls control the flow of traffic and protect closed systems from outside threats
- Anti-virus & Anti-malware

### Network-based firewalls

- Filter traffic by port number or application
    - OSI layer 4 vs OSI layer 7
    - Traditional VS NGFW firewalls
- Encrypt traffic
    - VPN between sites

### UTM / All-in-one security appliance

- Unified Threat Management (UTM) - also known as a web security gateway
    - URL filter/content inspection
    - Malware inspection
    - Spam filter
    - CSU/DSU
    - Router, Switch
    - Firewall
    - IDS/IPS
    - Bandwidth shper
    - VPN endpoint
- Keep in mind, these capabilities can only run at layer four The syste also cant hndle running all of these at once ll the time so it may only run a few before the device starts to slow down.

### The Next-generation firewall (NGFW)

- is the most common firewall
- Operates at layer seven
- They control traffic based on the application
- Also called other names
    - Application layer gateway
    - Stateful multilayer inspection
    - Deep packet inspection
- Their capable of checking everything that goes through the network and proforming a full packet decode of everything traversing those lanes
- It can work as a IPS
- Content filtering
    - You can block spesific sites or types of sites. EX: Any website catogorized as a gambling site or entertainment site

Web application firewall (WAF)

- Not a “nromal” firewall, because it applies to the rules of HTTP/HTTPS conversations
- It can allow or deny based on expected input
    - Unexpected input is a common method of exploiting an application

![Here is what a log file from a firewall would generally look like. (ignore the professor in the corner)](Screenshot_from_2025-06-10_14-14-12.png)

Here is what a log file from a firewall would generally look like. (ignore the professor in the corner)

## **Secure Communication - CompTIA Security+ SY0-701 - 3.2**

### VPNs

- Virtual Private Networks (VPNs): These are encrypted (private) data traversing a public network
- VPN concentrators are used as a middle ground between a corperate network and the internet so that it can hide information
- Encrypted tunnels
    - This is simply the path the VPN takes
    - It keeps your data safe and private online and encrypts it
    - The tunneling is basically when you put the original packet (IP header and data), and put it inside of alot more information like a new IP header, IPsec Headers, IPsec Trailers, etc. This hides your data by adding alot of unneccecary information for an interception to dig through to find important info (The IP header and data)
- For mobile devices an SSL/TLS VPN would be used (Secure Sockets Layer VPN)
    - There are (almost) no firewall issues!
    - No big VPN clients, so its usually remote access communication
    - They authenticate users, so there arent any requirements for digital certificates or shared passwords like IPsec
    - Can be run from a browser or from a (usually light) VPN client. Theses all apply across many operating systems.
    - These are commonly used from things like a laptop
- Site-to-site IPsec VPN
    - These are always on, basically. If not then its almost always on.
    - Firewalls often act as VPN concentrators
        - Probably already have firewalls in place

### Wide area networks

- Software Defined Networking in a Wide Area Network (SD-WAN)
    - Data center used to be in one place but the cloud changed everything
    - Cloud-based application communicate directly into the cloud
    - No need to hop through a central point

## **Data Types and Classifications - CompTIA Security+ SY0-701 - 3.3**

### Data types

- **Regulated**
    - managed by third party
    - Government laws and statutes
- **Trade secret**
    - An orginizations secret formulas
    - Often unique to an orginization
- **Intelectual property**
    - May be publicly visible
    - Copyright and trademark restrictions
- **Legal inforation**
    - Court records and documents
    - PII and other sensitive details
    - Usually stored in many different systems
- **Financial information**
    - Internal company financial details
    - Customer financials
    - Payment records
    - Credit cards data, bank records, etc.
- **Human readable data**
    - This is data that is simply stored in a way that can be read by a erson
    - Very clear and obvious
- **Non-human readbale data**
    - Not easily understood by humans
    - Encoded data
    - Barcodes
    - Images

<aside>
💡

Sensitive information should be a top priority in security.

</aside>

### Classifying sensitive data

- Not all data has the same level of categorization. EX: Licence tag numbers vs. Health records
- **Data classifications**
    - Proprietary
        - This is data that is the property of an orginization
        - May also include trade secrets
        - Often data unique to an orginization
    - PII - Personnaly Identifyable Information
        - Data that can be used to identify an individual
        - Name, date of birth, mothers maiden name, biometric information
    - PHI - Protected Health Information
        - Health information associated with an individual
        - Health status, health care records, payments for healthcare, and much more

## **States of Data - CompTIA Security+ SY0-701 - 3.3**

### Data at rest

- The data is on a storage device like a SSD, hard drive, flashdrive, etc.
- Encrypt the data
    - Whole disk cncryption
    - Database encryption
    - File- or folder-level encrytion
- Apply permissions
    - Access control lists
    - Only authorized users can access the data

### Data in transit (Data in motion)

- Data transmitted over the network
- Not much protection as it travels
    - Many different switches, routers, devices
- Network-based protection
    - Firewall, IPS
- Provide transport encryption
    - TLS (Transport Layer Security)
    - IPsec (Internet Protocol Security)

### Data in use

- Data that is activly processing in memory
    - System RAM, CPU registers and cache
- The data is almost alway decrypted
    - Otherwise, you couldnt do anything with it
- The attackers can pick he decry[ted information out of RAM
    - Very attractive option
    - Attackers will primarily go after data in use because if the data is in use, that means its information that is likely in a formated way thats easy to read like human readable data

### Data soverengnty

- This is information that is stored in another country, and its controled by the laws of that particular country
- Laws that may prohibit where data is stored
    - **GDPR (General Data Protection Regulation)**
    - Data collected on AU citizens must be stored in the EU
    - A complex mesh of technology and legalities

## **Protecting Data - CompTIA Security+ SY0-701 - 3.3**

### Geographic restrictions

- This refers to giving different permissions to people based on their physical locations.
- Location can be determined through geolocation.
- Geolocation - determining a user's location
    - GPS - mobile device, very accurate
    - 802.11 wireless, less accurate
    - IP address, not very accurate
- Geofencing
    - Automatically allow or restrict access when a user is in a particular location
    - Don't allow this app to run unless you're near the office

### Protecting data

- Ngl this is common sense so im gonna skip the stuff about protecting data in this video thats already been repeated alot
- Original form of info is called plaintext, ecrypted form is called ciphertext
- Hashing (not gonna repeat)
- Obfuscation (still, not gonna repeat)
- Masking: EX: (***) - **** - *234
- Tokenization (you get the point)
- Segmentation (do i really have to say it)

## **Resiliency - CompTIA Security+ SY0-701 - 3.4**

### High avalibility

- When a component  is replaced after a problem occors, it does not neccearealy mean the system will be up without elay. There is usually a amount of time needed to wait before the system can be up and running fine agian.
- High avalibility is also abreviated as (HA) sometimes
- Higher avalibility almost always means higher costs
    - Theres always another contengency you could add
    - Upgraded power, high quality sserver components, etc.

### Server clustering

- This is the combination of two or more servers
    - They appear as a single large server
    - Users would only see one device
- You could easily increase capacity and avalibility
- This is usually configured in the operating system
- Another similar method in doing things would be load balancing as seen before
    - This connects a bunch of systems in a way where they arent aware that the other devices are part of the same system, unlike server clustering
    - It balances a load across multiple server instead of one contiuous server

### Site resiliency

- Recovery site is prepped where the data is syncronized with the main servers
    - A **Hot Site** is one type of recovery site
        - A hot site is an exact replica of your main systems to the T
        - When you change something in the original server, you also make the same change to the hot site
        - The switch to flip your systems from the original to the hot site should be as simple as flipping a switch (or quite a few switches)
    - A **Cold Site** is another way of recovery
        - This is basically an empty building with no data
        - You must bring your data and people to run the site with you
        - This is just a free space to set up when its eventually needed
    - A **Warm Site** is a mix between the hot and cold sites
        - A warm site is where ther is space and a bt of equipment, but not enough so that you can transfer immedietly
        - Its just enough to get along
- One thing you must note is that your recovery site should be in a place far from your original site so that things such as weather cant be a factor in your systems not being up

### Platform diversity

- Vulnerabilities are problems that are solved when they are found
- Not all OS’s have the same vulnerabilities. With that in mind, be sure to have multiple types of OS’s on different devices so that one vulnerability is the cause of the whole systems fall.
- One good way to format would be Linux on the data centers and MacOS for the clients or vice versa
- You could also use multiple cloud providers as well so that your information isnt trapped in one location
- Continuity of operations planning (COOP): This is a type of failback measure when there isnt a recovery option service avalible as stated before. Examples of this would be things such as…
    - Paper recipts to replace digital ones
    - Manual transactions
    - Phone calls for transaction approval
    - Etc.

## **Capacity Planning - CompTIA Security+ SY0-701 - 3.4**

### Capacity plannig

- You only pay for what you need an no more
    - Extra space thats unused is simply wasting money, so make sure to keep up with what is needed, and only meet that requirement
- Having employees is apart of the service requirements
    - Too many employees
        - Redeploy to other parts of the orginization
        - Downsize (let people go)
    - Too few employees
        - Recruit new staff
        - It may be time consuming to add more staff

### Technology

- When first implementing a system, pay attention to things like changing size for demand
- Distribute load for web services acress multiple services
- Watch cloud providers for storage
- Infrastructure
    - The underlyinng framework
        - Application servers, network services, etc
        - CPU, network, storeage

## **Recovery Testing - CompTIA Security+ SY0-701 - 3.4**

### Recovery testing

- This is testing yourself and the industry for if an acctual event acctually happens
    - Use very spesific scenarios for practice
    - Use well defined rules of engagement
- **Tabletop excercise**: A tabletop exercise in cybersecurity is a simulated scenario where participants discuss their roles and responses to a cybersecurity incident. This collaborative format helps teams practice decision-making, communication, and coordination during a crisis, improving preparedness and response strategies without the need for a real attack.
- **Fail over test**: A failover test is when an organization tests their backup systems by deliberately switching from their main systems to their backup systems to make sure everything works correctly in case of a real emergency. It's like a fire drill, but for computer systems - you want to make sure your backup plan actually works before you really need it.
- Simulated events are also a good way to test things
    - One good simulation would be fake phishing attempts sent by the cybersecurity team to see if the employees need more training on cyber security practices
- Parellel processing is when you split a process through multiple (parrelell) CPUs

## **Backups - CompTIA Security+ SY0-701 - 3.4**

### Backups

- Obviously, backups are important and are used to save avalibility
- Some important things to consider is...
    - Total amount of data
    - Type of backup data
    - Backup media
    - Storage location
    - Bakkup and recovery software
    - Day of the week (The schedule of when backups should be planned for./Frequency)
- **On-site backups**
    - No internet link required
    - Data is immediatly valible
    - Geenerally less epensive than offside
- **Off-site Backups**
    - Transfer data over internet or WN link
    - Data is avalible after a disaster
    - Restoration can be proformed from anywhere
- Information thats stored can be encrypted, so make sure to consider that option whenever storing information
    - When transporting information, or keeping it somewhere like onsite, be sure to encrypt it
    - Always ask yourself, “What if someone DOES get a hold of this drive?”
- **Snapshots**
    - Snapshots are like incremental backups, and should usually be taken just about 24 hours
    - These are used for very fast recovery
- **Replication**
    - This is an ongoing, almost real time backup that keeps data syncronized in multiple locations
    - This could be used well for hot sites
- **Journaling**
    - **Journaling**: Refers to the process of recording events, actions, and changes within a system or network to provide a comprehensive log of activities. This practice is crucial for monitoring security incidents, maintaining compliance, and aiding forensic investigations if a breach occurs.
    - This is used for things like power outages

## **Power Resiliency - CompTIA Security+ SY0-701 - 3.4**

### Power resiliency

- Power is the one thing that can connect all devices no matte what individual differences they have
- We usually dont make our own power
    - Power is likely supplied by third parties
    - We cant control our power avalibility
- There are ways to mitigate power issues like short and long term power outages
    - **Uninteruptable Power Supply (UPS)**: This is a short-term backup power supply to combat things like blackouts, brownouts (drops in voltage), and surges (rises in voltage).
        - UPS types
            - Offline/Standby UPS
            - Line-interactive UPS
            - On-line/Double conversion UPS
        - These are temporary, and only last a certian amount of time. So be sure to make sure how long they will last and buy one that meets that capability
    - **Generators**: This is a long-term powr backup that is capable of powering an entire buiding
        - The generator takes time to turn on, so a UPS can be used as a middle ground until a generator can properly power your systems.