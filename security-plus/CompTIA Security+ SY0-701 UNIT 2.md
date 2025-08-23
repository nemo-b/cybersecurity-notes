## **Threat Actors - CompTIA Security+ SY0-701 - 2.1**

### Threat actors: Anyone trying to get into a system that's not allowed for any purpose

- Understanding who your treat actor is the first big step as you can understand motive, goals, and what they're planning and how to prepare for it. Some goals could be…
    - Getting money (usually the go-to)
    - Pulling strings; controlling an industry
    - Taking information to sell or blackmail
    - Getting traction, or pulling attention to something
    - It could also simply be someone in the industry like a white-hat hacker

**Hacktivist**: A hacker with a purpose (usually to do something rather than take something); making a business go down for something like philosophical reasons

**Insider threat**: Someone within the business taking advantage of resources to take over something

- Treated as medium level of sophistication
- Usually hard to find, but once found, mildly simple to deal with

**Organized crime**: Group with many assets, hacking a business

- Treated as very sophisticated

**Shadow IT**: Rouge person in the IT field in a business, acting as an insider threat, but with a lot more control, being more dangerous. 

<aside>
💡

Being able to class which type of threat we have, we have a higher chance to solve the issue and protect whatever the thrat is targeting. 

</aside>

## **Common Threat Vectors - CompTIA Security+ SY0-701 - 2.2**

### **Threat vectors**: A vulnerability in a system set in place by an organization

**Message-based vectors**

- These can be links sent in emails, SMS (Short Message Service) links or questions to bait certain responses, or anything else that involves messages.
    - **Phishing attacks**: Hackers sending a link to someone that when they click, can download malware (or send the victim into a website that contains a malware download link),  that can do what the hacker wants.
    - **Image-based vectors**
        - It's a bit hard to understand but from what I do understand, image formats hold information regardless and some information that they hold, could be taken advantage of and used as a threat.
        - Some formats that can be seen as threats are **SVG (Scalable Vector Graphic)** format, and **XML (Extensible Markup Language)** format.
        - The images security concerns would be HTML (HyperText Markup Language)
    - **File-based vectors**: This refers to a situation in which a collection of data is stored in a single location, allowing a hacker the opportunity to introduce harmful information discreetly. Some examples of vulnerable areas would be…
        - Adobe PDF. There's a lot of text, images, and sometimes executable code that could hide malicious code.
        - ZIP/RAR files (or any compression type). They contain many different files and its easy to hide something either within one of those files, or among the other files in the folder.
        - Microsoft Office. You could use macros to send information out to the hacker, or put in files.
    - **Vishing**: Phishing over the phone
    - **Removable device vectors**
        - An example of this would be a hacker leaving a USB in a parking lot, and when it gets picked up and put into a computer, it is recognized as a keyboard by the computer and starts typing things on the computer. These are classified as threats as they could come with macros that steal and export information through hardware.
- Keep software up to date to avoid a lot of patch issues
- Open service ports are also huge vulnerabilities. To solve the issue, you usually use either port based firewalls or application aware firewalls to keep threat actors out.

## **Phishing - CompTIA Security+ SY0-701 - 2.2**

### **Pretexting**: Lying to get information; the threat actor is acting like another person in a situation.

### **Typosquatting**: Using a fake URL that looks similar to something else.

<aside>
💡

Other Social Engineering Attacks - CompTIA Security+ SY0-701 - 2.2This unit lesson is a expanded version of the phishing information in the last lesson. This just expands and shows some things that show suspicion. Generally though, this information is well known and to be fair, is mostly common sense. If you need more clarification, feel free to rewatch the video.

</aside>

## **Impersonation - CompTIA Security+ SY0-701 - 2.2**

### Impersonation

- There is usually an acted out situation where people pretend to be someone they're not. This is meant to help you gain some trust in something you shouldn't.

<aside>
💡

This unit (similarly to last unit), is mostly a recap and expanding of what was learned in the last two lessons. Im solely going to include useful words similar to how i wrote last lseeon. 

