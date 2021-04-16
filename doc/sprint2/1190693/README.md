RCOMP 2019-2020 Project - Sprint 2 - Member 3333333 folder
===========================================

- Since in the ground floor in the right area are multiple CPs but they function in the same way to simplify the diagram I decided to only use one switch to represent all CPs in the right area.

<br/>

## Network devices and End nodes representations:

|           Name           |Representation |
|-------------------------:|---------------|
|Intermediate Cross Connect|Switch PT-Empty|
|Horizontal Cross-Connect  |Switch PT-Empty|
|Consolidation Point       |Switch PT-Empty|
|Access Point              |AccessPoint-PT |
|Nodes within DMZ          |Server-PT      |
|VoIP                      |Ip-Phone 7960  |
|Computer                  |PC-PT          |
|Laptop                    |Laptop-PT      |
|Router                    |Router 2811    |
|                          |               |

<br/>

# Building 3 nodes required

|  Network  |Required Nodes|
|----------:|:-------------|
|GroundFloor|      40      |
|FirstFloor |      44      |
|WI-FI      |      60      |
|DMZ        |     250      |
|VoIP       |      40      |
|Total      |     434      |
|           |              |

<br/>

## Building 3 Machine Ip Address
<br/>

## Available Ip Addressesses

|       VLAN|Nodes| Address          | Address Mask    |Network Address|Broadcast Address|First Valid Network|Last Valid Network|
|----------:|:---:|:----------------:|:---------------:|:-------------:|:---------------:|:-----------------:|:----------------:|
|GroundFloor| 40  | 10.126.85.192/26 | 255.255.255.192 | 10.126.85.192 | 10.126.85.255   | 10.126.85.193     |10.126.85.254     |
| FirstFloor| 44  | 10.126.85.0/26   | 255.255.255.192 | 10.126.85.0   | 10.126.85.63    | 10.126.85.1       |10.126.85.62      |
|      WI-FI| 60  | 10.126.84.64/26  | 255.255.255.192 | 10.126.84.64  | 10.126.84.127   | 10.126.84.65      |10.126.84.126     |
|        DMZ| 250 | 10.126.80.0/24   | 255.255.255.0   | 10.126.80.0   | 10.126.80.255   | 10.126.80.1       |10.126.80.254     |
|       VoIP| 40  | 10.126.86.0/26   | 255.255.255.192 | 10.126.86.0   | 10.126.86.63    | 10.126.86.1       |10.126.86.62      |
|           |     |                  |                 |               |                 |                   |                  |

<br/>

## Used Ip Adressesses

|       VLAN|            Machine                  | IP Address    |  Default Gateway |
|----------:|:------------------------------------|:-------------:|:----------------:|
|GroundFloor| Building3_GroundFloor_PC_Room_30.1  | 10.126.85.194 | 10.126.85.193    |
|           | Building3_GroundFloor_PC_Room_30.2  | 10.126.85.195 | 10.126.85.193    |
|           | Building3_GroundFloor_PC_Room_30.3  | 10.126.85.196 | 10.126.85.193    |
|           | Building3_GroundFloor_PC_Room_30.4  | 10.126.85.197 | 10.126.85.193    |
|           | Building3_GroundFloor_PC_Room_30.5  | 10.126.85.198 | 10.126.85.193    |
|           | Building3_GroundFloor_PC_RightSide_1| 10.126.85.199 | 10.126.85.193    |
| FirstFloor| Building3_FirstFloor_PC_Room_31.1   | 10.126.85.2   | 10.126.85.1      |
|           | Building3_FirstFloor_PC_Room_31.2   | 10.126.85.3   | 10.126.85.1      |
|           | Building3_FirstFloor_PC_Room_31.3   | 10.126.85.4   | 10.126.85.1      |
|           | Building3_FirstFloor_PC_Room_31.4   | 10.126.85.5   | 10.126.85.1      |
|           | Building3_FirstFloor_PC_Room_31.5   | 10.126.85.6   | 10.126.85.1      |
|           | Building3_FirstFloor_PC_Room_31.6   | 10.126.85.7   | 10.126.85.1      |
| DMZ       | Building3_Server                    | 10.126.80.2   | 10.126.80.1      |

<br/>

# Router 
  
## Router Sub-Interfaces

| Port              | VLAN | Address       | Mask            |
|-------------------|------|---------------|-----------------|
| FastEthernet0/0.1 | 325  | 10.126.85.193 | 255.255.255.192 |
| FastEthernet0/0.2 | 326  | 10.126.85.1   | 255.255.255.192 |
| FastEthernet0/0.3 | 327  | 10.126.84.65  | 255.255.255.192 |
| FastEthernet0/0.4 | 328  | 10.126.80.1   | 255.255.255.0   |
| FastEthernet0/0.5 | 329  | 10.126.86.1   | 255.255.255.192 |
| FastEthernet0/0.6 | 340  | 10.126.82.2   | 255.255.255.128 |
<br/>

## Routing table

| Building | Network       | Mask            | Next hop    |
|---------:|:-------------:|:---------------:|:-----------:|
| 2        | 10.126.84.0   | 255.255.255.192 | 10.126.82.1 |
|          | 10.126.83.128 | 255.255.255.128 | 10.126.82.1 |
|          | 10.126.82.128 | 255.255.255.128 | 10.126.82.1 |
|          | 10.126.87.64  | 255.255.255.240 | 10.126.82.1 |
|          | 10.126.86.192 | 255.255.255.192 | 10.126.82.1 |
| 5        | 10.126.86.64  | 255.255.255.192 | 10.126.82.4 |
|          | 10.126.84.128 | 255.255.255.128 | 10.126.82.4 |
|          | 10.126.81.0   | 255.255.255.0   | 10.126.82.4 |
|          | 10.126.86.128 | 255.255.255.192 | 10.126.82.4 |
| -        | 0.0.0.0       | 0.0.0.0         | 10.126.82.3 |

> Netwrok aggregation for the networks:
> - 10.126.84.128/26 and 10.126.84.192/26 to 10.126.84.128/25