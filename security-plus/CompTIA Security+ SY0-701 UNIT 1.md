## **Security Controls – CompTIA Security+ SY0-701 – 1.1**

### Control categories

Technical controls

- Controls implemented using systems
- Operating system controls
- Firewalls, antivirus

Managerial controls

- Administrative controls associated with security design and implementation
- Security policies, standard operating procedures

Operational controls 

- Controls implemented by people instead of systems
- Security guards, awareness programs

Physical controls (pretty obvious)

- Limit physical access
- Guard shack
- Fences, locks
- Badge readers

## Control Types

### Preventative control types

- Preventative
    - Block access to a resource
    - YOU SHALL NOT PAAASSSSSSSSSSSS!!!!! (in Messers words himself (love this guy))
- Prevent access
    - firewall rules
    - follow security policy
    - “Guard shack checks all identification” from his examples
    - Enable door locks

<aside>
💡

One good way to memorize what category is which, try and name random things and categorize them yourself. *Remember to put a picture of the examples at the end of the video lesson*

</aside>

### Deterrent control types

- Deterrent
    - Discourages intrusion attempt
    - Does not directly prevent access
- Make an attacker think twice
    - Application of splash screens
    - Threat of demotion
    - Front reception desk
    - Posted warning signs

### Detective control type

- Detective
    - Identify and log an intrusion attempt
    - May not prevent access
- Find the issue- Directive
    - Collect and review system logs
    - Review login reports
    - Regularly patrol the property
    - Enable motion sensors

### Corrective

- Corrective
    - Apply a control after an event as been detected
    - Reverse the impact of an event
    - Continue operating with minimal downtime
- Correct the problem
    - Restoring backups can mitigate a ransomware infection
    - Create policies for reporting security issues
    - Contact law enforcement to manage criminal activity
    - Use a fire extinguisher

### Compensating control types

- Compensating
    - control using other means
    - Existing controls aren't sufficient
    - May be temporary
- Prevent the exploitation of a weakness
    - Firewall blocks a specific application instead of patching the app
    - Implement a separation of duties
    - Require simultaneous guard duties
    - Generator used after power outage

### Directive control types

- Directive
    - Direct a subject towards security compliance
    - A relatively weak security control
- Do this, please
    - Store all sensitive files in a protected folder
    - Create compliance policies and procedures
    - Train users on proper security policy
    - Post a sign for “Authorized Personnel Only”

![Screenshot from 2025-05-26 12-39-55.png](Screenshot_from_2025-05-26_12-39-55.png)

<aside>
💡

There are many different things that could go into each box, but these are just simple examples. 

</aside>

## **The CIA Triad – CompTIA Security+ SY0-701 – 1.2**

## The CIA Triad

### Combination of principles

- The fundamentals of security
- Sometimes referenced as the AIC Triad

<aside>
💡

The CIA triad has no relations to the governmental C.I.A.

</aside>

### **C**onfidentiality

- Prevent disclosure of information to unauthorized individuals or systems
- Certain information should only be known to certain people
- Encryption
    - Encode messages so only certain people can see/decode it
- Access controls
    - Selectively restrict access to a resource
- Two-factor authentication
    - Additional conformation before information is disclosed

### Integrity

- Messages can’t be modified without detection
- Data is stored and transferred as intended
    - Any modification to the data would be identified
- Hashing
    - Map data of an arbitrary length to data of a fixed length
- Digital signatures
    - Mathematical scheme to verify the integrity of data
- Certificates
    - Combine with a digital signature to verify an individual
- Non-repudiation
    - Provides proof of integrity, can be assorted to be genuine

### Availability

- Systems and networks must be up and running
- Information is accessible to authorized users
    - Always at your fingertips
- Redundancy
    - Build services that will always be available
- Fault tolerance
    - System will continue to run, even when a failure occurs
- Patching
    - Stability
    - Close security Holes

## **Non-repudiation - CompTIA Security+ SY0-701 - 1.2**

**Non-repudiation**: Non-repudiation provides proof of integrity and ensures that something can be verified as genuine. It's related to the integrity aspect of the CIA triad, which deals with ensuring data remains unmodified and verifiable.

### Non-Repudiation