</aside>

## **Watering Hole Attacks - CompTIA Security+ SY0-701 - 2.2**

**Watering hole attack**: when a threat actor goes to a third party and pollutes data you intend to use later, before you can get to it. This leads to the threat actors malware reaching your systems if you aren't taking the proper precautions while trusting an outside source. 

- When other methods of infiltrating a system won't work, watering hole attacks are used as an after measure most of the time.

## **Other Social Engineering Attacks - CompTIA Security+ SY0-701 - 2.2**

Other social engineering attacks

- Misinformation and disinformation is used to change how people think about issues, or distract them from the truth in the situation
    - This can be harmful to a personal business because social presence is a serious part in running an organization
- Brand impersonation
    - This is when people pretend to be another place
    - This is bad because when people closely pretend to be a popular brand, it could lead to malware through things like typo squatting

## **Memory Injections - CompTIA Security+ SY0-701 - 2.3**

### Finding malware

- Everything on your computer works through your computer’s memory, so malware targets your computer's memory
    - Memory forensics can find the malicious code
- Memory contains running processes
    - DLLs (Dynamic Link Libraries)
    - Threads
    - Buffers
    - Memory management functions
    - etc…
- Malware injects itself inside a running process to hide inside of it

### Memory injection

- Malware is hidden within the starting address, and ending address of an existing process
- The injected malware has the same rights, permissions, and privileges as the process it's gotten into (when value is over 24000 in “Variable B”)

### DLL injection

- The threat actor injects a path into a malicious DLL, and it runs as part of the target process
- This is one of the most popular injection methods

## **Buffer Overflows - CompTIA Security+ SY0-701 - 2.3**

### Buffer overflows

- This is when an attacker writes excessive information that's unexpected into memory, and that information overflows into another section of memory
    - **Bounds checking**: Bounds checking is a security practice that ensures a program only accesses memory within predefined limits. It verifies that an input value falls within an acceptable range before the program uses it, preventing errors and vulnerabilities such as buffer overflows, which can lead to unauthorized access or crashes.
- Exploiting buffer overflows isn't a simple task, as it could simply cause systems to crash. This means it'll take a lot of time for the system to actually do what an attacker would like.

## **Race Conditions - CompTIA Security+ SY0-701 - 2.3**

### Race Conditions

**Race condition**: When two events happen nearly at the same time within an application, and the application doesn't take into account that the two events are happening simultaneously

- This is usually a programming fault that could lead to application error
- EX: Moving money from one account to another, and the application makes the assumption they're from the same place, and send both to one account.

### **Malicious Updates - CompTIA Security+ SY0-701 - 2.3**

### Software updates

- Always keep your operating systems up to date
- Make sure the sources are from trusted places, and that you have backups of the whole system before making big changes
- Malicious code COULD be found inside the “Update”

### Downloading & Updating

- Always be highly conscious of what you download as anything could be malicious
- Confirm the source of the download and always go directly to developers sites
- Many operating systems will only allow signed apps (digitally signed)

## **Operating System Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Operating systems

- Keeping the operating system up-to-date makes sure that the operating system is less vulnerable to malware made for specific versions.
- Microsoft updates Windows OS updates on the second Tuesday of each month, its usually referred to as “Patch Tuesday”

## **SQL Injection - CompTIA Security+ SY0-701 - 2.3**

**Code injection**: Adding your own information into a data stream

- This happens because of bad programming

SQL injection 

- SQL (Structured Query Language) is the most common relational database management system language
- SQL injections (SQLi) is when someone puts their own SQL requests into an existing application
    - Realistic, your application should never allow this
- SQL injections are very dangerous as you practically have complete control over all information in a database

<aside>
💡

if you find the prompted code = … OR ‘1’ = ‘1’”; then it means that its likely injected code, trying to take everything in a system. The example code used in the video was 

(”SELECT * FROM users WHERE name = ‘Professor**’ OR ‘1’ = ‘1**’’”). 

