RCOMP 2019-2020 Project - Sprint 2 - Member 3333333 folder
===========================================

## Network devices and End nodes representations:

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
|                          |               |

## Building 3 nodes required

|  Network  |Required Nodes|
|----------:|:-------------|
|GroundFloor|      40      |
|FirstFloor |      44      |
|WI-FI      |      60      |
|DMZ        |     250      |
|VoIP       |      40      |
|Total      |     434      |
|           |              |

## Building 3 Machine Ip Address

### Available Ip Addressesses

|       VLAN|Nodes| Address          | Address Mask    |Network Address|Broadcast Address|First Valid Network|Last Valid Network|
|----------:|:---:|:----------------:|:---------------:|:-------------:|:---------------:|:-----------------:|:----------------:|
|GroundFloor| 40  | 10.126.85.192/26 | 255.255.255.192 | 10.126.85.192 | 10.126.85.255   | 10.126.85.193     |10.126.85.254     |
| FirstFloor| 44  | 10.126.85.0/26   | 255.255.255.192 | 10.126.85.0   | 10.126.85.63    | 10.126.85.1       |10.126.85.62      |
|      WI-FI| 60  | 10.126.84.64/26  | 255.255.255.192 | 10.126.84.64  | 10.126.84.127   | 10.126.84.65      |10.126.84.126     |
|        DMZ| 250 | 10.126.80.0/24   | 255.255.255.0   | 10.126.80.0   | 10.126.80.255   | 10.126.80.1       |10.126.80.254     |
|       VoIP| 40  | 10.126.86.0/26   | 255.255.255.192 | 10.126.86.0   | 10.126.86.63    | 10.126.86.1       |10.126.86.62      |
|           |     |                  |                 |               |                 |                   |                  |


### Used Ip Adressesses

|       VLAN|            Machine                  | IP Address    |
|----------:|:------------------------------------|:-------------:|
|GroundFloor| Building3_GroundFloor_PC_Room_30.1  | 10.126.85.194 |
|           | Building3_GroundFloor_PC_Room_30.2  | 10.126.85.195 |
|           | Building3_GroundFloor_PC_Room_30.3  | 10.126.85.196 |
|           | Building3_GroundFloor_PC_Room_30.4  | 10.126.85.197 |
|           | Building3_GroundFloor_PC_Room_30.5  | 10.126.85.198 |
|           | Building3_GroundFloor_PC_RightSide_1| 10.126.85.199 |
| FirstFloor| Building3_FirstFloor_PC_Room_31.1   | 10.126.85.2   |
|           | Building3_FirstFloor_PC_Room_31.2   | 10.126.85.3   |
|           | Building3_FirstFloor_PC_Room_31.3   | 10.126.85.4   |
|           | Building3_FirstFloor_PC_Room_31.4   | 10.126.85.5   |
|           | Building3_FirstFloor_PC_Room_31.5   | 10.126.85.6   |
|           | Building3_FirstFloor_PC_Room_31.6   | 10.126.85.7   |
| WI-FI     | -                                   | 10.126.84.66  |
| DMZ       | Building3_Server                    | 10.126.80.2   |
