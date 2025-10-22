**Understanding Network Types and Topologies**

In the 21st century, much of human activity and interaction is facilitated by networks; from simple telephone conversations to updating store inventories or processing bank transfers. Networks are categorized by the area they cover:
- A **local area network (LAN)** is typically limited to a few kilometers (Borodin, 2024) and is often used in a single office or building.
- A **metropolitan area network (MAN)** spans tens of miles and may cover a town or city. A good example is cable TV. A MAN may also connect multiple LANs.
- **Wide area networks (WANs)** can span entire countries or the globe. The most popular WAN is the internet, which often contains LANs and MANs.

For the average user, a LAN is the go-to network type. It is cheaper and more versatile than the other two categories, making it ideal for individuals or small businesses with one location.

Beyond network categories, it is also important to consider network topology; the pattern in which devices are interconnected (Simplilearn, 2022).

Borodin (2024) lists four fundamental topologies and a hybrid topology combining any of them.

In a **mesh topology**, each node connects point-to-point with others. It is reliable, confidential, and easy to diagnose but costly and difficult to set up or reconfigure due to wiring and interdependence.

The **star topology** links all nodes to a central hub, avoiding mesh’s complexity while providing the same benefits at lower cost. However, dependence on a single hub can affect availability when that hub fails.

The **bus topology** uses a shared channel called the backbone. It’s easy to install and uses less cabling but is harder to reconfigure and also suffers from single-point failure.

The **ring topology** connects devices in a loop, each linked to two neighbors. It’s easy to install and isolate faults but a failed station can disable the entire network.

Common LAN topologies include bus, ring, star, or tree, which combines bus and star to be more efficient (Simplilearn, 2022).

**Role of Connecting Devices**

Connecting devices enable the smooth functioning of communication systems within a network (WhiteboardDoodles, 2024). Each device plays a specific role and is an essential component.

These devices operate on various layers of the Open Systems Interconnection (OSI) model, carrying out essential tasks like directing data packets to appropriate destinations (i.e., the router), processing and forwarding data (i.e., the switch and the hub), connecting LAN to internet via signal conversion (i.e., the modem), expanding or amplifying network (i.e., the access point and the repeater), connecting networks and network segments (i.e., the gateway and the bridge), managing traffic (i.e., the load balancer), and securing the network's entrypoint (i.e., the firewall).

**Transmission Modes and Practical Scenarios**

Data exchange over a network can be through a wired or wireless medium (ALL ABOUT ELECTRONICS, 2024). The data can flow one-way (unidirectional) or two-way (bidirectional). Based on this, there are three transmission modes: simplex, half-duplex, and full-duplex. 

In simplex communication, data flow is unidirectional with one device acting as a transmitter, and the other, a receiver. A great example is radio broadcasting, in which audio data is sent by the transmitter in the form of electromagnetic waves and then picked up by receiver antennae (Samim Group, 2024).

Half-Duplex communication is a bidirectional mode in which data may only flow in a given direction at a time. This mode is seen in walkie talkies, which carry audio data over a frequency one at a time.

Full-Duplex communication allows for simultaneous data flow in both directions. There are two approaches to this:
- Frequency division duplexing; where different frequencies are used such as in satelites.
- Time division duplexing; where multiple short time slots are assigned to each direction, depending on the size of data being transferred. Examples of this include Wi-Fi and cellular network.

**References**

1. ALL ABOUT ELECTRONICS. (2024, April 8). _Simplex, Half-Duplex and Full-Duplex Communication | Transmission modes in communication system_ [Video]. YouTube. https://youtu.be/RzAXEQ4XsSI/
2. Borodin, V. (Ed.). (2024). _Computer systems application_. Toronto Academic Press. ProQuest Ebook Central.
3. Samim Group. (2024, August 19). _How Radio Broadcasting Works_. https://www.samimgroup.com/blog/about-radio-broadcasting/
4. WhiteboardDoodles. (2024, October 27). _Network devices explained: Routers, switches, hubs & more | Networking Basics_ [Video]. YouTube. https://youtu.be/MXr_cyY0BVc/
5. Simplilearn. (2022, February 4). _What is network topology? | Types of network topology | BUS, RING, STAR, TREE, MESH | Simplilearn_ [Video]. YouTube. https://youtu.be/QGykYWbdf0A/

Word Count (minus question): 738 words.

Question: The various topologies all have their strengths and drawbacks, as well as situations where they are best applied. Is it safe to say that most common networks require a hybrid topology to better highlight strengths and compensate for drawbacks?