The bold part is the injected code.

</aside>

## **Cross-site Scripting - CompTIA Security+ SY0-701 - 2.3**

### Cross-site Scripting (XSS)

- It's called XSS because CSS is already taken by Cascading Style Sheets (As I already should know)
- It was called cross site scripting because it targeted browsers
    - The attack is based on **JavaScript**, which is enabled by just about everyone in their browser
- This is usually done when an attacker sends a link to a REAL trusted site, but when the link is clicked, it has additional information. The information is usually a malicious script that can take a lot of information from the browser.

Persisted (stored) XXS attack

- Attacker posts a message to a social site, so everyone who visits the page with the software has the malicious code run through their browser.

## **Hardware Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Hardware devices

- Any device connected to a network could lead to a security risk

### Firmware

- This is the operating system of the hardware device
- The only people who can really control the firmware are the vendors
- Usually there is an update every month of less on operating systems
    - If the OS isnt updating it could be a End-of-life (EOL). this means that the manufacturer will stop making a device and may stop supporting it.
    - An End-of-service-life (EOSL) is when a manufacturer stops selling a product and stops supporting it. This is dangerout because it means there are no more  patches, making the device more vulnerable.

### Legacy platforms

- Legacy devices are devices that run older operating systems, applications and middleware
- While they may seem replaceable, they could hold EOL software that is neccesary for cerian functions

## **Virtualization Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Virtualization security

- You should be keepinng up with virtual machines as you are with phisical devices
- There are virtualization vulnerabilities
    - Local privledge esclations
    - Command injection
    - Imformation disclosure

### VM escape protection

- Virtual machines are self-contained, which means you shouldnt be able to move from inside one VM on a hyperviser to a different VM on the same hyperviser
    - When you do jump between VM’s its valled Virtual machine escapng
    - Virtual machine escaping is dangerous as you basically have complete control of the device from it

## **Cloud-specific Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Security in the cloud

- Many companies use the cloud to store information and data
    - The information stored in the cloud is usually sensitive information
- A majority of companies, about 76%, dont even use multifactor authentication for management console users

### Attack the service

Denial of service (DoS)

- Usually done as an attack to people trying to access applications in the cloud

When people can manually navigate through the structure of web servers, it's called **Directory traversal**. This is usually not supposed to be possible, but it can happen.

**Out of bounds writing** is when unauthorized people write in memory areas. This could lead to data corruption, system crashes, or code execution.

## **Supply Chain Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

Service providers

- Service providers give you access to tools or data, and because you rely on them, they have to be the ones to protect THEIR systems
- If the service provider gets hacked, your information could be at risk as well

## **Misconfiguration Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Network vulnerabilities

- If you leave information in an open spot on the internet, it will become certian bait for hackers
- Make passwords strong for important accounts
    - Administrators are the imoprtant acccounts on window
    - The root is the important account on linux
- Watch out for the “HTTP” issue as it could leak information
- **Internet of things (IoT)**: The Internet of Things (IoT) refers to the growing network of internet-enabled devices. It includes fitness trackers, smart heating systems, smart cities, and potentially driverless cars.
- Open ports allow attackers to control a part of a system. These are blocked my firewalls.

## **Mobile Device Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Mobile device security

- Mobile devices are usually packed with alot of personal information

### Jailbreaking/rooting

Jailbreaking: Changing the purpose of a purpose base system (Mobile devices)

- On Andraoid its called rooting while on AppleiOS its called jailbreaking
- Jailbreaking replaces the Firmware or operating system
- Replacing the firmware to one that contains malicious code could destroy a phone

### Downloading/sideloading

**Sideloading**: Installing software on a device without using the approved app store or software distribution channel

- Sideloading could leave you vulnerable to malicious code as the place you download from could be dangerous

## **Zero-day Vulnerabilities - CompTIA Security+ SY0-701 - 2.3**

### Vulnerabilities

- Whatever device your using may already have vulnerabilities, but you wouldnt know uness you 100% understand the device (which nobody truly does)
- Attackers try to find vulnerabilities first to hack systems befre there are patches

