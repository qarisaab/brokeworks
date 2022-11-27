#### IP phones:
>traditional phones operate over the public switched network (pstn)
>ip phones uses voip to enable phone calls over an ip network. it has an internal 3 port switch one is used to connect to the switch one to the pc and one is connected internally to its self.
>this the pc and ip phone to share a single switch port. traffic from the pc passess through the ip phone to the switch.
>voice traffic is to be separated from the data traffic by placing them in different vlans

#### POE:
>Poe allows power sourcing equipment pse to provide power to the pd powerd device over an ethernet cable. pse is a switch and pd are ip phones , ap, or an ip camera.

#### QOS:
>it is a set of tools used by the network devices to apply different treatment to different packets.
>1.bandwidth: 
>the overall capacity of the link measured in kbps,mbps for eg 20%voice traffic, 30%
>for specific kind of data traffic.
>2.Delay:
>the amount of time it take traffic to go from one source to destination is called as one way delay.
>3.Jitter:
>the variation in the one way delay between packets from the same application.

#### Queuing:
>if a network device receive msgs faster than it can forward out of the interface the msg are placed in the queue. if the queue becomes full the packets are dropped this is called as tail drop and it can lead to something called as tcp global synchronization. A solution to prevent tail drop and tcp global synchronization is random early detection which drop selected tcp packets when the amount of traffic in the queue reaches a certain threshold the device will start RED.
>WRED is also a improved version of the red. an essential part of the qos is the use of the multiple queues. the device can match traffic on various factors and place then place it in the appropriate queue. but the interface can forward one frame at a time so a schedular is used to decide which queue traffic is forwarded from next

#### Classification:
>the purpose of the qos is to give priority to certain kinds of traffic over the others during network congestion. it organizes the network traffic into traffic classes. it is important to classify and identify traffic to give priority to it many method to identify or classify traffic:
>acl, nbar, pcp in the dot1q field and then there is the dscp field 
>pcp is also known as class of service.
>dscp uses 4 types of values for qos
> 	1. default forwarding
> 	1. expediated forwarding
> 	2. assured forwarding
> 	3. class selector

#### Trust Boundary:
> the trust boundry of the network is boundry in which the qos marking are trustred and forwarding without changing them if the marking are not trusted the device wil change the marking and forward them.