- You can't deny what you've said
- Sign a contract
    - Your signature adds non-repudiation
    - You really did sign the contract
    - Others can see your signature
- Adds a different perspective for cryptography
    - Proof of integrity
    - Proof of origin, with high assurance of authenticity

### Proof of Integrity

- Verify data does not change
    - The data remains accurate and consistent
- In cryptography, we use a hash
    - Represent data as a short string of text
    - A message digest, a fingerprint
- If the data changes, the hash changes
    - If the person changes, you get a different fingerprint

**Hashing**: Hashing is a process that takes data and maps it to a fixed-length string of text that acts like a digital fingerprint. If someone changes the original data even slightly, this fingerprint would be completely different, making it useful for verifying that data hasn't been tampered with. If needing a better example, please look at Professor messers video for the unit at roughly 1:50 into the video.

### Proof of Origin

- Prove the message was not changed
    - Integrity
- Prove the source of the message
    - Authentication
- Make sure the signature isn't fake
    - Non-repudiation
- Sign with a private key
    - The message doesn't need to be encrypted
    - Nobody else can sign this (Certificate-based authenticationobviously)

## **Authentication, Authorization, and Accounting - CompTIA Security+ SY0-701 - 1.2**

### AAA framework

- Identification
    - This is who you claim to be
    - Usually your username
- Authentication
    - Prove who you say you are
    - password and other authentication factors
- Authorization
    - Based on your identification and authentication, “What access do you have?”
- Accounting
    - Resources used: Login time, data sent and received, logout time

### Authenticating systems

### Certificate-based authentication

- You have to manage many devices
    - Often devices you'll never physically see
- A system can’t type a pasword
    - And you may not want to store one

<aside>
💡

**How can you truly authenticate a device?**

- Put a digitally signed certificate on the device

Other buisnesses processes rely on the certificate:

- Access to the VPN from authorized devices
- Management software can validate the end device
</aside>

### Certificate Authentication

- An organization has a trusted Certificate Authority (CA)
    - Certificate-based authenticationMost organizations have their own CA’s
- The organization signs the certificate with the organization’s CA’s

### Authorization Models

- The user or device has now authenticated
    - To what do they now have access?
    - Time to apply an authorization model
- Users and services → Data and applications
    - Associating individual users to access rights does not scale
- Put an authorization model in the middle
    - Define by Roles, Organization, Attributes, etc.

### No authorization model (EX)

- A simple relationship
    - User → Resource
- Some issues with this method
    - Difficult to understand why an authorization may exist
    - Does not scale

<aside>
💡

Please refer to video example to understand context. 

</aside>

## **Gap Analysis - CompTIA Security+ SY0-701 - 1.2**

### Gap Analysis

- Where you are compared with where you want to be
    - The “gap” between the two
- This may require extensive research
    - There’s a lot to consider
- This can take weeks or months
    - An extensive study with numerous participants
    - Get ready for emails, data gathering, and technical research

### Choosing the framework

- Work towards a known baseline
    - This may be an internal set of goals
    - Some organizations should use formal standards
- Determine the end goal
    - NIST Special Publication 800-171 Revision 2, Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations
    - ISO/IEC 27001, Information security management systems

### Evaluate people and processes

- Get a baseline of employees
    - Formal experience
    - Current training
    - Knowledge of policies and procedures
- Examine the current processes
    - Research existing IT systems
    - Evaluate existing security policies

### Compare and contrast

- The comparission
    - Evaluate existing systems
- Identify weaknesses
    - Along with the most effective processes
- A detailed analysis
    - Examine broad security categories
    - Break those into smaller segments

### The analysis and report

- The final comparison
    - Detailed baseline objectives
    - A clear view of the current state
- Need a path to get from the current security to the goal
    - This will almost certainly include time, money, and lots of change control
- Time to create the gap analysis report
    - A formal description of the current state
    - Recommendations for meeting the baseline

## **Zero Trust - CompTIA Security+ SY0-701 - 1.2**

### Zero trust

- Many networks are relatively open on the inside
    - Once you’re through the firewall, there are few security controls
- Zero trust is a holistic approach to network security
    - Covers every device, every process, every person
