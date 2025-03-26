Okay, here are the viva questions and answers, broken down by the 'a' and 'b' parts of each practical, as per your index:

**Practical 1: Configuring OSPF – I**

**(a) Single-Area OSPF Link Costs and Interface Priorities**

* **Question:** What is a single-area OSPF configuration?
    * **Answer:** An OSPF network where all routers are in the same area (Area 0).
* **Question:** How are OSPF link costs calculated by default?
    * **Answer:** Based on the interface bandwidth (reference bandwidth / interface bandwidth).
* **Question:** Why would you change OSPF link costs?
    * **Answer:** To influence path selection and traffic flow.
* **Question:** What is OSPF interface priority used for?
    * **Answer:** To determine the Designated Router (DR) and Backup Designated Router (BDR) on multiaccess networks.
* **Question:** How does a lower interface priority affect the DR/BDR election?
    * **Answer:** A lower priority makes a router less likely to become DR or BDR.

**(b) Multi-Area OSPF with Stub Areas and Authentication**

* **Question:** What is a multi-area OSPF configuration?
    * **Answer:** An OSPF network divided into multiple areas for scalability and efficiency.
* **Question:** What is a stub area in OSPF?
    * **Answer:** An area that doesn't receive external routes, reducing LSDB size.
* **Question:** Why use OSPF authentication?
    * **Answer:** To secure OSPF communication and prevent unauthorized updates.
* **Question:** What are some types of OSPF authentication?
    * **Answer:** Plaintext and MD5.

**Practical 2: Configuring OSPF – II**

**(a) OSPF Virtual Links and Area Summarization**

* **Question:** What is an OSPF virtual link?
    * **Answer:** A logical connection between areas that are not directly connected to the backbone area (Area 0).
* **Question:** When are virtual links necessary?
    * **Answer:** When an area becomes partitioned from the backbone.
* **Question:** What is OSPF area summarization?
    * **Answer:** The process of advertising summarized or aggregate addresses for an area.
* **Question:** What is the benefit of area summarization?
    * **Answer:** Reduces routing table size and routing overhead.

**(b) OSPF over Frame Relay**

* **Question:** What are some considerations when running OSPF over Frame Relay?
    * **Answer:** Frame Relay is a non-broadcast multi-access (NBMA) network, so OSPF network types need to be configured appropriately.
* **Question:** Why is the OSPF network type important on Frame Relay?
    * **Answer:** It affects DR/BDR election and neighbor discovery.
* **Question:** What are some OSPF network types used with Frame Relay?
    * **Answer:** Point-to-multipoint, non-broadcast.

**Practical 3: Redistribution and Administrative Distances**

**(a) Redistribution Between RIP and OSPF**

* **Question:** What is route redistribution?
    * **Answer:** The process of exchanging routing information between different routing protocols.
* **Question:** Why might you redistribute routes between RIP and OSPF?
    * **Answer:** To allow routers running different protocols to communicate.
* **Question:** What are some potential issues with route redistribution?
    * **Answer:** Routing loops, inaccurate metrics.

**(b) Manipulating Administrative Distances**

* **Question:** What is administrative distance?
    * **Answer:** A metric that indicates the trustworthiness of a routing source.
* **Question:** Why would you manipulate administrative distance?
    * **Answer:** To prefer routes from one routing protocol over another.
* **Question:** How do lower and higher administrative distances compare?
    * **Answer:** Lower AD is preferred.

**Practical 4: BGP**

**(a) Configuring BGP with Default Routing**

* **Question:** What is BGP?
    * **Answer:** Border Gateway Protocol, an inter-AS routing protocol.
* **Question:** What is a default route in BGP?
    * **Answer:** A route (0.0.0.0/0) used to forward traffic to an unknown destination.
* **Question:** When is configuring BGP with a default route useful?
    * **Answer:** To provide Internet access to an AS.

**(b) Using the AS_PATH Attribute**

* **Question:** What is the AS_PATH attribute?
    * **Answer:** A BGP attribute that lists the autonomous systems a route has traversed.
* **Question:** What is the purpose of the AS_PATH attribute?
    * **Answer:** To prevent routing loops and help in path selection.

**(c) BGP Route Reflectors and Route Filters**

* **Question:** What is a BGP route reflector?
    * **Answer:** A BGP router that relaxes the iBGP full-mesh requirement.
* **Question:** Why are route reflectors used?
    * **Answer:** To simplify iBGP configuration in large ASes.
* **Question:** What are BGP route filters?
    * **Answer:** Mechanisms to control the routing information that is advertised or received.
* **Question:** What are some ways to implement route filters in BGP?
    * **Answer:** Prefix lists, AS-path lists, and community lists.

**Practical 5: IPv6**

**(a) Configuring OSPF for IPv6**

* **Question:** What is OSPF for IPv6 called?
    * **Answer:** OSPFv3.
* **Question:** How does OSPFv3 differ from OSPFv2?
    * **Answer:** It uses link-local addresses and runs per-link rather than per-subnet.

**(b) Configuring 6to4 Tunnels**

* **Question:** What is a 6to4 tunnel?
    * **Answer:** A transition mechanism to encapsulate IPv6 traffic over an IPv4 network.
* **Question:** Why were 6to4 tunnels developed?
    * **Answer:** To allow IPv6 hosts to communicate over the existing IPv4 infrastructure.

**Practical 6: VLANs and EtherChannel**

**(a) Static VLANs, VLAN Trunking, and VTP Domains and Modes**

* **Question:** What is a static VLAN?
    * **Answer:** A VLAN assigned to a port manually.
* **Question:** What is VLAN trunking?
    * **Answer:** Carrying traffic from multiple VLANs over a single link.
* **Question:** What is VTP?
    * **Answer:** VLAN Trunking Protocol, used to propagate VLAN information.
* **Question:** What are VTP modes?
    * **Answer:** Server, client, and transparent.

**(b) Configuring EtherChannel**

* **Question:** What is EtherChannel?
    * **Answer:** Link aggregation technology that bundles multiple physical links into a single logical link.
* **Question:** What are the benefits of EtherChannel?
    * **Answer:** Increased bandwidth and redundancy.
* **Question:** What are some EtherChannel protocols?
    * **Answer:** LACP (Link Aggregation Control Protocol) and PAgP (Port Aggregation Protocol).

**Practical 7: Spanning Tree Protocol**

**(a) Spanning Tree Protocol (STP) Default Behavior**

* **Question:** What is the purpose of STP?
    * **Answer:** To prevent Layer 2 switching loops.
* **Question:** How does STP prevent loops?
    * **Answer:** By blocking redundant paths.
* **Question:** What is the root bridge?
    * **Answer:** The reference point for STP calculations.

**(b) Modifying Default Spanning Tree Behavior**

* **Question:** How can you modify STP behavior?
    * **Answer:** By changing bridge priority or path costs.
* **Question:** Why would you modify STP behavior?
    * **Answer:** To influence which ports forward traffic and optimize the network topology.
* **Question:** What are some STP enhancements?
    * **Answer:** RSTP (Rapid Spanning Tree Protocol) and MSTP (Multiple Spanning Tree Protocol).
