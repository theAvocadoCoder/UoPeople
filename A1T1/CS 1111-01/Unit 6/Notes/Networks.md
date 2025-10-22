## Computer Systems Application (Borodin, 2024)
A network is a set of interconnected devices (nodes) which are used to transmit data between them with agreed protocols.

The key distinction between a computer network and a distributed system is that in a distributed system, a collection of independent computers appears to its users as a single coherent system. A well-known example of this is the world wide web (WWW).

WWW should not be confused with the internet, which is a computer network (possibly the largest computer network). WWW is a distributed hypertext information system that is built on the internet and runs on it.

> Computer networking as we know it today may be said to have gotten its start with the Arpanet development in the late 1960s and early 1970s. Prior to that time there were computer vendor "networks" designed primarily to connect terminals and remote job entry stations to a mainframe.

Most networks use distributed processing, in which a task is divided among multiple computers (usually personal computers or workstations) to handle subsets of the task. 

### Network Prerequisites
The three most crucial are ==safety==, ==dependability==, and ==effectiveness==.

#### Execution (Effectiveness)
- **Transit time**: duration of time needed for a signal to transfer from one machine to another
- **Response time**: time that passes between receipt of a signal (request) and the reaction to that receipt
- **Throughput** and **Delay**: measures for progress. Network performance may be influenced by number of customers, type of data transmission, capabilities of the linked equipment, and quality of software.
- **Fewer interruptions** and increased **bandwidth**: Bandwidth is the maximum rate of data transfer across a given path. Users may boost bandwidth by sending more data via the network, but the lag will increase as a result of traffic overcrowding.
#### Reliability (Dependability)
Delivery precision is influenced by the ==number of inadequacies==, the ==pace== at which a ==connection== can be ==restored after a collapse==, and the system's ==adaptability to major disasters==.

#### Safety
The safeguarding of information from unauthorized exposure, the protection of lost data and advancement, and the establishment of policies and procedures for recovering data from intrusions are all concerns related to network security.

### Physical Structures
#### Connection Type
A connection is a communication medium that allows the transfer of data between two devices linked together in a network.
##### Point-to-Point
- Dedicated link between two devices
- Data transfer only permitted at the link's highest output.
- Usually involves physical wires and cables, but may also include microwave or satellite links.
##### Multi-point
- AKA multi-drop connection.
- Distinct devices using the same channel.
- Channel's ability is shared geographically/spatially or temporally in the multi-point surroundings.
#### Physical Topology
> Topology is concerned with the properties of a geometric object that are preserved under continuous deformations, such as stretching, twisting, crumpling, and bending; that is, without closing holes, opening holes, tearing, gluing, or passing through itself.

A connection may have one or more devices. A (physical) topology may be made up of two or more connections.

The spatial depiction of topology demonstrates how each connection and node (connecting element) connects to each other.

Four fundamental topologies are: ==ring==, ==bus==, ==star==, and ==mesh==.

##### Mesh
- Each device connected to another has a unique point-to-point connection.
- Each node is linked to n-1 nodes.
- n(n-1) physical links are needed.
###### Pros
- Support for own collected data; exterminating traffic issues arising from shared links between multiple gadgets.
- Reliability. The system is not rendered useless if just one connection breaks.
- Confidentiality & safety. Only intended receiver can see a message due to physical restrictions and direct line.
- Failure isolation and fault diagnosis are made simple by point-to-point connections. Traffic can be detoured, avoiding connections with issues.
###### Cons
- Largely linked to the amount of wiring and I/O access points needed.
- Interdependence makes setup and reconnection demanding.
- Physical location may not be able to support the setup (not enough space).
- I/O ports and cables required may cost impossible sums.
- Because of the cons, mesh topology is typically only partially implemented, and often in hybrid networks.
##### Star
- Each device has a dedicated ptp link to a central controller known as a hub.
- No direct traffic between devices, rather the controller acts as an exchange, relaying data between connected devices.
###### Pros
- Less expensive than mesh topology. Each device needs only one link and I/O port to connect to all others.
- Easy to install and reconfigure. Far less cabling to be housed; additions, moves, and deletions involve only one connection: device-hub.
- Robustness. Link failure is exclusive; other links remain active.
- Fault identification and isolation. As long as the hub functions, faulty links can be monitored and bypassed.
###### Cons
- Dependency on a single point. The entire system depends on the hub; if it goes down, the whole system is dead.
- Requires more cabling than other topologies besides mesh.
It is often used in local-area networks (LANs), especially high-speed ones.

##### Bus
- Multipoint connection, as opposed to mesh and star which are ptp.
- One long cable acts as a backbone to link all devices.
- Nodes are connected via drop lines (connections between device and main cable) and taps (connectors that splice into main cable or puncture sheathing to make contact with metallic core).
- The signal travelling along the backbone gets its energy transformed into heat, becoming weaker the farther it travels.
- Therefore, there is a limit to the number of taps supported on a bus and the distance between each tap.
###### Pros
- Ease of installation. Backbone is laid along the most efficient path, with drop lines of various lengths connecting nodes to it.
- Uses less cabling than mesh or star topologies
###### Cons
- Difficult reconnection and fault isolation. It is designed for optimally efficient installation, but is difficult when adding new devices.
- Signal reflection at taps can cause degradation in quality. Limiting the number and spacing of connected devices controls this. Adding new devices requires modification or replacement of the backbone.
- A fault or break in the bus cable stops all transmission.
Bus topology was one of the first used in the design of early LANs. Ethernet LANs can use bus topology, but they are less popular now for reasons.

##### Ring
- Each device has a dedicated ptp connection with only the two devices on either side of it.
- Signal passes along the ring in one direction, through devices, till it reaches its destination.
- Each device incorporates a repeater. This regenerates bits of a received signal intended for another device, and passes them along.
- Each device is (physically or logically) linked to only its immediate neighbors.
###### Pros
- Relatively easy to install and reconfigure.
- Device addition or deletion requires changing only two connections. The only constraints are media and traffic considerations (max ring length & number of devices).
- Fault isolation is simplified. Because signal is circulating at all times, if a device does not receive a signal within a specified period, it can issue an alarm. This aids problems detection and location.
###### Cons
- Unidirectional traffic can be a disadvantage; a break in the ring (e.g., a disabled station) can disable the entire network. This can be solved using a dual ring or a switch capable of closing off the break.
##### Hybrid
- Utilizing more than one of the main four topologies.
### Categories of Networks
Primarily LAN, normally covering an area <= 2 miles; WAN, as large as worldwide; and MAN, often tens of miles and lie between LAN and WAN.

#### LAN
- Usually privately owned and links the devices in a single office, building or campus.
- Currently limited in size to a few kilometers.
- Designed to allow resources (hardware, software or data) to be shared between personal computers or workstations.
- Generally use only one type of transmission medium.
- Most common topologies are bus, ring, and star.
- Early versions had data rates in a range of 4 - 16 Mbps.
#### WAN
- Provides long-distance transmission over large geographic areas. May transmit data, image, audio, and video information. Areas may comprise a country, continent, or even the whole world.
- The dial-up line that connects a home computer to the internet is a ptp WAN.
- The Internet is a switched WAN. It connects end systems, usually comprising of a router (internetworking connecting device) that connects to another LAN or WAN.
- Asynchronous transfer mode network has fixed-size data unit packets called cells and is also a  switched WAN.
#### MAN
- Size between LAN and WAN. Covers the area inside a town or city. Designed for customers who need high-speed connectivity, normally to the Internet, and have endpoints spread over a city or part of a city. Example is cable TV.