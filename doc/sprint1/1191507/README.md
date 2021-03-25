RCOMP 2019-2020 Project - Sprint 1 - Member 1191507 folder
===========================================
## Disclaimer

The number of outlets in a work space is always rounded up after calculation according to the *ratio of two outlets per 10 sq. meters* rule i.e. 12.5 sq. m / 10 * 2 = 2,5 outlets = 4 outlets.

The unit of measure of Telecommunications Enclosures is considered to be *1U = 1 CAT6A 24 ports patch panel*. Also, all TE have a 50% oversize to accomodate future upgrades *(given U units space required for the patch panels (S), the size of the enclosure will be (6 x S))*.

Each floor has only one HC since the area of each one is smaller than 1000 square meters.

Copper cables are of type S/UTP since no information is known about electrical cable schematics, in order to prevent possible EMI without expending too much budget.

## Building 1 - Ground Floor
![Ground floor schematic plan] (ground_floor.jpg)

Outside network connection is directed through ceiling cable passeway to the datacenter on the floor above (IC).
Cabling from IC is redirected back to this floor and into the HC. There are CP on 10.2 and 10.3 due to the high outlet density (close to 24 or greater).

### 10.1

Approximate dimensions and resource usage:

|Room length | Room width | Area | No. of Outlets | Copper Cabling | Fibre Cabling | Total Cabling
|------------|------------|------|----------------|---------------|--------|------|
|12 m | 7 m | 84 sq m | 18 | 684 m | 0 m | 684 m |

Inventory
- 18 Outlets
- 1 CAT6A patch panel (24 ports)
- 1 Telecommunications Enclosure of size 2U
- 42 Patch cords (24 0.5m long for TE + 18 5m long for end-user equipment) 

### 10.2
Approximate dimensions and resource usage:

|Room length | Room width | Area | No. of Outlets | Copper Cabling | Fibre Cabling | Total Cabling
|------------|------------|------|----------------|---------------|--------|------|
|12 m | 11 m | 132 sq m | 28 | 210 m | 34 m | 244 m |

Inventory
- 28 Outlets
- 1 Telecommunications Enclosure (HC and CP) of size 6U
- 1 CAT6A Patch Panel (48 ports) for CP
- 1 CAT6A Patch Panel (24 ports) for HC
- 100 Patch cords (72 0.5m long for TE + 28 5m long for end-user equipment)

### 10.3
Approximate dimensions and resource usage:

|Room length | Room width | Area | No. of Outlets | Copper Cabling | Fibre Cabling | Total Cabling
|------------|------------|------|----------------|---------------|--------|------|
|26 m | 22 m | 329 sq m | 6 | 339 m | 0 m | 339 m |

An additional network outlet was placed for the wireless LAN access point, since it must be in the middle of the room to garantee coverage of the whole floor. There could be a second access point in room 10.1 or 10.2, which would allow the placement of the AP in a more cable efficient way, however the current alternative saves on outlet costs and limits coverage on the exterior of the building.

This room doesn't have a CP since the number of outlets is relatively small and the cabling would be easy to install from HC due to the underfloor raceway.

Inventory
- 6 Outlets
- 1 Access Point/Router
- 6 Patch cords (up to 5 m long)

## Building 1 - First Floor
![First floor schematic plan] (first_floor.jpg)

The HC on this floor connects all network outlets of area 11.2 as well as CP for areas 11.3 and 11.4 (which have a higher density of outlets).

No wireless access point was placed on this floor, since the coverage is guaranteed by the access point on the ground floor.

### 11.1
This room houses the datacenter. Wiring and outlets are out of scope for this project.

### 11.2
Approximate dimensions and resource usage:

|Room length | Room width | Area | No. of Outlets | Copper Cabling | Fibre Cabling | Total Cabling
|------------|------------|------|----------------|---------------|--------|------|
|8 m | 6 m | 48 sq m | 10 | 154 m | 0 m | 154 m |

This room doesn't have a CP since the number of outlets is relatively small and the HC is located in the adjacent room, making the cabling easier to install.

Inventory:
- 10 Outlets
- 10 Patch cords (up to 5 m long)

### 11.3
Approximate dimensions and resource usage:

|Room length | Room width | Area | No. of Outlets | Copper Cabling | Fibre Cabling | Total Cabling
|------------|------------|------|----------------|---------------|--------|------|
|12 m | 7 m | 84 sq m | 18 | 666 m | 0 m | 666 m |

Inventory:
- 18 Outlets
- 1 CAT6A Patch Panel (24 ports)
- 1 Telecommunications Enclosure of size 2U
- 42 Patch cords (24 0.5m long for TE + 18 5m long for end-user equipment) 

### 11.4
Approximate dimensions and resource usage:

|Room length | Room width | Area | No. of Outlets | Copper Cabling | Fibre Cabling | Total Cabling
|------------|------------|------|----------------|---------------|--------|------|
|12 m | 11 m | 132 sq m | 28 | 1088 m | 0 m | 1088 m |

Inventory:
- 28 Outlets
- 1 CAT6A Patch Panel (48 ports)
- 1 Telecommunications Enclosure of size 4U
- 48 Patch cords
- 76 Patch cords (24 0.5m long for TE + 18 5m long for end-user equipment) 

### 11.5
This room is for storage and requires no outlets or cabling.
