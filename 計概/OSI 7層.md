![]
# 第7層 應用層
---

  應用層（Application Layer）提供為應用軟體而設計的介面，以設定與另一應用軟體之間的通訊。例如：HTTP、HTTPS、FTP、Telnet、SSH、SMTP、POP3等。

---
# 第6層 表達層
---

    表達層（Presentation Layer）把數據轉換為能與接收者的系統格式相容並適合傳輸的格式。

---
# 第5層 會議層
---

    會議層（Session Layer）負責在數據傳輸中設定和維護電腦網路中兩台電腦之間的通訊連接。

---
# 第4層 傳輸層
---

    傳輸層（Transport Layer）把傳輸表頭（TH）加至數據以形成數據包。傳輸表頭包含了所使用的協定等傳送資訊。例如:傳輸控制協定（TCP）等。

# 第3層 網路層
---

    網路層（Network Layer）決定數據的路徑選擇和轉寄，將網路表頭（NH）加至數據包，以形成封包。網路表頭包含了網路資料。例如:網際網路協定（IP）等。
---

# 第2層 資料連結層
---

    資料連結層（Data Link Layer）負責網路尋址、錯誤偵測和改錯。當表頭和表尾被加至數據包時，會形成資訊框（Data Frame）。數據連結串列頭（DLH）是包含了實體位址和錯誤偵測及改錯的方法。數據連結串列尾（DLT）是一串指示數據包末端的字串。例如乙太網、無線區域網路（Wi-Fi）和通用分組無線服務（GPRS）等。

    分為兩個子層：邏輯鏈路控制（logical link control，LLC）子層和媒介存取控制（Media access control，MAC）子層。
    
---
# 第1層 實體層

---

    實體層（Physical Layer）在局部區域網路上傳送資料框（Data Frame），它負責管理電腦通訊裝置和網路媒體之間的互通。包括了針腳、電壓、線纜規範、集線器、中繼器、網卡、主機介面卡等。

---


原文版

# Layer 7: Application Layer(應用層)
---

    The application layer is the OSI layer closest to the end user, which means both the OSI application layer and the user interact directly with the software application. This layer interacts with software applications that implement a communicating component. Such application programs fall outside the scope of the OSI model. Application-layer functions typically include identifying communication partners, determining resource availability, and synchronizing communication. When identifying communication partners, the application layer determines the identity and availability of communication partners for an application with data to transmit. The most important distinction in the application layer is the distinction between the application-entity and the application. For example, a reservation website might have two application-entities: one using HTTP to communicate with its users, and one for a remote database protocol to record reservations. Neither of these protocols have anything to do with reservations. That logic is in the application itself. The application layer has no means to determine the availability of resources in the network.

---
# Layer 6: Presentation Layer(表達層)
---

    The presentation layer establishes context between application-layer entities, in which the application-layer entities may use different syntax and semantics if the presentation service provides a mapping between them. If a mapping is available, presentation protocol data units are encapsulated into session protocol data units and passed down the protocol stack.

    This layer provides independence from data representation by translating between application and network formats. The presentation layer transforms data into the form that the application accepts. This layer formats data to be sent across a network. It is sometimes called the syntax layer.[23] The presentation layer can include compression functions.[24] The Presentation Layer negotiates the Transfer Syntax.

    The original presentation structure used the Basic Encoding Rules of Abstract Syntax Notation One (ASN.1), with capabilities such as converting an EBCDIC-coded text file to an ASCII-coded file, or serialization of objects and other data structures from and to XML. ASN.1 effectively makes an application protocol invariant with respect to syntax.

---
# Layer 5: Session Layer(會議層)
---

    The session layer controls the dialogues (connections) between computers. It establishes, manages and terminates the connections between the local and remote application. It provides for full-duplex, half-duplex, or simplex operation, and establishes procedures for checkpointing, suspending, restarting, and terminating a session. In the OSI model, this layer is responsible for gracefully closing a session, which is handled in the Transmission Control Protocol at the transport layer in the Internet Protocol Suite. This layer is also responsible for session checkpointing and recovery, which is not usually used in the Internet Protocol Suite. The session layer is commonly implemented explicitly in application environments that use remote procedure calls.

