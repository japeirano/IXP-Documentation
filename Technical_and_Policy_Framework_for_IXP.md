# Introduction

This document outlines the technical specifications, connection policies, and operational guidelines for participants of the Internet Exchange Point (IXP). It aims to ensure efficient, secure, and fair interconnection among members.

# Infrastructure Design and Specifications

## Network Design for the IXP
•	A detailed diagram of the network architecture is provided, showcasing the core and edge design, redundancy schemes, and capacity planning from edge to core to ensure high availability and scalability.

## Core Facility Layout
•	Illustrations of the main IXP facility's layout, including room arrangements tailored for optimal operations.
•	Specifics on rack configurations for cross-connects, ensuring efficient cable management and accessibility.
•	For self-run facilities, details on cooling and power infrastructure are provided to maintain optimal equipment performance and reliability.

## PoP Facility Layouts
•	Instructions for connecting at various points of presence (PoPs), enhancing the IXP's network reach.
•	For each PoP, layouts include room configurations, rack setups, and, for self-run facilities, cooling and power infrastructure, mirroring the core facility's emphasis on efficiency and reliability.

## Equipment Specifications
•	A comprehensive list of all networking hardware in use, including switches, routers, and any specialized equipment.
•	Detailed guidelines for configuring the equipment, ensuring consistency and best practices across the network.

 
# Technical Prerequisites

## Layer 1 (Physical Connectivity)
•	The IXP offers Ethernet connectivity over a switching infrastructure.
•	Service offerings include defined rates such as 10GE (Optical - LC) and 40GE (Optical - LC).
•	Link aggregation (802.3ad) is available upon request to support higher bandwidth requirements.

## Layer 2 (Data Link)
•	Each VLAN is allowed only one MAC address, which must be from the participant's Layer 3 device, typically a router interface.
•	Participants are required to disable spanning-tree on their exchange-facing interfaces to prevent broadcast storms or other Layer 2 issues.
•	The IXP will block all spanning-tree protocols to maintain network stability.

## Layer 3 (Network)
•	Participants will receive IP connectivity details (IPv4/IPv6) with appropriate subnet masks.
•	BGP sessions must be established using IP addresses provided by the IXP.
•	Proxy ARP and IPv6 Proxy Neighbour Discovery will be disabled on participant interfaces.
•	Prefix advertisements must be authorized by a regional internet registry through route object or RPKI ROA (e.g., APNIC, RIPE NCC etc) or accompanied by a no objection certificate/letter from the customer.

# Peering Policies

The IXP promotes a peering strategy that meets the expectations of all members and addresses the requirements of a contemporary peering fabric. Our objective is to optimize the utilization of the fabric in the most effective manner, thereby enhancing local traffic growth.

•	Multilateral Peering: We recommend and expect all members to peer with the route server, facilitating multilateral peering arrangements. 

•	Bilateral Peering Flexibility: Recognizing the varied strategic needs of our members, we also allow for bilateral peering arrangements. Members opting for bilateral peering are encouraged to do so in addition to participating in the multilateral peering setup. This flexibility ensures that members can establish direct peering relationships as per their individual policy requirements and strategic interests.

•	Peering Policy Publication: Members who prefer bilateral peering only are required to publish their peering policies. This transparency helps other members understand the criteria for establishing direct peering relationships, fostering an environment of open communication and collaboration.

•	Remote Peering: To accommodate the needs of members not located within the same city as our facilities, remote peering is permitted. Members may establish connectivity via their own Layer 2 backhaul or through accredited carrier providers. This inclusivity ensures that geographical location does not hinder participation in the IXP, thereby enhancing its reach and the diversity of its network connections.

# Operational Policies

## Support and Maintenance
•	The IXP will provide contact details for operational support, published on the IXP's website.
•	A procedure for announcing service-affecting maintenance will be established and communicated to participants.

## Monitoring and Statistics
•	The IXP's operations team will monitor the exchange platform for performance issues and inform participants of any significant events.
•	Traffic statistics, including total incoming and outgoing traffic volumes and participating AS numbers, will be published on a publicly accessible website.

## Compliance and Security
•	Participants are required to comply with all technical standards and security measures outlined in this framework.
•	The IXP reserves the right to take necessary actions to preserve the integrity and security of the exchange platform.