- Everything must be verified
    - Nothing is inherently trusted
    - Multi-factor authentication, encryption, system permissions, additional firewalls, monitoring and analytics, etc.

### Planes of operation

- Split the network into functional planes
    - Applies to physical, virtual, and cloud components
- Data plane
    - Process the frames, packets, and network data
- Control plane
    - Manages the actions of the data plane
    - Define policies and rules
    - Determines how packets should be forwarded
    - Routing tables, NAT tables

### Extend the physical architecture

- Separate into functional tasks
    - Incorporate into hardware or software

### Controlling trust

- Adaptive identity
    - Considering the source and the requested resources
    - Multiple risk indicators - relationship to the orginization, physical location, type of connection, IP adresses, etc
    - Make and authentication stronger, if needed
- Threat scope reduction
    - Decrease the number of possible entry points
- Policy-driven access control
    - Combine the adaptive identity with a predefined set of rules

### Security zones (Where are they connecting from, and where are you trying to connect?)

- Security is more than a one-to-one relationship
    - Broad categorizations provide a security-related foundation
- Where are you coming from and where are you going
    - Trusted, untrusted
    - Internal network, external network
    - VPN 1, VPN 5, VPN 11
    - Marketing, IT, accounting, Human Resources
- Using the zones may be enough by itself to deny access
    - For example, **Untrusted** to **Trusted** zone traffic

Policy enforcement point

- Subjects and systems
    - End userd, applications, non-human entities

## **Physical Security - CompTIA SY0-701 Security+ - 1.2**

### Barricades/bollards

- Prevent access
    - There are limits to the prevention
- Channel people through a spesific acess point
    - And keep out other things
    - Allow people, prevent cars and trucks
- Identify saftey concerns
    - And prevent injuries
- Can be used to an extreme
    - Concrete barriers/bollards
    - Moats

### Access control vestibules

- All doors normally unlocked
    - Opening one door causes others to lock
- All doors normally locked
    - Unlocking one door prevents others from being unlocked
- One door open/other locked
    - When one is open, the other cannot be unlocked
- One at a time, controlled groups
    - Managed control through an area

### Fencing

- Build a perimeter
    - Usually very obvious
    - May not be what you’re looking for
- Transparent or opaque
    - See through the fence (or not)
- Robust
    - Difficult to cut the fence
- Prevent climbing
    - Razor wire
    - Build it high

### Video surveillance

- CCTV (Closed circut television)
    - Can replace physical gaurds
- Camera feautures are important
    - Motion recognition can alarm and alert when something moves
    - Object detection can identify a licence plate or face
- Often many different cameras
    - Networked together nd recorded over time

### Gaurds and access badges

- Security gaurd
    - Physical protection at the reception area or of a facility
    - Validates identification of existing employees
- Two-person integrity/control
    - Minimize exposure to an attack
    - No single person has access to a physical asset
- Access badge
    - Picture, name, other details
    - Must be worn at all times
    - Electronically logged

### Lighting

- More light means more security
    - Attackers avoid the light
    - Easier to see when lit
    - Non IR cameras see better
- Specialized design
    - Consider overall light levels
    - Lighting angles may be important
        - Important for facial recognition
    - Avoid shadows and glare

### Sensors

- Infrared
    - Detects radiation in both light
    - Common in motion detectors
- Pressure
    - Detects a change in force
    - Floor and windoow sensors
- Microwave
    - Detects movemen across lirge areas
- Ultrasonic
    - Send ultrasonic signals, receive reflected sound waves
    - Detect motion, collision detection, etc.

## **Deception and Disruption - CompTIA Security+SY0-701 - 1.2**

### Honeypots

- Attract the bad guys
    - And trap them there
- The “attacker” is probably a machine
    - Makes for interesting recon
- Honeypots
    - Create a virtual world to explore (to distract bots)
- Constant attle to discern the real from the fake

### Honeynets

- A real network includes more than a single device
    - Servers, workstations, routers, switches, firewalls
- Honeynets
    - Build a larger deception network with one or more honeypots
- More than one source of information
    - Stop spammers - https://projecthoneypot.org

Honeyfiles

- Attracts the attackers with more honey
    - Create files with fake information
    - Something bright and shiny
