How to choose topology
- cost effective
- easy installation
- flexibility
- reliable security

## Simplex, Half-Duplex and Full-Duplex Communication | Transmission modes in communication system (ALL ABOUT ELECTRONICS, 2024)
- Data communication is exchange of data.
- Can be wired or wireless
- Can be one-way or two-way

Simplex is one way involving transmitter and receiver, e.g radio broadcasting, input devices or output devices.

Half-Duplex is two-way, but data flows one at a time, e.g walkie talkie.

Full-Duplex is two-way allowing simultaneous data flow in both directions. The two approaches are:
- frequency division duplexing: using different frequencies, e.g satelite
- time division duplexing: using different short time slots, e.g wifi and cellular network

## Network devices explained: Routers, switches, hubs & more | Networking Basics by (WhiteboardDoodles, 2024)

- Enable smooth functioning of communication systems within a network. They are essential components.
### Router
- Direct data packets to appropriate destination based on IP addresses.
- Operate at network layer of the OSI model.
- Connect multiple devices within LAN and link LAN to internet.
- Enable seamless data flow between devices.
- Often include security features, e.g., firewall, NAT
- Manage traffic efficiently, and prioritize data.
### Switch
- Facilitate communication within LAN.
- Operate at data link layer of the OSI model.
- Receive, process and forward data to appropriate data.
- Function primarily within a single network, using MAC address to determine where to send the data.
- Minimize network congestion.
- Devices connect to it via ethernet cables.
### Hub
- Connects several devices within a LAN.
- Broadcasts data to all connected devices.
- Largely been replaced by switches.
### Modem
- Short for modulator-demodulator.
- Connects local network to internet by converting digital signals from device to analog signals that can be transmitted over telephone lines, cable or fibre optics.
- Primarily provides service to the internet by communicating with ISP.
- Modem router is a modern general convenient solution.
### Access Point (AP)
- Expands wireless network, where router signal may be weak or inconsistent.
- Connect to router using ethernet cables and can broadcast strong Wi-Fi signal in a local area.
- Improves overall network performance
### Firewall
- Security barrier between internal network and internet.
- Hardware firewall is installed in network's entrypoint.
- Prevent unauthorized access, malwayre and cybersecurity risks.
### Network Interface Card (NIC)
- Bridge between device and network.
- Wired and wireless available; versatile.
### Repeater
- Regenerates and amplifies signals to extend network reach.
### Bridge
- Connects 2 or more network segments.
- Operates at data-link layer.
- Less common due to switches.
### Gateway
- Connects different networks; acts as translator when different protocols exist.
- Ensures compatibility.
### Load Balancer
- Manages traffic.
- Distributes incoming data requests evenly, preventing server from overload.
- Used in environments with large traffic.

## How the Internet works in 5 minutes (Aaron, 19 Feb 2009)
- Simply a wire.
- Everyday computers are clients because they are indirectly connected to the internet via ISPs.
- Data is sent in packets over the internet.
- Everything connected to the internet has an IP address.

## What is Internet Service Provider | How Internet Service Provider Works | Intellipaat (Intellipaat, 2022)
- Company/org providing services for internet access.
- First commercial ISP was in Australia and USA in 1989, called "The World". Slow dial up with wide customer base in 2 years.
- DSL (Digital Subscriber Line). First broadband through phone lines
- Cable broadband in 1996.
- Fibre Optics are flexible strands of glass with high-speed.
- Satellite helps rural areas.
### Tier 1 (aka Backbone ISP)
- Largest; connect different countries. Peer with each other at zero cost
### Tier 2 (aka Regional ISP)
- Connect different states in a country.
- Buys services from tier 2. 
- Peer with each other at a very low cost.
### Tier 3 (aka Local ISP)
- Smallest; buy connection from tier 2.

### ISP Techniques
- Mailbox
- Hosting
- Transit
- Virtual
- Free
- Wireless
### Factors in choosing
- Bandwidth
- Connection stability
- Customer volume and traffic
- Traffic volume during peak hours
- Virtual hosting features
- Capacity of e-mails box
- Stability and staying power
- Customer service and local support
- Price

## The Internet and the World Wide Web (MrBrownCS, 26 Sep 2017)
 - The internet is the worldwide collection of networks that use the Internet Protocol Suite (TCP/IP).
 - The World Wide Web (WWW) is the collection of web pages hosted on web servers. It runs using HTTP.
 - The internet is hardware (the literal wires) and the web is the resources hosted on the internet.
 - URLs help address specific web resources.
 - Data transverses the internet through routers forwarding packets.
- An IP address uniquely identifies a device on a network, and defines where it is located geographically.
- The router uses the destination IP address of the packet to identify where to send the packet, and routing algorithms determine the best route to get it there.
- This method of data transmission is known as packet switching.
- No fixed path is created between communicating devices; each packet can take a different route to reach its destination.
- Packets are divided into:
	- **Header**: contains info about the data, like:
		- packet number (position in sequence)
		- MAC & IP address of sender & receiver
		- protocol being used
	- **Data**
	- **Trailer**: contains a checksum; a validation check to determine if an error has been introduced. 
		Sender and receiver calculate a checksum using a function applied to the data. If they match, then the data hasn't been corrupted.

## IP addresses and DNS | Internet 101 | Computer Science | Khan Academy (Khan Academy, 2019)

## What are the CIA triad, AAA, and Non-repudiation in Cybersecurity? CompTIA Security Plus 701 - 1.2 (Ken Underhill - Cybersecurity Training, 6 Mar 2024)

