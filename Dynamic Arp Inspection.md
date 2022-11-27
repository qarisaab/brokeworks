---
#### what is ARP:
>arp is used to learn the mac address of known ip address it used to learn the mac address of the default gateway when sending traffic to another network. ARP request is a broadcast msg that has all fffffs in its mac address field.

#### Gratuitous ARP:
>It is a type of arp reply that is send without an arp request.
>it is send to the broadcast mac address. It allows other devices to learn the mac of the sending device without having to send the arp request.

#### Dynamic Arp inspection:
>DAI is the security feature of switches that is used to filter arp messages that are received on untrusted  ports. all ports are untrusted by default.
>typically all ports that are connected to network devices should be trusted and ports connected to end devices should be untrusted.
>when an arp msg is arrived on an untrusted port the dai will inspect the packet if it is okay it will forward it as normal

#### ARP Poisoning:
>An arp poisoning is an attack in which the attacker sends gratuitous arp reply using an other devices ip address and the devices in the network update their arp table to match the ip of the garp to the attacker device mac address and thats how we perfrom mitm.

#### Dynamic ARP inspection Operations:
>DAI inspects the msg the sender send to the untrusted ports and dai inspects the msgs using the dhcp snooping table to check if there is an binding entry if there is an entry the packet is forwarded normally and if there is no matching entry the arp msg is discarded.

#### DAI Configuration:
>`ip arp inspection vlan1`  "it is used to enable arp inspection on the vlan "
>`interface range ` "it is used to select the range of interfaces "
>`ip arp inspection trust` "it is used to make the interface as a trusted port"
>`show ip arp inspection interfaces` "used to show the arp inspection interfaces"
>`ip arp inspection limit rate 25 burst interval 2` "used to configure rate limiting"
>if arp msg are received faster than the specified rate the interface will be errdisabled


