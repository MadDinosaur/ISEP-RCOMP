RCOMP 2019-2020 Project - Sprint 2 - Member 1181490 folder
===========================================

### Notes on building 5's network simulation design

The task assigned to me in this sprint was the development of a layer two and layer three Packet Tracer simulation for building 5, and also encompassing the campus backbone.

As in sprint 2 it is necessary to simulate a network layout for building 5 based on the representation made in sprint 1, as a high number of nodes was assigned to each network, it will only be represented by one machine, that is, each CP will only be connected to a PC and if necessary to an AP.

### Network devices and End nodes representations:

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

### Building 5 nodes required

|  Network  |Required Nodes|
|-----------|--------------|
|GroundFloor|      40      |
|FirstFloor |      10      |
|WI-FI      |      60      |
|DMZ        |      250     |
|VoIP       |      40      |
|Total      |     400      |

### Building 5 Machine Ip Address

|            Machine            | IP Address  |
|-------------------------------|-------------|
|Buidling5_PC_GroundFloor_2     |10.126.86.66 |
|Building5_PC_GroundFLoor_5     |10.126.86.67 |
|Building5_PC_GroundFloor_3     |10.126.86.68 |
|Building5_PC_GroundFloor_4     |10.126.86.69 |
|Building5_PC_FirstFloor_0      |10.126.84.195|
|Building5_PC_FirstFloor_1      |10.126.84.194|


# Router 
  
## Router Sub-Interfaces

| Port              | VLAN | Address       | Mask               |
|-------------------|------|---------------|-----------------   |
| FastEthernet0/0.1 | 330  | 10.126.86.65  | 255.255.255.192    |
| FastEthernet0/0.2 | 331  | 10.126.84.193 | 255.255.255.192    |
| FastEthernet0/0.3 | 332  | 10.126.84.129 | 255.255.255.192    |
| FastEthernet0/0.4 | 333  | 10.126.84.1   | 255.255.255.192    |
| FastEthernet0/0.5 | 334  | 10.126.81.1   | 255.255.255.0      |
| FastEthernet0/0.6 | 340  | 10.126.86.129 | 255.255.255.192    |


## Routing table
| Building | Network       | Mask            | Next Hop          |
|----------|---------------|-----------------|------------       |
|   2      | 10.126.80.0   | 255.255.255.0   | 10.126.82.2       |
|          | 10.126.84.64  | 255.255.255.192 | 10.126.82.2       |
|          | 10.126.85.0   | 255.255.255.192 | 10.126.82.2       |
|          | 10.126.85.192 | 255.255.255.192 | 10.126.82.2       |
|          | 10.126.86.0   | 255.255.255.192 | 10.126.82.2       |
|   3      | 10.126.82.128 | 255.255.255.128 | 10.126.82.1       | 
|          | 10.126.83.128 | 255.255.255.128 | 10.126.82.1       |
|          | 10.126.84.0   | 255.255.255.128 | 10.126.82.1       |
|          | 10.126.86.192 | 255.255.255.255 | 10.126.82.1       | 
|          | 10.126.87.64  | 255.255.255.255 | 10.126.82.1       |
|   1      | 0.0.0.0       | 0.0.0.0         | 10.126.82.3       |