### Zero-day attacks

- An attack without a patch or method of mitigation
    - Happens because the vulnerability hasnt been recognized by the proviers of the device to fix
    - Until a patch is avalible, the attacker can do whatever theyd like with the attacked systems

> “Its difficult to protect a system if you have no idea a problem even exists.” - Professor Messer
> 

## **An Overview of Malware - CompTIA Security+ SY0-701 - 2.4**

### Malware

- Malware is a broad term that describes any type of software that does bad things to a system
- Malware types and methods
    - **Viruses**: Malware that attaches to files and spreads when the file is run.
    - **Worms**: Malware that self-replicates and spreads across networks without user action.
    - **Ransomware**: Malware that The owner of a resource decides who has access.locks or encrypts your files and demands payment to unlock them.
    - **Trojan horse**: Malware disguised as legitimate software to trick users into installing it.
    - **Root kit**: Malware that hides itself and gives attackers control over your system.
    - **Keylogger**: Malware that records everything you type to steal passwords or data.
    - **Spyware**: Malware that secretly collects your information without permission.
    - **Bloatware**: Pre-installed or unnecessary software that takes up space and slows down your device but usually isn’t malicious.
    - **Logic bomb**: Malware triggered by specific actions or conditions.
    - **Adware**: Malware that shows unwanted ads, sometimes tracking your behavior.
- One thing to note is that typically malware works together to break into a serious system
- Always have an offline backup to keep it away from things like ransomware

# **Viruses and Worms - CompTIA Security+ SY0-701 - 2.4**

### Viruses

- Viruses are known as one of the most common forms of malware
- Viruses can reprocuse itself in a system and spead through a network
- Some viruses are invisible and some are simply annoying
- **Antiviruses** are used to defend systems from viruses
- There are different types of viruses…
    - Program viruses: Viruses that are layed as part of an application
    - Boot secor viruses: Loads up with the power of the compputer with your OS
    - Scrpit viruses: OS and browser based
    - Macro viruses: Auto running sequences usually run in excel (Microsoft Office)
    - Fileless virus: A dangerous type of virus that is downloaded through a link that runs itself through memory, invisible to anyone thats unaware

### Worms

- Malware that self-replicate without human intervention at the speed of the victims network
- They move freely throughout networks and can only really be stopped with **Firewalls & IDS/IPS**
- Rare occorences

# **Spyware and Bloatware - CompTIA Security+ SY0-701 - 2.4**

### Spyware

- Malware that spies on you like keyloggers
- Can be stopped with anti-virus/anti-malware
    - One thing to note is that thirdparty software like malwarebyte can find and sometimes get rid of malware as well
- Always research what your putting on your system

## **Other Malware Types - CompTIA Security+ SY0-701 - 2.4**

### Keyloggers

- Takes every keystroke you click and keeps track of them to take things like passwords
- When your using a keyboard for things

### Logic bomb

- A malware that waits for a spesific event before activating
- Usually used by hacktivists

### Rootkits

- Rootkits modify core system files which means it runs as PART of the OS
- When it is running, it is invisible to the OS, meaning something task manager would be able to see
- **Secure boot with UEFI** is security in the BIOS that can identify something running within the operating system, namely, the rootkits. It also stops the rootkit from being able to run, which means the problem is to a degree solved.

<aside>
💡

Remember, alot of problems could be avoided if the people within a company only has the rights or permissions to do their jobs. 

</aside>

## **Physical Attacks - CompTIA Security+ SY0-701 - 2.4**

### Physical attacks

- If you can physically get to a device, there is a good chance that you could get into a system
- Brute force is something that is associated with getting into a system for password discovery, but it is most commonly noted as a way to physically get into an area as well

> “Door locks only keep out the honest people” - Professor Messer
> 
- HVAC systems are usually the least protected in a company, making them large vulnerabilities. Access to a HVAC system could mean turning off the AC, overheating devices in the building slowing them down.
- Watch out for smoke and/or fire