- Confidentiality, Integrity and Availability.
- Confidentiality is to help protect data from unauthorized access, disclosure or theft. Can be done with encryption, access control and data classification.
- Integrity makes sure data hasn't been altered in any way. Can be done with hashing, digital signatures and version control.
- Availability ensures resources are available when needed. Can be protected using Cloudflare for DDOS protection, and ensuring no hardware failure.
- Non-repudiation ensures a user can't deny what they do. digital signatures, time stamping, auto logging.
- Authentication, Authorization and Accounting
- Authentication is identifying that a user is who they say they are.
- Authorization determines what an authenticated user can actually access. Can be done with RBAC (role-based) and ABAC (attribute-based). Also PBAC (policy-based).
- Accounting involves tracking and recording activity of users. For compliance and incidence response.
- Gap Analysis is analyzing current state and goal. Allows analysis of gaps and how to get better. What to change to get better over time.

## Program Threats: Understanding Viruses, Trojans, Worms & Malware for Beginners (CodeLucky, 16 May 2025)

- Trojan horse is malicious code that seems legitimate. Requires user activation to execute and can't self-replicate like viruses. Often used to establish backdoors and steal sensitive information. Types:
	- **Backdoor**: create unauthorized access point to gain remote control, eg remote access trojans
	- **Spyware**: monitors and collects info, eg keyloggers and screen recorders
	- **Banking**: specifically for financial info, eg zeus, spyeye
	- **Ransomware**: encrypts user files and demands payment for decryption, eg wannacry, ryuk
	- **SMS**: short message service. infect mobile device to send premium-rate sms messages, generating revenue at user expense. eg fakeinst, opfake
	- **Botnet**: turns system into zombies that can be remotely controlled for distributed attacks. eg mirai, emotet.
- Virus is malware that when executed, replicates itself by modifying other programs and inserting its own code. Self replicating and must be attached to a host file. Can modify host code and need an execution trigger. Use evasion techniques and deliver payload. Types:
	- **Boot Sector**: infects master boot record. Activates at boot before OS loads. eg. Michaelangelo, Form.
	- **File Infector**: attach to executables. eg. CIH/Chernobyl, Cascade.
	- **Multipartite**: combine boot and file and can spread through multiple vectors. eg. Tequila, Flip.
	- **Polymorphic**: change code structure with each infection to evade detection by antivirus. eg.  `encrypt(virus_code, random_key);`
	- **Stealth**: Hides from detection by intercepting system calls and returning fake information. eg. `hook_system_call(read_file);`
	- **Macro**: Written in macro language embedded in documents like Word or Excel files. eg. `Sub AutoOpen() InfectDocument() End Sub`
- Worm is standalone malware that replicates itself to spread to other computers. Self replicating without host program, propagates via network. Spreads autonomously without user action, active scanning for vulnerabilities and ability to consume network bandwidth and resources. Notable in history:
	- Morris Worm: experiment by Robert Morris in 1988, exploited Unix sendmail, finger, and rsh/rexec.
	- Code Red: exploited buffer overflow vulnerability to target MS IIS web server in 2001, launched DDOS attacks, defaced sites with "Hacked By Chinese!"
	- Sasser: by German CS student Sven Jaschan in 2004, exploiting vulnerability in Windows' LSASS (Local Security Authority Subsystem Service)
	- Stuxnet: 2010, sophisticated, targeting industrial control systems, specifically Siemen's SCADA systems. Believed to be by US and Israel to sabotage Iran's nuclear program. First known cyber weapon to cause physical damage.
- Malware is any malicious software. Can take many forms and explore various vulnerabilities. Advanced types:
	- **Rootkit**: stays stealthy while providing privileged access to system. May modify system files and kernel to stay hidden. eg.
		```
		hook_system_call(detect_process);
		hide_files("/etc/secret/");
		```
	- **Ransomware**: encrypts files and demands payment for decryption. Often spreads through phishing emails or exploiting vulnerabilities. eg. WAnnaCry, Petya, Ryuk, CryptoLocker.
	- **Cryptojackers**: hijack system resources to mine crypto without user consent
	- **Advanced Persistent Threats**: sophisticated, focus on stealing data over long period. Often state sponsored and use multiple attack vectors to maintain persistence. eg. Stuxnet, Duqu, Flame, APT29 (Cozy Bear).
- Protection Strategies:
	- Use updated antivirus and anti malware software.
	- Keep operating systems and applicatin patched.
	- Implement strong access controls and authentication.
	- Use firewalls and intrusion detection systems
	- Monitor system behavior and network traffic
	- Maintain regular backups of critical data.
	- Train users on security awareness and best practices.
## # Malware Explained: How Hackers Attack (Ransomware, Spyware & More!) (Business Courses, 18 May 2025)

- Malware primary actions are SLIDE: 
	- ==Snoop==: eg spyware. logs password, browsing history.
	- ==Launch==: eg trojan. disguised as legit software to attack.
	- ==Imprison==: eg ransomware. locks your files for ransom.
	- ==Deceive==: eg adware. floods you with fake "virus" pop-ups.
	- ==Evade==: eg rootkits. hides deep in your system.
- How to protect self:
	- Update everything (OS, apps, firmware).
	- Use reputable antivirus (and keep it updated).
	- Don't click sketchy links/attachments.
	- Backup your data (so ransomware can't blackmail you).
## What is firewall? | Firewall explained | Firewalls and network security (Simplilearn, 2021)
- Firewall is a security device that filters incoming and outgoing traffic in a private network.
	- Packet filtering firewall, eg stateful inspection firewall (dynamic packet filtering firewalls)
	- Proxy firewall (application level gateway)