- Honeyfiles
    - Bait for the honeynet (passwords.txt)
    - Add many honeyfiles to file shares
- An alert is sent if the file is accesses
    - A virtual bear trap

### Honeytokens

- Track the malicious actors
    - Add some traceable data to the honeynet
    - If the data is stolen, youll know where it came from
- API credentials
    - Does not acctually provide access
    - Notifications are sent when used
- Fake email adresses
    - Add it to a contact list
    - Monitor the internet to see who posts it
- Many other honey tokens examples
    - database records, browser cookies, web page pixels

## **Change Management - CompTIA Security+ SY0-701 - 1.3**

### Change management

- How to make a change
    - Upgrade software, patch an application, change firewalla configuration, modify switch ports
- One of the most common risks in the enterprize
    - Occors very frequently
- Often overlooked or ignored
    - Did you feel that bits?
- Have clear policies
    - Frequency, duration, installation process, rollback procedures
- Sometimes extremely difficult to implement
    - Its hard to change corporate culture

### Change approval process

- A formal process for managing change
    - Avoid downtime, confusion, and mistakes
- A typical approval process
    - Complete the request forms
    - Determine the purpose of the change
    - Identify the scope of the change
    - Schedule a date and time of the change
    - Determine affected systems and the impact
    - Analyze the risk associated with the change
    - Get approval from the change control board
    - Get end-user acceptance after the change is complete

### Ownership

- An individual or entity needs to make a change
    - They dont own the process
    - They dont (usually) preform the acctual change
- The owner manages the process
    - Process updates are provided to the owner
    - Ensures the process is followed and accpetable
- Adress label printers needs to be upgraded
    - Shipping and receiving department owns the process
    - IT handles the actual change

Stakeholders

- Who is impacted by this change?
    - Theyll want to have input on the change management process
- This may not be as obvious as you think
    - A single change can include one individual or the entire company
- Upgrade software used for shipping labels
    - Shipping/receiving
    - Accounting reports
    - Product delivery timeframes
    - Revenue recognition - CEO visibility

### Impact analysis

- Determine a risk value
    - i.e., high, medium, low
- The risks can be a minor or farreaching
    - The “fix” doesnt acctually fix anything
    - The fix breaks something else
    - Operating system failures
    - Data corruption
- Whats the risk with NOT making the change?
    - Security vulnerability
    - Application unavalibility
    - Unexpected downtime to other services

### Test results

- Sandbox testing enviornment
    - No connection to the real world or productioin system
    - A technological safe space
- Use before making a change to production
    - Try the upgrde, aply the patch
    - Test and confirm before deployment
- Confirm the backout plan
    - Move everything back to the original
    - My sandbox cant consider every possibility

### Backout plan

- The change will work perfectly and nothing will ever go bad
    - Of course it will
- You should always have a way to revert your changes
    - Prepare for the worst, hope for the best
- This isnt as easy as it sounds
    - Some changes are difficult to revert
- Always have backups
    - Always have GOOD backups

### Maintenance window

- When is the change happening?
    - This might be the most difficult part of the process
- During the workday may not be the best option
    - Potential downtime woudl affect a large part of production
- Overnights are often a better choice
    - Challenging for a 24-hour production schedules
- The time of the year may be a consideration
    - Retail networks are frozen during the holiday season

<aside>
💡

Change management is CRITICAL, and should be well documented and well secured. There should also be checked standards that everyone should know that limit the controls people have on work devices. 

</aside>

## **Technical Change Management - CompTIA Security+ SY0-701 - 1.3**

### Technical change managment

- Put the change management process into action
    - Execute the plan
- There’s no such thing as a simple upgrade
    - Can have many moving parts
    - Seperate events may be required
- Change management is often concerned with “what” needs to change
    - The technical teamTechnical Change Management - CompTIA Security+ SY0-701 - 1.3 is connected with “how” to change it

### Allow list/deny list

- Any appliction can be dangerous
    - Vulnerabilities, trojan horses, malware
- Security policy can control app execution
    - Allow list, deny/block list
- Allow list
    - Nothing runs unless its approved
    - Very restrictive
- Deny list
    - Nothing on the “bad list” can be executed
    - Anti-virus, anti-malware

