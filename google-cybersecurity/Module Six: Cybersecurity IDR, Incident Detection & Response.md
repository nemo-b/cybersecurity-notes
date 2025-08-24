COURSE LEARNINGS:

- Incident response lifecycle
- Monitor and analyze network traffic
- Processes and procedures
- Interpret logs and alerts

The five core functions of the NIST CS

- Identify
- Protect
- Detect
- Respond
- Recover

**Incident**: An occurrence that actually on imminently jeopardizes, without lawful authority, the confidentiality, integrity, or availability of information or an information system; or constitutes a violation or imminent threat of violation of law, security policies, security procedures, or acceptable policies

**IMPORTANT NOTE**: All security incidents are events, but not all events are security incidents

**Event**: an observable occurrence on a network, system, or device

The 5 W’s of an incident

- Who triggered the incident
- What happened
- When the incident took place
- Where the incident took place
- Why the incident occored

**Incident handlers journal**: A form of documentation used in incident response

**Computer security incident response teams (CSIRT)**: A specialized group of security professionals that are trained in incident management and response

Roles in CSIRT

- Security analyst
- Technical lead
- Incident coordinator

**Incident response plan**: A document that outlines the procedures to take in each step of incident response

Elements of an incident plan:

- Incident response procedures
- System information
- Other documents

Tool types

- Detection and management tools
- Documentation tools
- Investigative tools

**Documentation**: Any form of recorded content that is used for a specific purpose (this is meant to provide instruction and guidance on topics)

Types of documentation:

- Playbooks
- incident handlers journals
- Policies
- Plans
- Final reports

***Note*** there is no industry standard for documentation, so it depends on the company to see how it should be done. Regardless, it should always be clear and concisely written. 

**Playbook**: A manual that provides detail about any operational action

**Word processor tools**: 

- Google Docs
- One note
- Evernote
- Notepad++

**Ticketing systems**

- Jira

**Other tools**

- Google sheets
- Audio recorded
- Cameras
- Handwritten notes

**Intrusion detection system**: An application that monitors system and network activity and produces alerts on possible intrusions

**IDS and IPS tools**

- Snort
- Zeek
- Kismet
- Sagan
- Suricata

Security operation, automation, and response (SOAR): A collection of applications, tools, and workflows that uses automation to respond to security events

**Network traffic**: The amount of data that moves across a network

**Network data**: The data that’s transmitted between devices on a network

**Indicators of compromise (IOC)**: Observable evidence that suggests signs of potential security incident

**Data exfiltration**: Unauthorized transmission of data from a system

**Defensive measures**:

- Prevent attacker access
- Monitor network activity
- Protect assets
- Detect and stop exfiltration

Components of a packet

- Header
- Payload
- Footer

**Network protocol analyzer (packet sniffer)**: A tool designed to capture and Analyze data traffic within a network

**Packet capture (P-cap)**: A file containing data packets intercepted from an. interface or network

***Note***: Different protocols use different headers

![Screen Shot 2024-04-02 at 8.20.25 PM.png](Screen_Shot_2024-04-02_at_8.20.25_PM.png)

- The **Version** field specifies which version of IP is being used
- **IHL** (Internet Header Length), specifies the length of the IP header plus any options.
- **TOS** (Type of Service), This field tells us if certain packets should be treated with different care.
- **Total length field**, identifies the length of the entire packet, including the headers and the data.

**Identification**, **flags**, and **fragment offset deal** with information related to fragmentation

**Fragmentation**: When an IP packet gets broken up into chunks, which then get transmitted over the wire and reassembled when they arrive at their destination

- **TTL** is similar to how tracking information provides
details about an envelope's expected delivery date.
- The **Protocol** field specifies the protocol used by providing a value, which corresponds to a protocol
- **Header checksum**, stores a value called a checksum, which is used to determine if any errors have occurred in the header.
- The **Source Address** specifies the source IP address
- The **Destination Address** specifies the destination IP address.
- The O**ptions** field is not required and is commonly used for network troubleshooting rather than common traffic

![Screen Shot 2024-04-07 at 6.09.06 PM.png](Screen_Shot_2024-04-07_at_6.09.06_PM.png)

Here is an example of packet information, this holds a lot  of information so please refer to the video for what determines what. [00:40:56](https://www.youtube.com/watch?v=MsGl6lX-YaI&list=PLTZYG7bZ1u6ocTMdhDwwmfjaNv134KcWn&index=6&t=2456s)

**Detection**: The prompt discovery of security events

Challenges in the detection and analysis phase

- Impossible to detect everything
- High volumes of alerts

Benefits of documentation

- Transparency
- Standardization
- Clarity

**Chain of custody**: The process of documenting evidence possession and control during an incident lifestyle

**Broken chain of custody**: Inconsistencies in the collection and logging of evidence in the chain of custody

Chain of custody establishes Integrity, reliability, and accuracy.

**Triage**: The importance of incidents according to their level of importance or urgency

Triage process

1. Receive and assess
2. Assign priority
3. Collect and analyze

Questions to ask

- Is there anything out of the ordinary?
- Are there multiple failed login attempts?
- Did the login happen outside of normal working hours?
- Did the login happen outside of the network?

**Containment**: The act of limiting and preventing additional damage caused by an incident

**Eradication**: The complete removal of the incident elements from all infected systems

**Recovery**: The process of returning infected systems back to normal operations

**Post-incident activity phase**: The process of reviewing an incident to identify areas for improvement during incident handling

**Final report**: Documentation that provides a comprehensive review of an incident

Questions to ask

- What happened?
- What time did it happen?
- Who discovered it?
- How did it get contained?
- What ere the actions taken for recovery?
- What could've been done differently?

**Log**: A record of events that occur within an organizations systems

Log details: 

- Date
- Time
- Location
- Action
- Names

**Log analysis**: The process of examining logs to identify events of interest

Logs contain:

- Timestamps
- System characteristics
- Action

Commonly used log formats

- Syslog
- JavaScript Object Notation (JSON)
- eXtensible Markup Language (XML)
- Comma Separated Values (CSV)

**Telemetry**: The collection and transmission of data for analysis

**Intrusion detection system (IDS)**: An application that monitors activity and alerts on possible intrusions

**Endpoint**: Any device connected on a network

**Host-based intrusion detection system**: An application that monitors the activity of the host on which its installed

**Network-based intrusion detection system**: An application that collects and monitors network traffic and network data

**Signature analysis**: Detection method used to find events of interest

Header

- Source and destination IP adresses
- Source and destination ports
- Protocols
- Traffic direction

**Please refer back to the video from 1:13:00 to get examples of how to use**

SEIM tool, splunk> and Chronicle 

**Search Processing Language (SPL)** - Splunk’s query language

**YARA-L**: A computer language used to create rules for searching through ingested log data

Types of search:

- Unified data model (UDM) - used for normalized data
- Raw log search - used for more in depth non-normalized data