---
# Layer 4: Transport Layer(傳輸層)
---

    The transport layer provides the functional and procedural means of transferring variable-length data sequences from a source to a destination host, while maintaining the quality of service functions.

    The transport layer controls the reliability of a given link through flow control, segmentation/desegmentation, and error control. Some protocols are state- and connection-oriented. This means that the transport layer can keep track of the segments and retransmit those that fail delivery. The transport layer also provides the acknowledgement of the successful data transmission and sends the next data if no errors occurred. The transport layer creates segments out of the message received from the application layer. Segmentation is the process of dividing a long message into smaller messages.

    OSI defines five classes of connection-mode transport protocols ranging from class 0 (which is also known as TP0 and provides the fewest features) to class 4 (TP4, designed for less reliable networks, similar to the Internet). Class 0 contains no error recovery and was designed for use on network layers that provide error-free connections. Class 4 is closest to TCP, although TCP contains functions, such as the graceful close, which OSI assigns to the session layer. Also, all OSI TP connection-mode protocol classes provide expedited data and preservation of record boundaries. Detailed characteristics of TP0-4 classes are shown in the following table:[22]


    An easy way to visualize the transport layer is to compare it with a post office, which deals with the dispatch and classification of mail and parcels sent. A post office inspects only the outer envelope of mail to determine its delivery. Higher layers may have the equivalent of double envelopes, such as cryptographic presentation services that can be read by the addressee only. Roughly speaking, tunnelling protocols operate at the transport layer, such as carrying non-IP protocols such as IBM's SNA or Novell's IPX over an IP network, or end-to-end encryption with IPsec. While Generic Routing Encapsulation (GRE) might seem to be a network-layer protocol, if the encapsulation of the payload takes place only at the endpoint, GRE becomes closer to a transport protocol that uses IP headers but contains complete Layer 2 frames or Layer 3 packets to deliver to the endpoint. L2TP carries PPP frames inside transport segments.

    Although not developed under the OSI Reference Model and not strictly conforming to the OSI definition of the transport layer, the Transmission Control Protocol (TCP) and the User Datagram Protocol (UDP) of the Internet Protocol Suite are commonly categorized as layer-4 protocols within OSI.

    Transport Layer Security (TLS) provide security at this layer.

---
# Layer 3: Network Layer(網路層)
---

    The network layer provides the functional and procedural means of transferring variable length data sequences (called packets) from one node to another connected in "different networks". A network is a medium to which many nodes can be connected, on which every node has an address and which permits nodes connected to it to transfer messages to other nodes connected to it by merely providing the content of a message and the address of the destination node and letting the network find the way to deliver the message to the destination node, possibly routing it through intermediate nodes. If the message is too large to be transmitted from one node to another on the data link layer between those nodes, the network may implement message delivery by splitting the message into several fragments at one node, sending the fragments independently, and reassembling the fragments at another node. It may, but does not need to, report delivery errors.

    Message delivery at the network layer is not necessarily guaranteed to be reliable; a network layer protocol may provide reliable message delivery, but it need not do so.

    A number of layer-management protocols, a function defined in the management annex, ISO 7498/4, belong to the network layer. These include routing protocols, multicast group management, network-layer information and error, and network-layer address assignment. It is the function of the payload that makes these belong to the network layer, not the protocol that carries them.

---
# Layer 2: Data Link Layer(資料連結層)
---

    The data link layer provides node-to-node data transfer—a link between two directly connected nodes. It detects and possibly corrects errors that may occur in the physical layer. It defines the protocol to establish and terminate a connection between two physically connected devices. It also defines the protocol for flow control between them.

    IEEE 802 divides the data link layer into two sublayers:[20]

    Medium access control (MAC) layer – responsible for controlling how devices in a network gain access to a medium and permission to transmit data.
    Logical link control (LLC) layer – responsible for identifying and encapsulating network layer protocols, and controls error checking and frame synchronization.
    The MAC and LLC layers of IEEE 802 networks such as 802.3 Ethernet, 802.11 Wi-Fi, and 802.15.4 ZigBee operate at the data link layer.

    The Point-to-Point Protocol (PPP) is a data link layer protocol that can operate over several different physical layers, such as synchronous and asynchronous serial lines.

    The ITU-T G.hn standard, which provides high-speed local area networking over existing wires (power lines, phone lines and coaxial cables), includes a complete data link layer that provides both error correction and flow control by means of a selective-repeat sliding-window protocol.

    Security, specifically (authenticated) encryption, at this layer can be applied with MACSec.

---
# Layer 1: Physical Layer(實體層)
---

    The physical layer is responsible for the transmission and reception of unstructured raw data between a device and a physical transmission medium. It converts the digital bits into electrical, radio, or optical signals. Layer specifications define characteristics such as voltage levels, the timing of voltage changes, physical data rates, maximum transmission distances, modulation scheme, channel access method and physical connectors. This includes the layout of pins, voltages, line impedance, cable specifications, signal timing and frequency for wireless devices. Bit rate control is done at the physical layer and may define transmission mode as simplex, half duplex, and full duplex. The components of a physical layer can be described in terms of a network topology. Physical layer specifications are included in the specifications for the ubiquitous Bluetooth, Ethernet, and USB standards. An example of a less well-known physical layer specification would be for the CAN standard.

---