### Restricted activities

- The scope of a change is important
    - Defines exacly which components are covered
- A change approval isnt permission to make any change
    - The change control approval is very spesific
- The scope may need to be expanded during the change window
    - Its impossible to prepare for all possible outcomes

### Downtime

- Services will eventually be unavalible
    - The change process can be disruptive
    - Usually scheduled during non production hours
- If possible, prevent any downtime
    - Switch to secondary system, upgrade the primary, then switch back (seamlessly)
- Minimize any downtime events
    - The process should be as automated as poossible
    - Swith back to secondary if issues appear
    - Should be part of the backout plan
- Send emails and calender updates

### Restarts

- Its common to require a restart
    - Implement the new configuration
    - Reeboot the OS, power cycle the switch, bounce the service
    - Can the system recover from a power outage
- Services
    - Stop and restart the service or daemon
    - May take seconds or minutes
- Applications
    - Close the application completly
    - Launch a new application instance

### Legacy applications

- Some applications were here before you arrived
    - They’ll be here when you leave
- Often no longer suported by the developer
    - You’re now the support team
- Fear of the unknown
    - Face your fears and document the system
    - It may not be as bad as you think
- May be quirky
    - Create spesific processes and procedures

### Dependencies

- To complete A, you must first complete B
    - A service will not start without other actice services
    - An application requires a spesific library version
- Modifying one component may require changing or restarting other components
    - This can be challenging to manage
- Dependencies may occor across systems
    - Upgrade the firewall code first
    - Then upgrade the firewall management software

### Documentation

- It can be challenging to keep up with changes
    - Documentation can become outdated very quickly
    - require with the change management process
- Updating diagrams
    - Modifications to network configurations
    - Adress updates
- Updating policies/procedures
    - Adding new systems may require new procedures

### Version control

- Track changes to a file or configurtion data over time
    - Easily revert to a previous setting
- Many opportunities to manage versions
    - Router configurations
    - Window OS patches
    - Application registry entries
- Not always straightforward
    - Some devices and operating systems provide version control features
    - May require additional management software

Public Key Infrastructure - CompTIA Security+ Sy0-701 - 1.4

Public Key Infrastructure - CompTIA Security+ Sy0-701 - 1.4

## **Public Key Infrastructure - CompTIA Security+ Sy0-701 - 1.4**

### Public Key Infrastructure (PKI)

- Policies, procedures, hardware, software, people
    - Digital: create, distribute, manage, store, revoke
- This is a big, **big**, endeavor
    - Lots of planning
- Also refers to the binding of public keys to people or devices
    - The certificate authority
    - Its about trust

### Symmetric encryption

- A single, shared key
    - Encrypt with the key
    - Decrypt with the same key
    - If it gets out, youll need another key
- Secret key algorythm
    - A shared secret
- Doesnt scale very well
    - Can be challenging
- Very fast to use
    - Less overhead than asymetric encryption
    - Often combined with asymetric encryption

### Asymmetric encryption

- Public key cryptography
    - Two (or more) mathematically related keys
- Private key
    - Keep this private
    - One person/One device
- Public key
    - Anyone can see this key
    - Give it away
- The private key is the only key that can decrypt data encrypted with the public key
    - You cant derive the private key from the public key

### The key pair

- Asymetric encryption
    - Public key Cryptography
- Key generation
    - Build both the public and private key at the same time
    - Lots of randomization
    - Large prime numbers
    - Lots and lots of math
- Everyone can have the public key
    - Only one person can have the private key (as an example. Normally multiple people can have a private key with permission.)

<aside>
💡

If you have a public key with a private key pair, but only have the public—there is no way to decript or reverse enjineer the math for the private key without having it. The public key alone is not as useful. 

</aside>

### Key escrow

- Someone else holds your decryption keys
    - Your private keys are in the hands of a 3rd party
    - This may be within your own orginization
- This can be a legitamate buisness aranement
    - A buisness might need acess to employee information
    - Government agencies may need to decrypt partner data
- Controversial?
    - Of course
    - But may still be required

## **Encrypting Data - CompTIA Security+ SY0-701 - 1.4**

### Encrypting stored data

