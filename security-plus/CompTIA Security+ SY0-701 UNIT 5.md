## **Security Policies - CompTIA Security+ SY0-701 - 5.1**

### Security policy guidelines

- What policies are you following to provide CIA?
    - Confidentiality, Integrity, and Availability
- High level strategies like data storage requirements and security event procedures
- Detailed security goals
    - This includes appropriate Wi-Fi usage, requirements for remote access
- Security policies answer the “what” and “why”
    - Technical security controls, the “how”

### Information security policies

- The big list of all security related policies
- Includes compliance requirements, which can be critical to an organization
- Detailed security procedures that determine what should be done when something happens

Acceptable use policies (AUP)

- This is exactly what it says, it is a policy that determines what the acceptable use of company assets is
- They cover many topics
    - Internet use, telephones, computers, mobile devices, etc
- Used by an organization to limit legal liability
    - If someone is dismissed, these are the well-documented reasons why

### Business continuity

- Not everything goes to plan, so always plan for situations that are outside the norm
    - This could be things like the loss of computers or other common technologies
- There need to be an alternative
    - Manual transactions
    - Paper receipts
    - Phone calls for transaction approvals
- There must also be documentation of the problems, and also documentation and testing of the fallbacks before the problem occurs
    - You can't rely on something that exists, but doesn't work

Disaster recovery plan

- If there is a disaster, IT should be ready
    - Part of the business continuity planning
    - Keep the organization up and running
- Disasters are many and varied
    - Natural disasters
    - Technology or system
    - Human created disasters
- A comprehensive plan has the following…
    - Recovery location
    - Data recovery method
    - Application restoration
    - IT team and employee availability

### Incident response roles

- Incident response team
    - Specialized group, trained and tested
- IT security management team
    - corporate support
- Compliance officers
    - Intricate knowledge of compliance rules
