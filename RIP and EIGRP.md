#### RIP:
>routing protocol that is industry standard.
>distance vector protocol (uses routing by rumor logic)
>uses hop count as its metric one router = one hop.
>the maximum hop count of a route is 15 
>rip uses two msgs:
>- request 
>- response
>by default rip enabled routers will share there routing tables every 30 seconds
>rip v2 supports vlsm and cidr and include information such as subnet mask in advertisements.
>messages are multicast address to 224.0.0.9

#### EIGRP:
>eigrp stands for enchanced interior gateway routing protocol 
>improved version of igrp
>eigrp can perform unqual ecmp
>the AS number must match between router or they will not form adjacency and share route information.