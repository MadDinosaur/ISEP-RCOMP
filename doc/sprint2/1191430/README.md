RCOMP 2020-2021 Project - Sprint 2 - Member 1191430 folder
==========================================================

### Notes on building 2's network simulation design

The task assigned to me in this sprint was the development of a layer two and layer three Packet Tracer simulation for building 2, and also encompassing the campus backbone.

As in sprint 2 it is necessary to simulate a network layout for building 2 based on the representation made in sprint 1, as a high number of nodes was assigned to each network, it will only be represented by one machine, that is, each CP will only be connected to a PC and if necessary to an AP.

As on the first floor of building 2 I assigned more cps than the switch in the packet tracer can contain, I only identified 7 cps at most 9, however the remaining cps that remain to be identified are the same as the rest, so one of the cps that are represented can exemplify the functionality of those that are missing.

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

### Building 2 nodes required

|  Network  |Required Nodes|
|-----------|--------------|
|GroundFloor|      60      |
|FirstFloor |      70      |
|WI-FI      |     100      |
|DMZ        |      12      |
|VoIP       |      40      |
|Total      |     282      |

### Building 2 Machine Ip Address

|            Machine            | IP Address  |
|-------------------------------|-------------|
|Buidling2_PC_GroundFloor_01    |10.126.84.2  |
|Building2_Laptop_GroundFloor_01|10.126.82.130|
|Building2_Laptop_GroundFloor_02|10.126.82.131|
|Building2_PC_GroundFloor_02    |10.126.84.3  |
|Building2_PC_GroundFloor_03    |10.126.84.4  |
|Building2_PC_FirstFloor_01     |10.126.83.130|
|Building2_PC_FirstFloor_02     |10.126.83.131|
|Building2_Laptop_FirstFloor_01 |10.126.82.132|
|Building2_PC_FirstFloor_03     |10.126.83.132|
|Building2_PC_FirstFloor_04     |10.126.83.133|
|Building2_PC_FirstFloor_05     |10.126.83.134|
|Building2_PC_FirstFloor_06     |10.126.83.135|
|Building2_Laptop_FirstFloor_02 |10.126.82.133|
|Building2_PC_FirstFloor_07     |10.126.83.136|
|Building2_PC_FirstFloor_08     |10.126.83.137|