### RFID cloning

- RFID is a form of ID that is used for things like acess badges and key fobs
- RFID cloners can even be found on amazon for less that $50 which means duplicating acess badges isnt a big roblem for someone trying to really get into a system
    - Physically protecting assets like badges is a serious issue
    - RFID cloners are also very fast, and it could be as simple as brushing it “accidentaly” by someone with an access card to clone it, making this a VERY quick process
    - Multi-factor Authentication (MFA) is one good way to prevent this

## **Denial of Service - CompTIA Security+ SY0-701 - 2.4**

### Denial of service (DoS)

- DoS is the forcing of a service to fail, typically by overloading the service
- DoS’ are usually due to design failures or vulnerabulities, they coudl also just be a smokescreen to lead another malware into the systems
- This could give a cometitive advantage to buisnesses as if a competitordoesnt have access to important services, they could be the replacement for their customers
- Sometimes their easy to make by unplugging a system

**Bandwidth DoS**: This is an attack aimed at overwhelming a network's bandwidth to disrupt services. By flooding the target with excessive requests, it slows down or completely disables access for legitimate users. This results in downtime, making resources unavailable and causing frustration.

**Distributed Denial of Service (DDoS)**: This is a cyber attack where multiple compromised computers are used to flood a target server or network with overwhelming traffic, causing it to slow down or become completely unavailable to users.

- DNS amplification DoS’ are when an attacker would send a small peice of information, and the system would take that information and amplify it, or expnd it into alot of information, flooding a system, and usually crashing the devices its sent to

## **DNS Attacks - CompTIA Security+ SY0-701 - 2.4**

- **Domain name services (DNS):** DNS, or Domain Name System, is like the internet's phone book. It translates user-friendly domain names (like www.example.com) into IP addresses (like 192.0.2.1) that computers use to identify each other on the network. This system makes it easier for people to access websites without needing to remember complex numbers.

### DNS poisoning

- This would be the modification of DNS servers. This is not traditional as its VERY difficult to get into a DNS server to the point it would be almost impossible, or would take very well versed hackers to do.
- Hackers may attack the host file instead to get acess to the DNS system. This usually means you need high level clearance to even get into an account to get into the DNS to modify it.
- DNS poisoning basically rewrites the destination of a DNS server so that instead of going to the intentional location, like youtube.com, it would go to a different page that could hold malware.

### Domain hijacking

- This is basically the last bulletpoint in the secation “DNS poisoning”

## **Wireless Attacks - CompTIA Security+ SY0-701 - 2.4**

### Wireless attacks

- A wireles deauthentication attack is a cyber attack that deactivates a persons wireless devices in a similar was to a DoS
- For these attacks to work youd need to know the MAC adress or hardare wi-fi adress of the user you want to disconnect
    - The code is `airodump-ng` and then specifying the wireless card used on your linix device
- This form od DoS has already been adressed by the IEEE
- Encrypting important management frames is a good way to protect agianst these types of attacks
- There are alot more ways that wireless jamming could happen. Here are a few…
    - Constant flows of random bits of information
    - Constant, legitamate frames
    - Data sent at random times, or random data and legitamate frames
    - etc

Radio frequency (RF) jamming

- This is a form of DoS by transmitting frequencies along with wifi and overlapping thhem to be untranslatable to a device, making it unnable to connect to networks
    - It could also be unintentional by standing next to a microwave or florecent lights or other things that give off strong frequency levels

## **On-path Attacks - CompTIA Security+ SY0-701 - 2.4**

On-path network attack

- This is an attack where a man sits in a place between both networks where he can see all information going between the two systems, sometimes it may even be able to modify information being sent
    - This is a very terrifying way of attacking systems as its almost imposible for the two systes to know that their information is being redirected to a third party
    - One form of this is ARP poisoning, whats required for this is a subnet. Because ARP doesnt have an security or encryption to it, its simple for someone to pull off.
- This is also known as a man-in-the-middle attack

