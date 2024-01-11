# OSPF

which is a unique feature of OSPF that splits large networks into smaller sections

## Distance vector protocol

use `routing by rumor` in which each router shares information about the routers they know
and their metric cost to reach each destination

However, the routers don't have a complete map of the network they use the information their
neighboring routers tell them to determine the best route to each destination

When using a `Link state` routing protocol every router creates a connectivity map of the
network

all routers have the same complete map of the network, each router independently uses this
map to calculate the best route to each destination

Like state protocols use more resources (CPU) on the router because more information is shared

Routers store information about the network in LSAs, which are organized in a structure called 

the LSDB

Routers will flood LSAs until all routers in the OSPF area develop the same map of the network(LSDB)

Note: In the case of OSPF, it means they send the LSAs to all of their OSPF neighbors

