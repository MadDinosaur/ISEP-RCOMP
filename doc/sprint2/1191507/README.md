RCOMP 2020-2021 Project - Sprint 2 - Member 1101507 folder
===========================================

## Disclaimer

Despite the number of end devices that building 1 is equipped to support, in order to keep the simulation concise and easy to read, each room that has outlets is represented by only one end device (PC).

The number of ports in each switch are not representative of the number of ports on the physical equipment considered in the structured cabling project from sprint 1. Each switch has only the sufficient number of ports for the simulation to be functional.

The IP-Phone was connected to the ground floor HC since it is the closest point to the reception desk on room 10.3, where presumably a telephone line will be needed. The Server can be placed in the datacentre (room 11.1) and for that reason was connected to the building IC.

Wireless and phone end devices' IP addresses are represented in this document but are not configurated in the simulation since the related information is not available on the current sprint. The adresses below are, therefore, hypothetical.

---

## Network Devices and End Nodes representations

|           Name           |Representation |
|--------------------------|---------------|
|Intermediate Cross Connect|Switch PT-Empty|
|Horizontal Cross-Connect  |Switch PT-Empty|
|Consolidation Point       |Switch PT-Empty|
|Access Point              |AccessPoint-PT |
|Nodes within DMZ          |Server-PT      |
|VoIP                      |Ip-Phone 7960  |
|Computer                  |PC-PT          |
|Laptop                    |Laptop-PT      |
|Router                    |Router 2811    |

---
## Building 1 and Backbone nodes required

|  Network  |Required Nodes|
|-----------|--------------|
|GroundFloor|      40      |
|FirstFloor |      40      |
|WI-FI      |      24      |
|DMZ        |      70      |
|VoIP       |      20      |
|Backbone   |     120      |
|Total      |     314      |

---
## Building 1 Devices Static IP Addresses
### Backbone VLAN
|Device | IP Address |
|-------|------------|
|Building1_Router | 10.126.82.3 |
<br>
### Ground Floor VLAN
|Device | IP Address |
|-------|------------|
|Building1_Router | 10.126.85.65 |
|Building1_GroundFloor_PC_01 | 10.126.85.66 |
|Building1_GroundFloor_PC_02 | 10.126.85.67 |
|Building1_GroundFloor_PC_03 | 10.126.85.69 |
<br>
### First Floor VLAN
|Device | IP Address |
|-------|------------|
|Building1_Router | 10.126.85.129 |
|Building1_FirstFloor_PC_01 | 10.126.85.130 |
|Building1_FirstFloor_PC_02 | 10.126.85.132 |
|Building1_FirstFloor_PC_03 | 10.126.85.133 |
<br>
### Wifi VLAN
|Device | IP Address |
|-------|------------|
|Building1_Router | 10.126.87.1 |
|Building1_GroundFloor_WirelessLaptop | 10.126.87.2 |
|Building1_FirstFloor_WirelessLaptop | 10.126.87.3 |
<br>
### DMZ VLAN
|Device | IP Address |
|-------|------------|
|Building1_Router | 10.126.83.1 |
|Building1_Server | 10.126.83.2 |
<br>
### VoIP VLAN
|Device | IP Address |
|-------|------------|
|Building1_Router | 10.126.87.33 |
|Building1_Server | 10.126.87.34 |

---
## Routing Table

|    Building    |    Network     |      Mask       |    Next Hop   |     
|:--------------:|:--------------:|:---------------:|:-------------:|
|2 | 10.126.82.128 | 255.255.255.128 | 10.126.82.1 | 
|2 | 10.126.83.128 | 255.255.255.128 | 10.126.82.1 |
|2 | 10.126.84.0   | 255.255.255.128 | 10.126.82.1 |
|2 | 10.126.86.192 | 255.255.255.255 | 10.126.82.1 | 
|2 | 10.126.87.64  | 255.255.255.255 | 10.126.82.1 |
|3 | 10.126.80.0   | 255.255.255.0   | 10.126.82.2 |
|3 | 10.126.84.64  | 255.255.255.192 | 10.126.82.2 | 
|3 | 10.126.85.0   | 255.255.255.192 | 10.126.82.2 |
|3 | 10.126.85.192 | 255.255.255.192 | 10.126.82.2 |
|3 | 10.126.86.0   | 255.255.255.192 | 10.126.82.2 |
|5 | 10.126.81.0   | 255.255.255.0   | 10.126.82.4 |
|5 | 10.126.84.128 | 255.255.255.192 | 10.126.82.4 | 
|5 | 10.126.84.192 | 255.255.255.192 | 10.126.82.4 |
|5 | 10.126.86.64  | 255.255.255.192 | 10.126.82.4 |
|5 | 10.126.86.128 | 255.255.255.192 | 10.126.82.4 |
|Internet | 0.0.0.0 | 0.0.0.0 | 120.57.201.201 |