On-path browser attack

- This is another form of “on-path” attacks where the middleman was on the same computer a the victim
    - Malware/trojan is configured as a proxy that is able to redirect traffic before and after its sent to the network, because of that, encryption does nothing to protect the services
    - It waits for you to log into something like a bank account, ten saves all of that information and cleans you out
- This is also known as a man-in-the-broswer attack

## **Replay Attacks - CompTIA Security+ SY0-701- 2.4**

### Replay attacks

**Replay attack**: A replay attack is a network security breach where an attacker intercepts and reuses valid data transmission to fraudulently gain unauthorized access or perform illicit actions. This often involves capturing data packets and sending them again to trick a system into accepting them as legitimate.

- Pass the hash is a form of replay attack where the client sends a normal authentication request to  serve. Between the traffic, the hacker is intercepting or redirecting it in between the client and server with the username and hashed password. From there, the hacker then takes that copied information and continues sending it to the server, then whats sent back is the acctual information needed after authentication, giving the hacker access to whatever was just logged into.
    - One way this can be solved is using encryption
    - Another way this could help is by “salting the information” (adding extra stuff to distract the hacker, and works well with authentication)

### Browser cookies and session ID’s

- Cookies are simply information stored on your computer by the browser
    - These are used for tracking, personalization and session management
- Cookies also contain session ID’s, which is the information that hackers usually target because it is what maintains your session across multiple browser sessions
    - A subsection of this would be session hijacking (Sidejacking). Sidejacking is whenever a session ID is stolen and used in a web serve so that an attacker could just continue from where a victim left off on their broswer
- Session hijacking could be stopped by end-to-end encryption, or *encrypt end-to-somewhere* (research)

## **Malicious Code - CompTIA Security+ SY0-701 - 2.4**

### Summary

This unit was basically a rundown of EveryTHING ive already learned about malware, but with real life examples. 

## **Application Attacks - CompTIA Security+ SY0-701 - 2.4**

### Injection attacks

- Code injection is adding your own information to a data stream
    - Different types of injections
        - HTML Injection
        - SQL Injection
        - XML Injection
        - LDAP Injection
        - etc…

### Buffer overflows

- Buffer overflowing is when you overwrite a buffer of memory, and as a result, the information overflows into other memory areas
    - This can be corrected with bounds checking
    - This is a very difficult thing to exploit

## Privledge esclation

- The higher privledge a victim has, the more acess a hacker has in a system
    - The goal for an hacker is to get administrator access
- A solution for this would be to have updated Anti-malware/Anti-virus software
- Elevation of privledge vulnerability was an issue mostly prevalent in 2008-2016
    - The hackers goal here is to get System Privledges, which is the HIGHEST level of access for a hacker avalible

### Cross-site requests

- Cross-site requests are a common, and lefitimate way of using information from a seperate server on websites
    - EX: A youtube video on a website like ProfessorMesser.com
- Cross-site request forgery is an attack on a browser where the hacker attempts

### Directory traversal

- This is simply when you switch through different parts of the system like folders
- People shoud oly have access to the directories that they need for their job

## **Cryptographic Attacks - CompTIA Security+ SY0-701 - 2.4**

### Cryptographic attacks

- Youve encrypted data and sent is to another person
- The attacker woud need the key to ee the information
- Keep in mind when a hacker cant get in without a key, they are likely to imediatly try to get into a system or whatever their trying to do without the key, so you need to be sure the system is well gaurded otherwise the key is useless

### Birthday attack

- This is a problem defined by its example
    - EX: In a room of 23 students, the chance of two of them sharing a birthday is 50%. For a class of 30, the percentage would rise to about 30%. This means if this was an orginized system, there would be “duplicate” data though its legitamate
- The “duplicate data” I used in the example is really called **hash collision**
    - Collisions are usually found by brute forcing by hackers
    - The way to combat brute force attacks here is to extend the length of the hashs so that they take much longer to decode
