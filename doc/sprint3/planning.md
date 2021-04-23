RCOMP 2020-2021 Project - Sprint 3 planning
===========================================

### Sprint master: 1181490


# 1. Sprint's backlog # 


Update the campus.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 1,2,3,5.

# 2. Technical decisions and coordination #

-   DHCPv4 service

-   VoIP service

    |Building|Number|
    |:------:|:----:|
    |    1   | 111111111|
    |    2   | 222222222|
    |    3   | 333333333|
    |    5   | 555555555|
    
-   Adding a second server to each DMZ network to run the HTTP service.

    |Building|Server|
    |:------:|:----:|
    |    1   | WEB1|
    |    2   | WEB2|
    |    3   | WEB3|
    |    5   | WEB5|

-   Configuring DNS servers to establish a DNS domains tree.

    |Building|IPv4|DNS Domain|DNS Name Server|
    |:------:|:--:|:--------:|:-------------:|
    | 1 | 10.126.83.2| rcomp-20-21-dl-g1 | ns.rcomp-20-21-dl-g1 |
    | 2 | 10.126.87.66  | building-2.rcomp-20-21-dl-g6 | ns.building-2.rcomp-20-21-dl-g1 |
    | 3 | 10.126.80.2 | building-3.rcomp-20-21-dl-g6 | ns.building3.rcomp-20-21-dl-g6 |
    | 5 | 10.126.81.2 |  building-5.rcomp-20-21-dl-g6|ns.building5.rcomp-20-21-dl-g6 |


-   Enforcing NAT (Network Address Translation).
-   Establishing traffic access policies (static firewall) on routers.
  
# 3. Subtasks assignment #

-   1191507 - Update the campus.pkt layer three Packet Tracer simulation from the
previous sprint, to include the described features in this sprint for
building 1.

-   1191430 - Update the campus.pkt layer three Packet Tracer simulation from the
previous sprint, to include the described features in this sprint for
building 2.
Final integration of each member’s Packet Tracer simulation into a
single simulation.


-  1190693 - Update the campus.pkt layer three Packet Tracer simulation from the
previous sprint, to include the described features in this sprint for
building 3.

- 1181490 - Update the campus.pkt layer three Packet Tracer simulation from the
previous sprint, to include the described features in this sprint for
building 5.


# 4. Taks: #

1.  OSPF dynamic routing 
2.  HTTP servers 
3.  DHCPv4 Service
4.  VoIP service
5.  DNS
6.  NAT (Network Address Translation)

