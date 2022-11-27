---
#### Spanning Tree Protocol:
>stp is a layer 2 protocol it enables redundant layer 2 networks.
>stp solves the problem of broadcast storms by disabling some switch interfaces in the network and solve the problem of mac address flapping.
>classic spanning tree is an industry standard protocol IEEE 802.1D
>stp prevent loops by placing the redundant ports in a blocking state disabling the interface 
>these interface acts as a backup that can enter a forwarding state when one interface fails.
>by selecting which ports are forwarding and which are blocking stp creates a path to and from a network this prevents layer 2 loops.
>stp enabled switches send and receive bpdus from their interface every 2 seconds. If a switches receive a bpdu on an interface it knows that it is connected to another switches becuz routers and pc dont use bpdus 
>switches uses the bridge id field in the bpdu to elect the root bridge for the network other switches in the network will need a path to reach the root bridge 
>the switch with the lowest bridge id becomes the root bridge 
>all ports in the root bridge are in the forwarding state 
>the switch with the lowest bridge id is elected as root bridge 
>bridge id = priority + mac address

#### Ports states:
>1. Blocking:
>2. listening
>3. learning
>4. forwarding
>