
   

> 
> # Computer Network Architecture

Computer Network Architecture is defined as the physical and logical design of the software, hardware, protocols, and media of the transmission of data. Simply we can say that how computers are organized and how tasks are allocated to the computer.

**The two types of network architectures are used:**

![Computer Network Architecture](https://static.javatpoint.com/tutorial/computer-network/images/computer-network-architecture.png)

-   Peer-To-Peer network
-   Client/Server network

----------

## Peer-To-Peer network

-   Peer-To-Peer network is a network in which all the computers are linked together with equal privilege and responsibilities for processing the data.
-   Peer-To-Peer network is useful for small environments, usually up to 10 computers.
-   Peer-To-Peer network has no dedicated server.
-   Special permissions are assigned to each computer for sharing the resources, but this can lead to a problem if the computer with the resource is down.

![Computer Network Architecture](https://static.javatpoint.com/tutorial/computer-network/images/peer-to-peer-network.png)

### Advantages Of Peer-To-Peer Network:

-   It is less costly as it does not contain any dedicated server.
-   If one computer stops working but, other computers will not stop working.
-   It is easy to set up and maintain as each computer manages itself.

### Disadvantages Of Peer-To-Peer Network:

-   In the case of Peer-To-Peer network, it does not contain the centralized system . Therefore, it cannot back up the data as the data is different in different locations.
-   It has a security issue as the device is managed itself.

----------

## Client/Server Network

-   Client/Server network is a network model designed for the end users called clients, to access the resources such as songs, video, etc. from a central computer known as Server.
-   The central controller is known as a  **server**  while all other computers in the network are called  **clients**.
-   A server performs all the major operations such as security and network management.
-   A server is responsible for managing all the resources such as files, directories, printer, etc.
-   All the clients communicate with each other through a server. For example, if client1 wants to send some data to client 2, then it first sends the request to the server for the permission. The server sends the response to the client 1 to initiate its communication with the client 2.

![Computer Network Architecture](https://static.javatpoint.com/tutorial/computer-network/images/client-server-network.png)

### Advantages Of Client/Server network:

-   A Client/Server network contains the centralized system. Therefore we can back up the data easily.
-   A Client/Server network has a dedicated server that improves the overall performance of the whole system.
-   Security is better in Client/Server network as a single server administers the shared resources.
-   It also increases the speed of the sharing resources.

### Disadvantages Of Client/Server network:

-   Client/Server network is expensive as it requires the server with large memory.
-   A server has a Network Operating System(NOS) to provide the resources to the clients, but the cost of NOS is very high.
-   It requires a dedicated network administrator to manage all the resources.

# OSI Model – Layers of OSI Model


**OSI stands for Open Systems Interconnection**. It was developed by ISO – ‘International Organization for Standardization’, in the year 1984. It is a 7-layer architecture with each layer having specific functionality to perform. All these 7 layers work collaboratively to transmit the data from one person to another across the globe.

> Prerequisite:  [Basics of Computer Networking](https://www.geeksforgeeks.org/basics-computer-networking/)

## OSI Model

The OSI model, created in 1984 by ISO, is a reference framework that explains the process of transmitting data between computers. It is divided into seven layers that work together to carry out specialised network functions, allowing for a more systematic approach to networking.

![OSI Model](https://media.geeksforgeeks.org/wp-content/uploads/20210220204638/cn1.png)

## The 7 layers of the OSI Model?

The OSI model consists of seven abstraction layers arranged in a top-down order:

1.  [Physical Layer](https://www.geeksforgeeks.org/physical-layer-in-osi-model/)
2.  [Data Link Layer](https://www.geeksforgeeks.org/data-link-layer/)
3.  [Network Layer](https://www.geeksforgeeks.org/network-layer-services-packetizing-routing-and-forwarding/)
4.  [Transport Layer](https://www.geeksforgeeks.org/transport-layer-responsibilities/)
5.  [Session Layer](https://www.geeksforgeeks.org/session-layer-in-osi-model/)
6.  [Presentation Layer](https://www.geeksforgeeks.org/presentation-layer-in-osi-model/)
7.  [Application Layer](https://www.geeksforgeeks.org/application-layer-in-osi-model/)

## **Physical Layer – Layer 1**

The lowest layer of the OSI reference model is the physical layer. It is responsible for the actual physical connection between the devices. The physical layer contains information in the form of **bits.**  It is responsible for transmitting individual bits from one node to the next. When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together.

![Data Bits in the Physical Layer](https://media.geeksforgeeks.org/wp-content/uploads/20230405124830/data-bits.jpg)

### Functions of the Physical Layer

-   **Bit synchronization:**  The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at the bit level.
-   **Bit rate control:**  The Physical layer also defines the transmission rate i.e. the number of bits sent per second.
-   **Physical topologies:**  Physical layer specifies how the different, devices/nodes are arranged in a network i.e. bus, star, or mesh topology.
-   **Transmission mode:**  Physical layer also defines how the data flows between the two connected devices. The various transmission modes possible are Simplex, half-duplex and full-duplex.

> **Note:**
> 
> 1.  Hub, Repeater, Modem, and Cables are Physical Layer devices.
> 2.  Network Layer, Data Link Layer, and Physical Layer are also known as  **Lower Layers**  or  **Hardware Layers**.

## **Data Link Layer (DLL) – Layer 2**

The data link layer is responsible for the node-to-node delivery of the message. The main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer. When a packet arrives in a network, it is the responsibility of the DLL to transmit it to the Host using its MAC address.  
The Data Link Layer is divided into two sublayers:

1.  [Logical Link Control (LLC)](https://www.geeksforgeeks.org/logical-link-control-llc-protocol-data-unit/)
2.  [Media Access Control (MAC)](https://www.geeksforgeeks.org/introduction-of-mac-address-in-computer-network/)

The packet received from the Network layer is further divided into frames depending on the frame size of the NIC(Network Interface Card). DLL also encapsulates Sender and Receiver’s MAC address in the header.

The Receiver’s MAC address is obtained by placing an  [ARP(Address Resolution Protocol)](https://www.geeksforgeeks.org/how-address-resolution-protocol-arp-works/) request onto the wire asking “Who has that IP address?” and the destination host will reply with its MAC address.

### Functions of the Data Link Layer

-   **Framing:** Framing is a function of the data link layer. It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.
-   **Physical addressing:**  After creating frames, the Data link layer adds physical addresses (MAC addresses) of the sender and/or receiver in the header of each frame.
-   **Error control:**  The data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.
-   **Flow Control:**  The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving an acknowledgment.
-   **Access control:** When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.

![Function of DLL](https://media.geeksforgeeks.org/wp-content/uploads/20230405130015/DatalinkLayer-660x335.jpg)

> **Note:**
> 
> 1.  Packet in the Data Link layer is referred to as  **Frame.**
> 2.  Data Link layer is handled by the NIC (Network Interface Card) and device drivers of host machines.
> 3.  Switch & Bridge are Data Link Layer devices.

## **Network Layer – Layer 3**

The network layer works for the transmission of data from one host to the other located in different networks. It also takes care of packet routing i.e. selection of the shortest path to transmit the packet, from the number of routes available. The sender & receiver’s IP addresses are placed in the header by the network layer.

### Functions of the Network Layer

-   **Routing:**  The network layer protocols determine which route is suitable from source to destination. This function of the network layer is known as routing.
-   **Logical Addressing:** To identify each device on Internetwork uniquely, the network layer defines an addressing scheme. The sender & receiver’s IP addresses are placed in the header by the network layer. Such an address distinguishes each device uniquely and universally.

> **Note:**
> 
> 1.  Segment in the Network layer is referred to as  **Packet**.
> 2.  Network layer is implemented by networking devices such as routers and switches.

## **Transport Layer – Layer 4**

The transport layer provides services to the application layer and takes services from the network layer. The data in the transport layer is referred to as  _Segments_. It is responsible for the End to End Delivery of the complete message. The transport layer also provides the acknowledgment of the successful data transmission and re-transmits the data if an error is found.

**At the sender’s side:** The transport layer receives the formatted data from the upper layers, performs  **Segmentation**, and also implements  **Flow & Error control**  to ensure proper data transmission. It also adds Source and Destination port numbers in its header and forwards the segmented data to the Network Layer.

> **Note:**  The sender needs to know the port number associated with the receiver’s application.
> 
> Generally, this destination port number is configured, either by default or manually. For example, when a web application requests a web server, it typically uses port number 80, because this is the default port assigned to web applications. Many applications have default ports assigned.
> 
> **At the receiver’s side:** Transport Layer reads the port number from its header and forwards the Data which it has received to the respective application. It also performs sequencing and reassembling of the segmented data.

### Functions of the Transport Layer

-   **Segmentation and Reassembly:**  This layer accepts the message from the (session) layer, and breaks the message into smaller units. Each of the segments produced has a header associated with it. The transport layer at the destination station reassembles the message.
-   **Service Point Addressing:**  To deliver the message to the correct process, the transport layer header includes a type of address called service point address or port address. Thus by specifying this address, the transport layer makes sure that the message is delivered to the correct process.

#### Services Provided by Transport Layer

1.  [Connection-Oriented Service](https://www.geeksforgeeks.org/connection-oriented-service/)
2.  [Connectionless Service](https://www.geeksforgeeks.org/connection-less-service/)

**1. Connection-Oriented Service:**  It is a three-phase process that includes

-   Connection Establishment
-   Data Transfer
-   Termination/disconnection

In this type of transmission, the receiving device sends an acknowledgment, back to the source after a packet or group of packets is received. This type of transmission is reliable and secure.

**2. Connectionless service:**  It is a one-phase process and includes Data Transfer. In this type of transmission, the receiver does not acknowledge receipt of a packet. This approach allows for much faster communication between devices. Connection-oriented service is more reliable than connectionless Service.

> **Note:**
> 
> 1.  Data in the Transport Layer is called  **Segments**.
> 2.  Transport layer is operated by the Operating System. It is a part of the OS and communicates with the Application Layer by making system calls.
> 3.  The transport layer is called as  **Heart of the OSI**  model.
> 4.  **Device or Protocol Use :**  TCP, UDP NetBIOS, PPTP

## **Session Layer – Layer 5**

This layer is responsible for the establishment of connection, maintenance of sessions, and authentication, and also ensures security.

### Functions of the Session Layer

-   **Session establishment, maintenance, and termination:**  The layer allows the two processes to establish, use and terminate a connection.
-   **Synchronization:**  This layer allows a process to add checkpoints that are considered synchronization points in the data. These synchronization points help to identify the error so that the data is re-synchronized properly, and ends of the messages are not cut prematurely and data loss is avoided.
-   **Dialog Controller:**  The session layer allows two systems to start communication with each other in half-duplex or full-duplex.

> **Note:**
> 
> 1.  All the below 3 layers(including Session Layer) are integrated as a single layer in the TCP/IP model as the ????pplication Layer”.
> 2.  Implementation of these 3 layers is done by the network application itself. These are also known as  **Upper Layers or**  **Software Layers.**
> 3.  **Device or Protocol Use :**  NetBIOS, PPTP.

**for Example:-**

Let us consider a scenario where a user wants to send a message through some Messenger application running in his browser. The “Messenger” here acts as the application layer which provides the user with an interface to create the data. This message or so-called Data is compressed, encrypted (if any secure data), and converted into bits (0’s and 1’s) so that it can be transmitted.

![Communication in Session Layer](https://media.geeksforgeeks.org/wp-content/uploads/20230405124947/communication.jpg)

Communication in Session Layer

## **Presentation Layer – Layer 6**

The presentation layer is also called the  **Translation layer**. The data from the application layer is extracted here and manipulated as per the required format to transmit over the network.

### Functions of the Presentation Layer

-   **Translation:**  For example, ASCII to EBCDIC.
-   **Encryption/ Decryption:**  Data encryption translates the data into another form or code. The encrypted data is known as the ciphertext and the decrypted data is known as plain text. A key value is used for encrypting as well as decrypting data.
-   **Compression:**  Reduces the number of bits that need to be transmitted on the network.

Note:  **Device or Protocol Use :**  JPEG, MPEG, GIF

## **Application Layer – Layer 7**

At the very top of the OSI Reference Model stack of layers, we find the Application layer which is implemented by the network applications. These applications produce the data, which has to be transferred over the network. This layer also serves as a window for the application services to access the network and for displaying the received information to the user.

**Example**: Application – Browsers, Skype Messenger, etc.

> **Note:**  1. The application Layer is also called Desktop Layer.
> 
> 2. **Device or Protocol Use :**  SMTP

### Functions of the Application Layer

The main functions of application layer are given below.

-   Network Virtual Terminal: It allows a user to log on to a remote host.
-   FTAM- File transfer access and management : This application allows a user to  
    access file in a remote host, retrieve files in remote host and manage or  
    control files from a remote computer.
-   Mail Services : Provide email service.
-   Directory Services : This application provides distributed database sources  
    and access for global information about various objects and services.

># The TCP/IP Reference Model

[TCP/IP](https://www.tutorialspoint.com/tcp-ip-in-computer-networking)  Reference Model is a four-layered suite of communication protocols. It was developed by the DoD (Department of Defence) in the 1960s. It is named after the two main protocols that are used in the model, namely, TCP and IP.  **TCP**  stands for "**Transmission Control Protocol**" and  **IP**  stands for "**Internet Protocol**".

The four layers in the TCP/IP protocol suite are −

1.  **Host-to- Network Layer −**It is the lowest layer that is concerned with the physical transmission of data. TCP/IP does not specifically define any protocol here but supports all the standard protocols.
2.  **Internet Layer −**It defines the protocols for logical transmission of data over the network. The main protocol in this layer is  [Internet Protocol (IP)](https://www.tutorialspoint.com/internet_technologies/internet_protocols.htm)  and it is supported by the protocols  [ICMP](https://www.tutorialspoint.com/what-is-icmp-protocol),  [IGMP](https://www.tutorialspoint.com/what-is-igmp-in-the-computer-network),  [RARP](https://www.tutorialspoint.com/what-is-reverse-address-resolution-protocol-rarp), and  [ARP](https://www.tutorialspoint.com/what-is-address-resolution-protocol-arp).
3.  **Transport Layer −**  It is responsible for error-free end-to-end delivery of data. The protocols defined here are Transmission Control Protocol (TCP) and  [User Datagram Protocol (UDP)](https://www.tutorialspoint.com/data_communication_computer_network/user_datagram_protocol.htm).
4.  **Application Layer −**  This is the topmost layer and defines the interface of host programs with the transport layer services. This layer includes all high-level protocols like  [Telnet](https://www.tutorialspoint.com/introduction-to-telnet),  [DNS](https://www.tutorialspoint.com/what-is-a-domain-name-system),  [HTTP](https://www.tutorialspoint.com/http/http_overview.htm),  [FTP](https://www.tutorialspoint.com/what-is-ftp),  [SMTP](https://www.tutorialspoint.com/what-is-smtp), etc.

The following diagram shows the layers and the protocols in each of the layers −

![](https://www.tutorialspoint.com/assets/questions/images/30037-1531479425.png)

[  
# Difference between OSI and TCP/IP Reference Model


| Feature                                        | OSI                                   | TCP/IP                                            |
|-----------------------------------------------|---------------------------------------|---------------------------------------------------|
| Representation                                | Open System Interconnection (OSI)     | Transmission Control Protocol/Internet Protocol  |
| Independence                                  | Generic, protocol independent         | Depends on standard protocols                       |
| Development                                   | Model first, protocols created later  | Protocols first, then built the model               |
| Quality of Services                           | Provides quality services             | Does not provide quality services                  |
| Administration and Conventions                | Defines administration, interfaces, and conventions | Does not mention services, interfaces, and protocols |
| Protocol Visibility                           | Protocols are hidden and can be replaced easily | Protocols are not hidden and cannot be easily replaced |
| Complexity                                    | More complex than TCP/IP              | Simpler than OSI                                   |
| Connection Types in Network Layer             | Both connection and connectionless oriented transmission | Connectionless transmission                        |
| Connection Types in Transport Layer           | Connection-oriented transmission      | Supports both connection and connectionless-oriented transmission |
| Approach                                      | Vertical                              | Horizontal                                        |
| Header Size (Minimum)                         | 5 bytes                               | 20 bytes                                          |
| Protocol Handling                             | Protocols may be unknown and replaced as technology evolves | Returning protocol is not difficult                |


![](https://www.tutorialspoint.com/assets/questions/media/51877/reference_model.jpg)


# Design Issues

In the code generation phase, various issues can arises:

1.  Input to the code generator
2.  Target program
3.  Memory management
4.  Instruction selection
5.  Register allocation
6.  Evaluation order

## 1. Input to the code generator

-   The input to the code generator contains the intermediate representation of the source program and the information of the symbol table. The source program is produced by the front end.
-   Intermediate representation has the several choices:  
    a) Postfix notation  
    b) Syntax tree  
    c) Three address code
-   We assume front end produces low-level intermediate representation i.e. values of names in it can directly manipulated by the machine instructions.
-   The code generation phase needs complete error-free intermediate code as an input requires.

## 2. Target program:

The target program is the output of the code generator. The output can be:

a)  **Assembly language:**  It allows subprogram to be separately compiled.

b)  **Relocatable machine language:**  It makes the process of code generation easier.

c)  **Absolute machine language:**  It can be placed in a fixed location in memory and can be executed immediately.

## 3. Memory management

-   During code generation process the symbol table entries have to be mapped to actual p addresses and levels have to be mapped to instruction address.
-   Mapping name in the source program to address of data is co-operating done by the front end and code generator.
-   Local variables are stack allocation in the activation record while global variables are in static area.

## 4. Instruction selection:

-   Nature of instruction set of the target machine should be complete and uniform.
-   When you consider the efficiency of target machine then the instruction speed and machine idioms are important factors.
-   The quality of the generated code can be determined by its speed and size.

### Example:

The Three address code is:

1.  a:= b + c
2.  d:= a + e

Inefficient assembly code is:

1.  MOV b, R0 R0→b
2.  ADD c, R0 R0 c + R0
3.  MOV R0, a a → R0
4.  MOV a, R0 R0→ a
5.  ADD e, R0 R0 → e + R0
6.  MOV R0, d d → R0

## 5. Register allocation

Register can be accessed faster than memory. The instructions involving operands in register are shorter and faster than those involving in memory operand.

The following sub problems arise when we use registers:

**Register allocation:**  In register allocation, we select the set of variables that will reside in register.

**Register assignment:**  In Register assignment, we pick the register that contains variable.

Certain machine requires even-odd pairs of registers for some operands and result.

### For example:

Consider the following division instruction of the form:

1.  D x, y

Where,

**x**  is the dividend even register in even/odd register pair

**y**  is the divisor

**Even register**  is used to hold the reminder.

**Old register**  is used to hold the quotient.

## 6. Evaluation order

The efficiency of the target code can be affected by the order in which the computations are performed. Some computation orders need fewer registers to hold results of intermediate than others.


# Switching Techniques

In large networks, there may be more than one paths for transmitting data from  **sender**  to receiver. Selecting a path that data must take out of the available options is called  **switching**. There are two popular switching techniques – circuit switching and packet switching.

![Switching](https://www.tutorialspoint.com/communication_technologies/images/switching.jpg)

## Circuit Switching

When a dedicated path is established for data transmission between sender and receiver, it is called circuit switching. When any network node wants to send data, be it audio, video, text or any other type of information, a  **call request signal**  is sent to the receiver and acknowledged back to ensure availability of dedicated path. This dedicated path is then used to send data. ARPANET used circuit switching for communication over the network.

### Advantages of Circuit Switching

Circuit switching provides these advantages over other switching techniques −

-   Once path is set up, the only delay is in data transmission speed
-   No problem of congestion or garbled message

### Disadvantages of Circuit Switching

Circuit switching has its disadvantages too −

-   Long set up time is required
    
-   A request token must travel to the receiver and then acknowledged before any transmission can happen
    
-   Line may be held up for a long time
    

## Packet Switching

As we discussed, the major problem with circuit switching is that it needs a dedicated line for transmission. In packet switching, data is broken down into small packets with each packet having source and destination addresses, travelling from one router to the next router.


# Connection-Oriented and Connectionless Service

Data communication is a telecommunication network to send and receive data between two or more computers over the same or different network. There are two ways to establish a connection before sending data from one device to another, that are  **Connection-Oriented**  and  **Connectionless Service**. Connection-oriented service involves the creation and termination of the connection for sending the data between two or more devices. In contrast, connectionless service does not require establishing any connection and termination process for transferring the data over a network.

## Connection-Oriented Service

A connection-oriented service is a network service that was designed and developed after the telephone system. A connection-oriented service is used to create an end to end connection between the sender and the receiver before transmitting the data over the same or different networks. In connection-oriented service, packets are transmitted to the receiver in the same order the sender has sent them. It uses a handshake method that creates a connection between the user and sender for transmitting the data over the network. Hence it is also known as a reliable network service.

![Connection-Oriented vs Connectionless Service](https://static.javatpoint.com/tutorial/computer-network/images/connection-oriented-vs-connectionless-service.png)

Suppose, a sender wants to send data to the receiver. Then, first, the sender sends a request packet to a receiver in the form of an  **SYN**  packet. After that, the receiver responds to the sender's request with an (SYN-ACK) signal/packets. That represents the confirmation is received by the receiver to start the communication between the sender and the receiver. Now a sender can send the message or data to the receiver.

Similarly, a receiver can respond or send the data to the sender in the form of packets. After successfully exchanging or transmitting data, a sender can terminate the connection by sending a signal to the receiver. In this way, we can say that it is a reliable network service.

### TCP

[TCP (Transmission Control Protocol)](https://www.javatpoint.com/tcp)  is a connection-oriented protocol that allows communication between two or more computer devices by establishing connections in the same or different networks. It is the most important protocol that uses  **internet protocol**  to transfer the data from one end to another. Hence, it is sometimes referred to as TCP/IP. It ensures that the connection is established and maintained until the data packet is transferring between the sender and receiver is complete.

## Connectionless Service

A connection is similar to a  **postal system**, in which each letter takes along different route paths from the source to the destination address. Connectionless service is used in the network system to transfer data from one end to another end without creating any connection. So it does not require establishing a connection before sending the data from the sender to the receiver. It is not a reliable network service because it does not guarantee the transfer of data packets to the receiver, and data packets can be received in any order to the receiver. Therefore we can say that the data packet does not follow a  **defined**  path. In connectionless service, the transmitted data packet is not received by the receiver due to network congestion, and the data may be lost.

![Connection-Oriented vs Connectionless Service](https://static.javatpoint.com/tutorial/computer-network/images/connection-oriented-vs-connectionless-service2.png)

For example, a sender can directly send any data to the receiver without establishing any connection because it is a connectionless service. Data sent by the sender will be in the packet or data streams containing the receiver's address. In connectionless service, the data can be travelled and received in any order. However, it does not guarantee to transfer of the packets to the right destination.

### UDP

The  [UDP (User Datagram Protocol)](https://www.javatpoint.com/udp-protocol)  is a connectionless protocol that allows communication between two or more devices without establishing any connection. In this protocol, a sender sends the data packets to the receiver that holds the destination address. A UDP does not ensure to deliver the data packets to the correct destination, and it does not generate any acknowledgment about the sender's data. Similarly, it does not acknowledge the receiver about the data. Hence, it is an unreliable protocol.

| S. No | Comparison Parameter | Connection-oriented Service                            | Connectionless Service                                        |
|-------|-----------------------|-------------------------------------------------------|----------------------------------------------------------------|
| 1.    | Related System        | Designed and developed based on the telephone system. | Service based on the postal system.                             |
| 2.    | Definition            | Used to create an end-to-end connection between the senders and receivers before transmitting data over the same or different networks. | Used to transfer data packets between senders and receivers without creating any connection. |
| 3.    | Virtual Path          | Creates a virtual path between the sender and receiver. | Does not create any virtual connection or path between the sender and receiver. |
| 4.    | Authentication        | Requires authentication before transmitting data packets to the receiver. | Does not require authentication before transferring data packets. |
| 5.    | Data Packets Path     | All data packets are received in the same order as sent by the sender. | Not all data packets are received in the same order as sent by the sender. |
| 6.    | Bandwidth Requirement | Requires higher bandwidth to transfer data packets.    | Requires low bandwidth to transfer data packets.                |
| 7.    | Data Reliability      | More reliable connection service, guarantees data packet transfer from one end to the other end with a connection. | Not a reliable connection service, does not guarantee the transfer of data packets from one end to another for establishing a connection. |
| 8.    | Congestion            | No congestion as it provides an end-to-end connection between sender and receiver during data transmission. | May be congestion due to not providing an end-to-end connection between the source and receiver for data packet transmission. |
| 9.    | Examples              | Transmission Control Protocol (TCP) is an example of a connection-oriented service. | User Datagram Protocol (UDP), Internet Protocol (IP), and Internet Control Message Protocol (ICMP) are examples of connectionless service. |


# Virtual Circuit in Computer Network


**Virtual Circuit**  is the computer network providing connection-oriented service. It is a connection-oriented network. In virtual circuit resource are reserve for the time interval of data transmission between two nodes. This network is a highly reliable medium of transfer. Virtual circuits are costly to implement.

![](https://media.geeksforgeeks.org/wp-content/uploads/20200512113141/Untitled-Diagram-166.png)

**Working of Virtual Circuit:**

-   In the first step a medium is set up between the two end nodes.
-   Resources are reserved for the transmission of packets.
-   Then a signal is sent to sender to tell the medium is set up and transmission can be started.
-   It ensures the transmission of all packets.
-   A global header is used in the first packet of the connection.
-   Whenever data is to be transmitted a new connection is set up.

**Congestion Control in Virtual Circuit:**  
Once the congestion is detected in virtual circuit network, closed-loop techniques is used. There are different approaches in this technique:

-   **No new connection –**  
    No new connections are established when the congestion is detected. This approach is used in telephone networks where no new calls are established when the exchange is overloaded.
-   **Participation of congested router invalid –**  
    Another approach to control congestion is allow all new connections but route these new connections in such a way that congested router is not part of this route.
-   **Negotiation –**  
    To negotiate different parameters between sender and receiver of the network, when the connection is established. During the set up time, host specifies the shape and volume of the traffic, quality of service and other parameters.

**Advantages of Virtual Circuit:**

1.  Packets are delivered to the receiver in the same order sent by the sender.
2.  Virtual circuit is a reliable network circuit.
3.  There is no need for overhead in each packet.
4.  Single global packet overhead is used in virtual circuit.

**Disadvantages of Virtual Circuit:**

1.  Virtual circuit is costly to implement.
2.  It provides only connection-oriented service.
3.  Always a new connection set up is required for transmission.

# Datagram Network



In a connectionless communication systems, datagram refers to the smallest unit via which data is transmitted. Datagrams are data packets which contain adequate header information so that they can be individually routed by all intermediate network switching devices to the destination. These networks are called datagram networks since communication occurs via datagrams. They exist in packet switching networks.

## Features of Datagram Networks

-   Datagram switching is done at the network layer of the communication system.
    
-   In datagram networks, each data packet or datagram is routed independently from the source to the destination even if they belong to the same message. The network treats the packet as if it exists alone.
    
-   Since the datagrams are treated as independent units, no dedicated path is fixed for data transfer. Each datagram is routed by the intermediate routers using dynamically changing routing tables. So two successive packets from the source may follow completely separate routes to reach destination.
    
-   In these networks, no prior resource allocation is done for the individual packets. This implies that no resources like buffers, processors, bandwidth, etc. are reserved before the communication commences.
    
-   In datagram networks, resources are allocated on demand on a First−Come First−Serve (FCFS) basis. When a packet arrives at a router, the packet must wait if there are other packets being processed, irrespective of its source or destination.
    
-   Datagram communication is generally guided by User Datagram Protocol or UDP.
    

The following diagram shows datagram packets being send by host H1 to host H2. The four datagram packets labelled as A, B, C and D, all belonging to same message are being routed separately via separate routes. The packets in the message arrives in the destination out of order. It is the responsibility of H2 to reorder the packets in order to retrieve the original message.

![](https://www.tutorialspoint.com/assets/questions/media/46035/host2.jpg)


# Autonomous System
**Autonomous System (AS)**  is a group of routers and networks working under a single administrative domain. It is a 16-bit value that defines the routing domain of the routers. These numbers range from 1 to 65535.  

-   **Public Autonomous System Number –**  
    These are 16-bit values that range from 1 to 64511. The service provider will provide a public AS if the customer is connected to more than one ISPs such as multihoming. A global autonomous number, which will be unique, is provided when the customer wants to propagate its BGP routes through 2 ISPs.  
    
-   **Private Autonomous system Number –**  
    Private Autonomous System Number are 16-bit values that range from 64512 to 65535. The service provider will provide a private autonomous system number to the customer when the customer wants multi-connection to a single ISP (single home or dual home network) but not to more than one ISPs. These are provided in order to conserve the autonomous system numbers.  
    
-   **Assigning of AS numbers –**  
    The Autonomous numbers are first assigned by IANA (Internet Assign Number Authority) to the respective regional registries. Further, the regional registry distributes these autonomous numbers (from the block of autonomous numbers provided by IANA) to entities within their designated area.  
    



-   Source IP address: The source is the one who is sending the data.
-   Destination IP address: The destination is a host that receives the data from the sender.
-   Header length
-   Packet length
-   TTL (Time to Live): The number of hops occurs before the packet gets discarded.
-   Transport protocol: The transport protocol used by the internet protocol, either it can be TCP or UDP.

There is a total of 14 fields exist in the IP header, and one of them is optional.

**Payload:**  Payload is the data that is to be transported.


## References

https://www.javatpoint.com/computer-network-architecture
https://www.geeksforgeeks.org/open-systems-interconnection-model-osi/
https://www.tutorialspoint.com/The-TCP-IP-Reference-Model
https://www.tutorialspoint.com/difference-between-osi-and-tcp-ip-reference-model
https://www.javatpoint.com/design-issues
https://www.tutorialspoint.com/communication_technologies/communication_technologies_switching_techniques.htm
https://www.javatpoint.com/connection-oriented-vs-connectionless-service
https://www.geeksforgeeks.org/virtual-circuit-in-computer-network/
https://www.tutorialspoint.com/datagram-network
https://www.geeksforgeeks.org/administrative-distance-ad-and-autonomous-system-as/