- A hash being the exact same even after encryption is called a collision, and these are really bad because they are meant to be two seperate values
    - Hash collisions are VERY rare, but if their found it likely means your encryption method is not good and needs to be changed

### Downgrade attack

- This is an attack type that is using a perfectly good encrytion, but the implementation of the encryption shows the results quickly making the system very vulnerable
- Thils also leads to SSL stripping which takes the “S” from “HTTPS”, which makes the website more vulnerable
    - Heres a super long Ai response about how SSL stripping works for revision:
    - SSL stripping is a type of attack that targets HTTPS communication between a user and a web server. The attack is primarily executed by an adversary who intercepts the user's requests and downgrades them from a secure HTTPS connection to an insecure HTTP connection without the user's knowledge. This is typically done using techniques such as man-in-the-middle (MitM) attacks.
    When a user attempts to connect to a website that supports HTTPS, the attacker intercepts the connection and sends the user a non-secure HTTP version instead. The attacker then relays information between the user and the website, allowing them to capture sensitive data, such as login credentials or credit card numbers, while the user believes they are securely communicating with the intended server.
    One common method to facilitate SSL stripping is to exploit the lack of HSTS (HTTP Strict Transport Security) on a website. If a site does not enforce HSTS, the attacker can easily redirect the user to the unsafe version. To mitigate such vulnerabilities, users are encouraged to avoid clicking on links from unknown sources, ensure their browser indicates a secure connection (e.g., showing "https://" in the URL), and utilize tools that enhance online security.

## **Password Attacks - CompTIA Security+ SY0-701 - 2.4**

Hashing passwords

- Hashes are like a fingerprint that makes data unique and is used alot for passwords
- When saving something as a hash, your taking a variable input and saving it as a fixed-length string of text; which is practically a form of encryption

### Spraying attack