- Protect data on storage devices
    - SSD, hard drive, USB drive, cloud storeage, etc.
    - This is data at rest
- Full-disk and partition/volume encryption
    - Bitlocker, file vault
- File encryption
    - EFS (Encryption File System), third-party utilities

### Database encryption

- Protecting stored data
    - And the transmission of that data
- Transparent encryption
    - Encrypt all database information with a symetric key
- Record-level encryption
    - Encrypt individual columns
    - Use seperate symmeric keys for each column

### Transport encryption

- Protect data traversing the network
    - You’re probably doing this now
- Encrypting in te application
    - Browsers can communicate using HTTPS
- VPN (Virtual Private Network)
    - Encrypts all data transmitted over the network, regardless of the application
    - Client-based VPN using SSL/TLS
    - Site-to-site VPN using IPsec

### Encryption algorithms

- There are many, many different ways to encrypt data
    - The proper “formula” must be used during encryption and decryption
- Both sides decide on the algorythm before encrypting the data
    - The details are often hidden from the end user
- There are adventages and disadventages between algorithms
    - Security level, speed, complexity of implementation, etc.

<aside>
💡

For the acctual Comptia test, you dont have to know the names of different encryption algorythims or the details. All you must know about them is that two ways of translating them are very different. Remember you cant decrypt an algorithm without a key. 

</aside>

### Cryptographic keys

- There’s very little tat isnt nkown about the cryptographic process
    - The algorythim is usually a known entity
    - The only thing you dont know is the key (the main part)
- The key determines the output
    - Encrypted data
    - Hash value
    - Digital signature

### Key lengths

- Larger keys tend to be more secure
    - Prevent brute-force attacks
    - Attackers can try ever possible key combination
- Symetric encryption
    - 128-bit or larger symetric keys are common
    - These numbers get larger and larger as time goes on
- Asymmetric encryption
    - Complex calculations of prime numbers
    - Larger keys than symmetric encryption
    - Common to see key lengths of 3,072 bits or larger

### Key stretching

- A weak key is a weak key
    - By itself, its not very secure
- Make a weak key stronger by performing multiple processes
    - Hash a password. hash the hash of the password. And continue…
    - Key stretching, key strengthening
- Brute force attacks would require reversing each of those hashes
    - The attacker has to spend much more time, even though the key is small

## **Key Exchange - CompTIA Security+ SY0-701 - 1.4**

### Key exchange

- A logical challenge
    - How do you share an encryption key across an insecure medium without pysically transferring the key?
- Out-of-band key exchange
    - Dont sned the symmetric key over the internet
    - telephone, courier, in-person, etc.
- In-band key exchange
    - Its on the metwork
    - Protect the key with additional information
    - Use asymmetric encryption to deliver a symmetric key

### Real-time encryption/decryption

- There’s a need for fast security
    - Without compromising the security part
- Share a symmetric session key using asymmetric encryption
    - Client encrypts a random (symmetric) key with a server’s public key
    - The server decrypts this shared key and uses it to encrypt dataa
    - This is the session key

### Symmetric key from asymmetric keys

- Use public and private key cryptography to create a symettric key
    - “Math is powerful”

![Screenshot from 2025-05-28 15-57-46.png](Screenshot_from_2025-05-28_15-57-46.png)

<aside>
💡

***This needs reveiw***

Here is an example of how you can use two private keys to make two symetric keys. This is one way you can send a symetric key across a network.

</aside>

## **Encryption Technologies - CompTIA Security+ SY0-701 - 1.4**

### Trusted Platform Module (TPM)

- A specification for cryptocraphic functions
    - Cryptography hardware on a device
- Cryptographic processor
    - Random number generator, key generators
- Persistent memory
    - Unique keys burned in during manufacturing
- Versitile memory
    - Storeage keys, hardware configuration information
    - Securely store Bitlocker keys
- Password protected
    - No dictionary attacks

### Hardware Security Module (HSM)

- Used in large enviornments
    - Clusters, redundant power
    - Securely store thousands of cryptographic keys
- High-end cryptographic keys
    - Plug-in card or seperate hardware device
- Key backup
    - Secure storage in hardware
- Cryptographic accelerators
    - Offload that CPU overhead from other devices

### Key management system

