#### Link state routing Protocols:
>when using a link state routing protocol every router creates a connectivity map of the network
>to make a map every router advertise its information about its interfaces to its neighbors and these advertisements are passed along to other routers until all routers in the network develop the same map of the network.
>each router independently uses the map to calculate the best route to each destination.
>
#### OSPF:
>stands for open shortest path first 
>also known as dijkstra algorithm
>three version ospf v1, v2, v3
>router store information about the network in LSAs that are organized in a structure called lsdb 

#### Metric:
>ospf metric is called as cost
>it is calculated based on the bandwidth speed of the interface 
>it is calculated by dividing the reference bandwidth value by the interface bandwidth.
>the default reference bandwidth is 100 mbps.
>fast ethernet with a speed of 100 mbps has a cost of 1 100/100= 1
>change the ospf cost `auto cost reference bandwidth mbps `

#### OSPF Broadcast network type:
>they are enabled on ethernet interfaces by default 
>hello msgs are send to 224.0.0.5
>a dr bdr and drother is elected with the interface priority and the highest router id btw the interface priority is 1 on all interfaces 
>in the broadcast network the router will form full adjacency with the dr and bdr of the network segment not dr other.

#### P to P network:
>enabled on serial interfaces using ppp and hdlc 

#### OSPF msg types:
>- hello
>- DBD
>- LSR
>- LSU
>- LSACK
>ospf has 5 msg types.