- Technical staff
    - This is like serious IT hardware guys (sorry, it's easier to picture than to explain)
- User community
    - They see everything

<aside>
💡

If you'd like to see what type of guide is used for incident handling, you could look at **NIST SP00-61**.

</aside>

Software development lifecycle (SDLC)

- Systems development life cycle
    - Or application development life cycle
- Many ways to get from an idea to app
    - And many moving parts
    - Customer requirements
    - Keep the process on schedule
    - Stay in budget
- There’s no “best way”
    - But it helps to have a framework
    - There are many options

![Here's an example of popular SDLCs. The one on the right is meant to be… well… agile. Quick and easy and meant for less serious issue. The waterfall method is used for more intricate issues as a slow method to do things. It is used in a way so the step NIST SP00-61 of solving a security issue can be broken into easier to follow steps, which greatly helps in following guides like the one given by NIST.](Screenshot_From_2025-06-25_12-11-40.png)

Here's an example of popular SDLCs. The one on the right is meant to be… well… agile. Quick and easy and meant for less serious issue. The waterfall method is used for more intricate issues as a slow method to do things. It is used in a way so the step NIST SP00-61 of solving a security issue can be broken into easier to follow steps, which greatly helps in following guides like the one given by NIST.

## **Security Standards - CompTIA Security+ SY0-701 - 5.1**

### Security standards

- This is a formal definition for security technologies and processes
    - Complete documentation reduces security risk
    - Everyone must understand the expectations
- These may be written in-house
- Many standards are already available
    - ISO (International Organization for Standardization)
    - NIST (National Institute of Standards and Technology)

### Passwords

- This is the most basic security standard
- Most companies have different standards of what may make a good password
- Define acceptable authentication methods
    - No local accounts, only LDAP to the AD database, etc.
- Create policies for secure password resets
    - Avoid unauthorized resets and access
- Other password policies
    - Password change frequency, secure password storage requirements, password manager options, etc.

### Access controls

- This is the policy determining how people can access data in the company
    - This could include what time is avalible, what clearance level, if it needs a sign-off by management, etc.
- Determine how a user gets access
    - Require privilege documentation
- Document how access may be removed
    - Security issue, expiration, contract renewals, etc.

### Physical security

- Rules and policies regarding physical security controls
    - Dors, building access, property security
- Granting physical access is different for employees and visitors
- Define specific physical security systems
    - Electronic door locks, ongoing monitoring, motion detection
- Additional security concerns may include things like mandatory escorts, offboarding, etc.

### Encryption

- Define specific standards for encrypting and securing data
    - All things cryptographic
    - Can include implementation standards
- Password storage
- Data encryption minimus
    - Algorithms for data in use, data in transit, data at rest
    - Will probably be different for each data state

## **Security Procedures - CompTIA Security+ SY0-701 - 5.1**

### Change management

- A formal process for managing change
    - Avoid downtime, confusion, and mistakes
- Nothing changes without the process
    - Determine the scope of the change
    - Analyze the risk associated with the change
    - Create a plan
    - Get end-user approval
    - Present the proposal to the change control board
    - have a **backout plan** if the change doesn't work
    - Document the changes

### Onboarding

- Bring a new person into the orginization
    - New hires or transfers
- IT agreements need to be signed
    - Maybe part of the employee handbook or a seperate AUP
- Create accounts
    - Associate the user with the proper groups and departments
- Provide required IT hardware
    - Laptops, tablets, etc.
    - Preconfigured and ready to go

### Offboarding

- “All good things come to an end.”
- This process should be pre-planned
- What happens to the hardware and data?
- Account information is usually deactivated, but not always deleted

### Playbooks

- Conditional steps to follow; a broad process
    - Investigate a data breach, recover from ransomware
- Step-by-step set of processes and procedures
    - A manual checklist
    - Can be used to create automated activities
- Often integrated with a SOAR platform
    - Security Orchestration, Automation, and Response
    - Integrate third-party tools and data sources
    - Make security teams more effective

### Monitoring and revision

- IT security is constantly changing
    - Processes and procedures also must change
- Update to security posture
    - Tighten change control, additional playbooks
- Change to an individual procedure
    - Update the playbooks, include additional checks
- New security concerns
    - Protect against emerging threats

### Governance structures

- Boards
    - A panel of specialists
    - Set the tasks or requirements for the committees
- Committees
    - Subject-matter experts
    - considers the input from a board
    - Determines next steps for a tops at hand
    - Presents the results to the board
- Government entities
    - A different kind of machine
    - Legal concerns, administrative requirements, political issues
    - Often open to the public
- Centralized/decentralized
    - The source of the process and procedures
    - Centralized governance is located in one location with a group of decision makers
    - Decentralized governance spreads the decision-making process around to other individuals or locations

## **Security Considerations - CompTIA Security+ SY0-701 - 5.1**

### Regulatory

- regulations are often mandated
    - Security processes are usually a foundational consideration
    - Logging, data storage, data protection, and retention
- Sarbanes-Oxley Act (SOX)
    - The Public Company Accounting Reform and Investor Protection Act of 2002
- The Health Insurance Probability and Accountability Act (HIPAA)
    - Extensive healthcare standards for storage, use, and transmission of healthcare information

### Legal

- the security team is often tasked with legal responsibilities
    - Reporting illegal activity
    - Holding data required for legal processing
- Security breach notifications
    - A legal requirement in many jurisdictions
- cloud computing can make this challenging
    - Data moves between jurisdictions without human intervention
    - The security team must now follow legal guidelines

### Industry

- the industry may require specific considerations
    - Every market is a bit different
- Electrical and public utilities
    - Isolated and protected system controls
- Medical
    - Highly secure data storage and access logs
- Data encryption and protection

### Geographical security

- Local/regional
    - City and state government records
    - Uptime and availability of end-user services
- National
    - federal governments and national defense
    - Multi-state organizations
    - State secrets remain safe

### Global

- large multinational companies
- Global financial markets
- Legal concerns will vary widely

## **Data Roles and Responsibilities - CompTIA Security+ SY0-701 - 5.1**

### Data responsibilities

- High-level data relationships
    - Organizational responsibilities, not always technical
- Data owner
    - Accountable for specific data, often a senior officer
    - VP of sales owns the customer relationship data
    - Treasurer owns the financial information

### Data roles

- Data controller
    - Manages the purposes and means by which personal data is processed
- Data processor
    - Processes data on behalf of the data controller
    - Often a third party or a different group
- Payroll controller and processor
    - Payroll department (data controller) defines payroll amounts and timeframes
    - Payroll company (data processor) processes payroll and stores employee information
- Data custodian/steward
    - Responsible for data accuracy, privacy, and security
- Works directly with the data
    - Ensures compliance with any applicable laws and standards
    - Manages the access rights to the data
    - Implements security controls

## **Risk Management - CompTIA Security+ SY0-701 - 5.2**

### Risk identification

- The only certainty is uncertain
    - Risk management helps to understand potential risks
    - Identify weaknesses before they become an issue
- An important part of any orginization because growth brings risk, and its useful to get ahead of any potential problems
- Risk managment
    - Manage potential risk
    - Qualify internal and external threats
    - Risk analysis helps plan for contingencies

### Performing a risk assesment

- There are many ways to do this and its determines by what company your at
- One-time assesment
    - The assesment may be a part of a one-time project
    - Company aquistition, new equipment instalation, unique new security threats, etc.
- Continuous assesments
    - May be apart of an existing process
    - Change control requires a risk assesment as part of the change

### Ad hoc assesments

- An orginization may not have a formal risk assesment process
    - Perform a risk assesment when the situation requires
- EX: CEO is back from a confrence and wants to know if the orginization is protected from a new attack type

### Recurring assesments

- Eveluation occors on standard intervals
- An internal asesment
    - Performed  every three months at the begining of a quarter
- A mandated risk assesment
    - Required by certian orginizations
    - Some legal requirements will mandate an assesment
    - PCI DSS requires annual risk assesment

## **Risk Analysis - CompTIA Security+ SY0-701 - 5.2**

### Qualitative risk assesment

- This is a way of identifying risk factors
- This is used usually in a graph that shows collors to show how high the risk is for certian things

### Quantitative risk assesment

- ARO (Annualized Rate of Occurrence)
    - How likely is it that a hurricane will hit? In Montana? In Florida?
- Asset value (AV)
    - The value of the asset to the orginization
    - Includes the cost of the asset, the effct on company sales, potential regulatory fines, etc
- SLE (Single Loss Expectancy)
    - What is the monetary loss if a single event occors?
    - Asset value (AV) x Exposure factor (EF)
    - Laptop stoen = $1,000 (AV) x 1.0 (EF) = $1,000 (SLE)

### Likelihood and probability

- Risk likelihood
    - A qualitative measurement of risk
    - Rare, possible, almost certian, etc
- Risk probability
    - A quanitative measurement of risk
    - A statistical measurement
    - Can be based on historical performance

## **Risk Management Strategies - CompTIA Security+ SY0-701 - 5.2**

### Risk management strategies

- Transfer risk
    - This gives the risk to a third party
    - This is like cybersecurity insurance
- Accept
    - A buisness decision; “We’ll take the risk!”
    - This is often the usual course
- Accept with exemption
    - A security policy or regulation cannot be followed
    - May be based on avalible security controls, size of the orginization, total assets, etc.
    - Exemption may need approval
- Accept with exception
    - Internal security policies are not applied
    - Monthly security updates must be applied within 3 clender days
    - The monthly updates cause a critical software package to crash
    - An exception is made to update timeframe
- Avoid
    - Stop participating in high-risk activities
    - This effecttivly removes the risk
- Mitigate
    - Decrease the risk level
    - Invest in security systems

### Risk reporting

- A formal document
    - Identifies risk
    - Detailed information for each risk
- Usually created for senior management
    - make decisions regarding resources, budgeting, additional security tasks
- Commonly includes critical and emerging risks
    - The most important considerations

## **Business Impact Analysis - CompTIA Security+ SY0-701 - 5.2**

### Recovery

- Recovery time objective (RTO)
    - get a system up and running quickly
    - Get back to a particular service level
    - You’re not up and running until the data base and web server are operational
- Recovery point objective (RPO)
    - How much data loss is acceptable?
    - Bring the system back online; how far back does the system go?
    - If the database is up, but only provides the last 12 months of data
- Mean time to repair (MTTR)
    - Average time required to fix an issue
    - This includes time spent diagnosing the problem
    - An important metric for determining the cost and time associated with unplanned outages
- Mean time between failures (MTBF)
    - The time between outages
    - Can be used as a prediction or calculated based on historical performance
    - Total uptime/number of breakdowns
    - Statistically plan for possible outages

## **Third-party Risk Assessment - CompTIA Security+ SY0-701 - 5.3**

### Third pary risk

- Every orginization works with vendors
    - Payroll, customer relationship management, email marketing, travel, raw materials
- Important company data is often shared
    - Categorize by vendor to manage risk
- Use contracts for clear understanding

Peneration testing

- Pentest: simulate an attack
- Similar to vulnerability scanning
- Often a compliance mandate

### Rules of engagement

- This is an mportant document
    - defines purpose and scope
    - makes everyone aware of test parameters
- Type of testing ans schedule
    - On site physical breach, internal test, external test
    - Normal work hours
- The rules
    - IP adress ranges
    - Emergency contacts
    - How to handle sensitive information
    - In-scope and out-of-scope devices or applications

### Right-to-audit clauses

- Common with buisness partners
    - Data sharing
    - Out sourcing
- Third-party providers
    - Can hold all of the data
    - Manage internet access
    - are they secure?
- Right-to-audit should be in contract

### Evidence of internal audits

- Evaluate the effectivness of security controls
    - Have a third-party perform an audit
- May be required for compliance
    - Its a good idea, even without industry standards
- Check for security controls and processes
    - access management, offboarding, password security, VPN controls, etc
    - Theres always an opportunity for improvment
- Perform at a reasonable frequency
    - A single audit isnt very helpful in the long-term

Supply chain analysis

- The system involved when creating a product
    - Involves orginizations, people, activites, and resources
- Suply chain analysis
    - Get a product or service from supplier to supplier
    - Evaluate coordination between groups
    - Identify areas of improvment
    - Access the IT systems supporting the operation
    - Document the buisness process changes
- Software update installs malware: March-June 2020

Vendor selection process

- Due dilligence
    - Check a company out before doing buisness
    - Investigate and verify information
    - financial status, pending or past legal issues, etc
    - Financial status, pending or past legal issues, etc
    - Background checks, personnel interveiws
- Conflict of interest
    - A personal interest could compromise judegemt
    - A potential partner also does buisness with your largest competitor
    - A third-party employs the brother of the CEO
    - A third-party offers gifts if a contract is signed
- Ongoing management of the vendor dealership
- Rveiws should occor on a daily basis
- Different vendors may be checked for different indicators
- Assign a person to be in chenge of the vendor relationship

## **Agreement Types - CompTIA Security+ SY0-701 - 5.3**

### Common agreements

- **Service Level Agreements (SLA)**
    - Minimum terms for service provided
    - Uptime, response time agreement, etc
    - Commonly used between customers and service providers
- Contract with an Internet provider
    - SLA is no more than four hous of unscheduled downtime
    - Technician will be dispached
- **Memorandum of Understanding (MOU)**
    - Both sides agree in general to the contents of the memorandum
    - Usually states common goals, but not much more
    - May include statements of confidentiality
    - Informal letter of intent; not a signed contract
- **Memorandum of agreement (MOA)**
    - The next step abouve a MOU
    - Both sides conditionally agree to the objectives
    - Can also be a legal document, even without a legal language
    - Unlike a contract, may not contain legally enforceable promises
- **Master Service agreement (MSA)**
    - Legal contract and agreement of terms
    - A broad framework to cover later transactions
    - many detailed negociations happen here
    - Future projects will be based on this agreement
- **Work order (WO) / Statement of Work (SOW)**
    - Spesific list of items to be completed
    - Used in conjunction with MSA
    - Details the scope of the job, location, deliverables schedule, acceptance criteria, and more
    - You use the SOW to refer to when you need to see if a job was done correctly
- **Buisness Partners Agreement (BPA)**
    - Going into buisness together
    - Owner stake
    - Financial contract
- Decision-making
    - Who makes the buisness decisions?
    - The BPA lists the spesific individuals and scope
- Prepare for contingencies
    - Financial issues
    - Disaster recovery

### Non-disclosure agreement (NDA)

- Confidentiality agreement between parties
    - Information in the agreement should not be disclosed
- Protects confidential information
    - Trade secrets
    - Buisness activities
    - Anything else listed in the NDA
- Unilateral or bilateral (or multilateral)
    - One-way NDA or mutual NDA
- Formal contract
    - Signitures usually required

## **Compliance - CompTIA Security+ SY0-701 - 5.4**

### Compliance

- **Compliance**: Meeting the standards of laws, policies, and regulations
- Rules
    - Many are industry-spesific or situational
    - They apply along many parts of buisness and life
- Penalties could include fines, loss of employment, or incarceration

### Compliance reporting

- Internal
    - Monitor and report on organizational compliance efforts
    - Large orginizations have a Central compliance Officer (CCO)
    - Also used to provide details to custom or potential investors
- External
    - Documentation required by external or industry regulators
    - May require annual or ongoing reporting
    - Missing or invalid reporting could result in fines and/or sanctions

### Regulatory compliance

- Sarbanes-Oxley Act (SOX)
    - The Public Company Accounting Reform and Investor Protection Act of 2002
- The Health Insurance Portability and Accountability Act (HIPPA)
    - Extensive healthcare standards for storage, use, and transmisssion of health care information
- The Gramm-Leach-Bliey Act of 1999 (GLBA)
    - Disclosure of privacy information from financial institutions

### HIPPA non-compliance fines and sanctions

- Fine of up to $50,000, or up to 1 year in prison, or both; (Class 6 Felony)
- Under false pretenses; a fine of up to $100,000, up to 5 years in prison, or both; (Class 5 Felony)
- Intent to sell, transfer, or use individually identifyable health information for commercial advantage, personal gain, or malicious harm, a fine up to $250,000, or up to 10 years in prison, or both; (Class 4 Felony)
- Civil fines; Maximum is $100 for each violation, with the total amount not to exceed $25,000 for all violations of an identical requirement or prohibition during a calender year; (Class 3 Felony)
- Other consequences may include…
    - Loss of licence
        - Significant economic sanction
        - Orginization cannot sell products
        - Others cannot purchase from a sanctioned company
        - May be expensive to re-licence
    - Contractual impacts
        - Some buisness deals may require a minimum compliance level
        - Without compliance, the contract may be in breach
        - May be resolved with or without a court of law

### Compliance monitoring

- Compliance monitoring: Ensure compliance in day-to-day operations
- Due diligence/care
    - A duty to act honestly and in good faith
    - Investigate to verify
    - Due care tends to refer to internal activities
    - Due duligence is often associated with third-party activities
- Attestation and acknowledgement
    - Someone must “sign off” on formal compliance documentation
    - Ultamately responsible if the documentation is incorrect
- Internal and external
    - Monitor compliance with internal tools
    - Provide access or information to third-party participants
    - May require ongoing monitoring of third-party operations
- Automation
    - A must-have for large orginizations
    - Can be quite different across vertical markets
    - Many third-party monitoring systems
    - Collect data from people and systems
    - Compile data and report

## **Privacy - CompTIA Security+ SY0-701 - 5.4**

### Privacy legal implication

- This is constantly evolving as new privacy concerns become apparent and as new useage of data arizes
- Local/regional
    - state and local governments set privacy limits
    - Legal information, vehicle registration details, medical listing
- National
    - Privacy laws for everyone in a country
    - HIPPA, online privacy for children under 13, etc
- Global
    - Many countried are working together for privacy

### GDPR - General Data Protection Regulation

- European Union regulation
    - Data protection and privacy for individuals in the EU
    - Name, adress, photo, email address, bank details, posts on social networking websites (social media), medical information, a computer’s IP address, etc.
- Controls export of personal data
    - Users can decide where their data goes
    - Can request removal of data from search engines
- Gives “data subjects” control of their personal data
    - A right to be forgotten

### Data subject

- Any information relating to an identified or identifiable natural person
    - An individual with personal data
- This includes everyone
    - Name, ID number adress information, genetic makeup, physical characteristics, location data, etc
    - You are the data subject
- Laws and regulations
    - Privacy is sdeally defined from the perspective of the data subject

### Data responsibilities

- High-level data relationships
    - Orginizational responsibilities, not always technical
- Data owner
    - Accountable for spesific data, often a senior officer
    - VP of sales owns the customer relationship data
    - reasurer owns the financial information

### Data roles

- Data controller
    - manages the purpose and mean by which personal data is processed
- Data processor
    - Processes data on behalf of the data controller
    - Often a third-party or different group
- Payroll controller and processor
    - Payroll departent (data controller) defines payroll amounts and timeframes
    - Payroll company (data processor) processes payroll and stores employee information

### Data inventory and retention

- What data does your orginization store?
    - You should document your data inventory
- Data inventory
    - A listing of all managed data
    - Owner, update frequency, format of the data
- Internal use
    - Project collaboration, IT security, data quality checks
- External use
    - Select data to publicly share publicly
    - Follow existing laws and regulations

## **Audits and Assessments - CompTIA Security+ SY0-701 - 5.5**

### Audits and assesments

- Not just for taxes
    - There are good reasons to audit your technology
- Cybersecurity audit
    - Examines the IT infrastructure, software, devices, etc
    - checks for effectivness of policies and procedures
    - Find vulnerabilities before the attackers
    - Can be performed internally or by a third-party
- Attestation
    - Provides an opinion of truth or accuracy of a company’s security positioning
    - An auditor will attest to a company’s cybersecurity posture

### Internal audits

- Audits arent only done with third parties
- Audits done by your own company are called internal audits
- Audit committee
    - Oversees risk management activities
    - All audits start and stop with the committee
- Self-assessments
    - Have the orginization perform their own checks
    - Consolidate the self-assessments into ougoing reports

External audits

- This is when an audit is done by a third party, and this may sometimes be mandated
- Regulatory requirments
    - An independent third-party may be required to perform the audit
    - Audit type and frequency are often based on the regulation
- Examinations
    - Audits will often require hands-on research
    - View record, compile records, gather additional details
- Assessment
    - Audit will assess current activities
    - May also provide recomendation for future improvments

## **Penetration Tests - CompTIA Security+ SY0-701 - 5.5**

### Physical penetration testing

- Operating system security can be circumvented by physical means
    - Modify the boot process
    - Boot from other media
    - Modify or replace OS files
- Physical security is key
    - Prevent access by unauthorized individuals
- Assess and test physical security
    - Can you enter a building without a key?
    - What access is avalible inside?
    - Doors, windows, eevators, physical security processes

### Pentesting perspectives

- Offensive
    - The red team
    - Attack the systems and look for vulnerabilities to exploit
- Deffensive
    - The blue team
    - Identify attacks in real time
    - Prevent any unauthorized access
- Integrated
    - Create an ongoing process
    - Identify and patch exploitable systems and services
    - Test agian

### Working knowledge

- How much do you know about the test?
    - Many different approaches
- Known enviornment
    - Full disclosure
- Partially known enviornment
    - A mix of known and unknown
    - Focus on certian systems or applications
- Unknown enviornment
    - The pentester knows nothing about the systems under attack
    - “Blind” test

### Reconnaissance

- Need information before the attack
    - Can’t rush blindly into battle
- Gathering a digital footprint
    - Learn everything you can
- Understand the security practice
    - Firewalls, security configurations
- Minimize the attack area
    - Focus on key systems
- Create a network map
    - Identify routers, networks, remote sites

### Passive reconnaissance

- Learn as much as you can from open sources
    - Theres’s alot of information out there
    - Remarkably different to protect or identify
- Social media
- Corporate website
- Online forums, Reddit
- Social engineering
- Dumpster diving
- Buisness orginizations

### Active reconaissance

- Trying the doors
    - Maybe one is unlocked
    - Don’t open it yet
    - Relativly easy to be seen
- Visible on network traffic and logs
- Ping scans, port scans
- DNS queries
- OS scans, OS fingerprinting
- Service scans, version scans

## **Security Awareness - CompTIA Security+ SY0-701 - 5.6**

### Phishing campains

- How many employees would click a link in a phishing email?
    - There is a way to find out
- Many companies will perform their own phishing campaign
    - Send a phishing smail to your employees
- An automated process
    - Centralized reporting for incorrect clicks
    - Users can receive immediate feedback and security training
    - Some orginizations will schedule in-person training
- The goal is to help your co-workers recognize a phishing attempt
    - Spelling and gramatical errors
    - Domain name and email inconsistencies
    - Unusual attachments
    - Request for personal information
- Respond to reported suspicious messages
    - Email filtering can get the worst offenders
    - Never click a link in an email
    - Never run an attachment from an email
    - All orginizations should have a process for reporting phishing

![This is what it should generally look like when a phishing email is properly blocked by email filters.](Screenshot_From_2025-06-30_20-20-12.png)

This is what it should generally look like when a phishing email is properly blocked by email filters.

### Anomalous behavior recognition

- Risky behavious
    - Modifying hosts file
    - Replacing a core OS file
    - Uploading sensitive files
- Unexpected behavior
    - Logon from another country
    - Increase in data transfers
- Unintentional behavior
    - Typing the wrong domain name
    - Misplacing USB Drives
    - Misconfiguring security settings

### Reporting and monitoring

- Track and analyze security awareness metrics
    - Automated
    - Phishing click rates
    - Password manager adoption, MFA use, password sharing
- Initial
    - First occorence is an opportunity for user training
    - Work towards avoiding the issue in the future
- Recurring
    - The value of long term-monitoring
    - Identify high-frequency security issues
    - Help users with multiple occorrences

### Development

- Create a Security Awareness team
    - Determine roles for training, monitoring, policy creation, etc.
- Esablish a minimum awareness level
    - Information delivery (emails, posters, notices, training)
    - Depth of training based on job function
- Integrate compliance mandates
    - PCI DSS, HIPPA, GDPR, etc.
- Define metrics
    - Assess the performance of security awareness programs
    - Make updates in lower-performing areas

### Execution

- Create the training materials
    - Provided to users in different forms
- Document success measurements
    - How will we know the awareness is working?
- Identify the stakeholders
    - Provide ongoing metrics and performance data
- Deploy the training materials
    - Classroom training, posters, weekly emails, etc.
- Track user training efforts
    - Ongoing monitoring, usually wit an automated reporting system

## **User Training - CompTIA Security+ SY0-701 - 5.6**

### Security awareness training

- Before providing access, train your users
    - Detailed security requirements
- Specialized training
    - Each user role has unique security responsibilities
- Also applies to third-parties
    - Contractors, partners, suppliers
- Detailed documentation and records
    - Problems later can be serve for everyone

### User guidence and training

- **Policy/handbook**
    - document all security requirements
    - Provide access online in policy guidelines
    - Refrence the policies in the employee handbook
- **Situational awareness**
    - Users should always be looking for threats
    - Software attacks: Email links, attachments, unusual URLs, text messages, etc.
    - Physical attacks: USB drives in a FedEx envelope, unlocked building doors, etc.
    - Be ready for anything
- **Insider threat**
    - Difficult to gaurd agianst
    - Add multiple approvals for critical processes
    - Monitor files and systems as much as possible
    - It should be very difficult to make an unauthorized change
- **Password management**
    - Many standards to choose from
    - Guide users with standard requirements (length, complexity, etc.)
    - his is often controlled using technology (Group policy)
- **Removable media and cables**
    - Unknown USB drives can contain malware
    - Unknown cables can be malicious
- **Social engineering**
    - Extensive and ongoing training
    - The attackers are very good
    - The users are your front line of defense
- **Operational security**
    - View security from the attacker’s perspective
    - Users need to identify sensitive data
    - Keep the sensitive data private
- **Hybrid/remote work enviornments**
    - Working from home brings unusual security risks
    - No access to family and friends
    - Additional endpoint security
    - Security policies for VPN access