- Services are everywhere
    - On-premises, cloud-based
    - Many different keys for many different services
- Manage all keys from a centralized manager
    - Often provided as third-party software
    - Seperate the encryption keys from the data
- All key management from one console
    - Create keys for a spesific service or cloud provider (SSL/TLS, SSH, etc.)
    - Associate keys with spesific users
    - Rotate keys on regular intervals
    - Log key use and important events

### Keeping data private

- Our data is located in many different places
    - Mobile phones, cloud, laptops, etc.
    - The most private data is often physically closest to use
- Attackers are always finding new techniques
    - Its a race to stay one step ahead
- Our data is changing constantly
    - How do we keep this data protected?

### Secure enclave

- A protected area for our secrets
    - Often implemented as a hardware processor
    - Isolated from the main processor
    - Many different technologies and names
- Provides extensive security features
    - Has its own boot ROM
    - Monitors the system boot process
    - True random number generator
    - Real-time memory encryption
    - Root cryptographic keys
    - Preforms AES encryption in hardware

---

From this point on, Im only writing the things that i dont already understand down. Proper notes rather than everything on screen. I plan to meet a time schedule and writing in the style of the previous notes was wasting alot of time. 

---

## **Obfuscation - CompTIA Security+ SY0-701 - 1.4**

### Obfuscation: The process of making something unclear

Steganography: Greek for “concealed writing”; hiding writing in an image

- The cover text: the container document or file
- Steganography isnt just hiding things in images, you can also leave dots on paper that are translatable. The dots are known as machine identification codes.
- There is also audio stegonography and video stegonogrpahy.

Tokenization: Replacing sensitive data with a non-sensitive placeholder

- For example, paying with your phone is an example of this. Your phone creates a short term use token of your credit card data making it safe to send across the network to the card reader. This can be seen on recipts sometimes.

Data masking: Data obfusctaion; hiding some of the original data

- Example: SSN hiding ****-**-*999; same can be used for phone numbers or whatever neccesary. This is a common method of protecting PII (Personally identifyable information)

## **Hashing and Digital Signatures - CompTIA Security+ SY0-701 - 1.4**

### Hashes

- They represent data as a short string of text
    - A message digest, a fingerprint
- You use these to verify if a downloaded document is the same as the original
    - Integrity

### Collision

- You have to make sure your hashes are unique
- If you hash something, and it makes the same hash as another hash—thats called a collision
    - Collisions are incredibly rare and almost impossible, but you should be wary

**Salt**: Random information added to a password when hashing

- Salt is used to make a hash look different to someone who is trying to brute force
    - Salt example: dragon, dragon +eEr4K

### Digital signatures

- Proves that the message was not changed
    - Integrity
- Proves the source of the message
    - Authentication
- Makes sure the message isnt fake
    - Non-repudiation
- Sign in with private key
    - The message doesnt need to e encrypted
    - Nobody else can sign this (obviously)

<aside>
💡

When making a digital signiture, its usually as simple as clicking a checkbox that makes a digital signiture. Its used on many programs, and knowing the details of the process isnt nessecary (though it is useful). 

</aside>

## **Blockchain Technology - CompTIA Security+ SY0-701 - 1.4**

### Blockchain: a distributed ladger

- Keeps track of transactions
- Used for EVERYTHING that involves transations

## **Certificates - CompTIA Security+ SY0-701 - 1.4**

### Certificates

- A public certificate
    - Binds a public key witha digital signiture
    - Also holds other details about the holder
- A digital signiture adds trust

### Certificate details

- Serial number
- Version
- Signiture algorythim
- Issuer
- Name of cert holder
- Public key
- Extensions
- etc…

<aside>
💡

A certificate works exactly how you piture it to. Its a form of identification.

</aside>

### A Root of Trust

- This is a large factor that shos inherent trust through third parties

**Certificate Authority (CA)**: A trusted organization that issues and validates digital certificates. Think of it like an official identity verifier - they help establish trust by signing certificates that prove the authenticity of public keys and their holders.

- They are built into browsers (yes any browser)
- If its trusted on one browser, its trusted in any browser

If you have your own servers and private certificates that work only in an orginization then you have a **private certificate authoritiy.**