- Hackers usually attempt to log into accounts using a brute force moethod where they try every password possible to force the syste to give one eventually, but that takes long and they may be locked out of the account
- Instead of brute forcing, they try to use the most common passwords first
    - While using common passwords is a uhge security risk, its called “common passwords” for a reason, as many many people still use them regardless of its risk
    - Here is a list of the top 10,000 most common passwords as examples: [https://en.wikipedia.org/wiki/Wikipedia:10,000_most_common_passwords](https://en.wikipedia.org/wiki/Wikipedia:10,000_most_common_passwords)
    - **Spraying attacks** are “brute force attacks” (not really but close) where for the hacker, the threat of a lockout, could be leading to a security report of a alarm/alert. One thing hackers would do is take the top three most common passwords and try tham on one account. After they try the top three, they moe onto another account hoping for a different result. This leads o no alarms or lockCloud Infrastructures - CompTIA Security+ SY0-701 - 3.1outs.
        - The way this could be dealt with is as simple as enforcing strong password policies at work

## **Indicators of Compromise - CompTIA Security+ SY0-701 - 2.4**

### Indicators of compromise (IOC)

- An event that indicates an intrusion
    - Some indicators could be…
        - Unusual amount of network activity
        - Change to file hash values
        - Irregular international traffic
        - Changes to DNS data
        - Uncommon login patterns
        - Spikes of read equests to certian files
- The biggest IOC is account logout’s
    - This could be intentional by the buisness
    - This could also be a ploy used by hackers to keep you from logging in to

### Concurrent session usage

- Concurrent session usage tells us that if we are in one session, we cant also be in another session
- If there is a single person on multiple devices that arent meant to run together like unrigistered devices, it likely means there is an attacker in the system

### Resource consumption

- Resource comsumption is when an attacker overuses resources in a way that causes problems in a system
    - Indicators of this would beCloud Infrastructures - CompTIA Security+ SY0-701 - 3.1 spikes in resource usage at weird times in the day like 3AM, or just general overusgae of things unexpectedly
- Resource inaccessability is whenever you dont have access to something in a server. Here are some examples of when this would happen
    - Server being down
    - Network disruption
    - Server outage
    - Encrypted data (meaning potentional ransomware attack)
    - Brute force attacks

### Logging

- In cybersecurity, one of the most important things your meant to do is make logs of events and situations to keep track of
    - “Out-of-cycle” refers to when things appear in the logs when they arent meant to be there
    - This may happen becuse of firewall traffic and make sure its meant to be there or not
- Missing logs could mean that a hacker may have deleted it to make sure there isnt a record that they were on that system at a point
- Information is everywhere…
    - Authentication logs
    - File access logs
    - Firewall logs
    - Proxy logs
    - Server logs
- Be sure to set up logs for all avalible systems and have good storage of that info

## **Segmentation and Access Control - CompTIA Security+ SY0-701 - 2.5**

### Segmenting the network

- Segmenting the network into groups make it easy to keep data safe by protecting areas individuallyCloud Infrastructures - CompTIA Security+ SY0-701 - 3.1
    - One way it would be safer is that if information is stolen, it's easier to see where it was stolen from so you could work backwards from the issue

### Access control lists (ACL’s)

- Access control lists are lists that allow or disallow traffic in groups
    - They also restrict access to network devices
- ACL’s are only held onto by high authority personell like admins
- This includes **application allow lists** and **application deny lists**
    - This makes sure that only legitamate apps would be allowed to do things on devices
    - Allow lists
        - Allow lists dont let any program to run unless spesifically allowed to do so. These are very restrictive, but keep many programs from being hit with malware and other issues.
    - Deny lists
        - Deny lists let every program run, unless spesifically mentioned to not be allowed. These are less restrictive but also allow for vunerabilities to show like malware and viruses.
        - This means to use deny lists effectivly, you must maintain your software and have anti-viruses and anti-malware, as well as other procautions to run.

**Application hash**: Instead of an application being known for its name, it instead is identified by a hashed version that is a variable for the name of the application. 

## **Mitigation Techniques - CompTIA Security+ SY0-701 - 2.5**

### Mitigating risks

- Patching is a simple way to fix vulnerabilities
    - This happens every month and are INCREDIBLY important
    - This has been descussed alot so if extra info is needed go to the video
- Encryption
    - This has been discussed lot, its like a MFA for accessing data. Makies data hard to read without knowing how to decode (using an encryption key)
    - File level incryption (Windows EFS)
    - Full disk encryption (FDE)
        - This encrypts everything on the drive
        - You can do this with things such as Bitlocker, FileVault, or whatever else your job may use
    - Application data encryption
        - This is managed my the app and makes sure stored data in the app is proteted
- Least privledge
    - This is simply the idea that limits how much anyone in the company can do to only what they need to be able to do their job
- Configuration enforcement
    - A Posture assesment is a check everytime a device connects to the company servers
    - Extensive checks means you check indiviudual things in a device like what OS patch version it is, EDR (Endpoint Detection and Response) version, firewall status, etc.
- Make sure to qurintine devices that dont pass checks
- Decommisioning
    - This is something thats treated as a formal policy that takes systems away from being used in a safe manner because data in the “trash” can still be taken and used
    - Its mostly used for storage deices like hard drive, SSD’s and USB drives

## **Hardening Techniques - CompTIA Security+ SY0-701 - 2.5**

### System hardening

- Enforce password policies
- Updates for OS. service packs and security patches
- Network and security

### System security

**Endpoint detection and response (EDR)**: Also referred to as endpoint detection and threat response (EDTR), is an endpoint security solution that continuously monitors end-user devices to detect and respond to cyber threats like ransomware and malware.

- This is arguable one of the most useful things you can use in the field of cybersecurity as it automates defensive programs

**Host-based firewall**: this is a software based firewall that runs on every endpoint and allows or disallows incoming and/or outgoing application traffic

**Host-based intrusion prevension system (HIPS)**: These recognize and block known attacks, secure OS and application configs, validate service requestion, and much more.

### Ports

- Open ports are HUMOUNGOUS VULNERABILITIES. Every port must be closed ecept required ones. firewalls are used for these.
