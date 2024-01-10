# OSPF

which is a unque feature of ospf that splits large networks into smaller sections

## Distance vector protocol

use `router by rumor` in which echo route shares information about the routers they know
and their metric cost to reach each destination

However the routers don't have a complete map of the network they use the information their
neighboring routers tell them to determine the best route to each destination

When using a `Link state` routing protocol every router creates a connectivity map of the
network

all routers have the some complete map of the network, each router independently uses this
map to calculate the best route to each destination

Like state protocols use more resource(cpu) on the router, becouse more information is shared

Routers store information about the network in LSAs, which are organized in struture called 

the LSDB

Routers will flood LSAs untill all routers in the OSPF area develop the same map of network(LSDB)

Note: In the case of OSPF, it means they send the LSAs to all of their OSPF neighbors

