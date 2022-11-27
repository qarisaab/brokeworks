---

#### why ipv6:
>there are just arent many ipv4 address the permenant solution is transition to ipv6
>ipv4 address are assigned by the IANA and IANA distributes ipv4 to the RIRS regional internet registries which them assign them to the companies that need them
>An ipv6 address is 128 bits 
>ipv6 has 8 quartets with hex digits the first 48 bits of the address are the global routing prefix and the next 16 bits are the subnet id and the last 64 bits are the host identifier. the global routing prefix and the subnet id are used to make the network portion of the address and the last 64 bits represent the host id.
>use the command `ipv6 unicast routing`

#### EUI 64:
>eui stands for extended unique identifier. method of converting mac address into interface identifier
>this then becomes the host portion of the ipv6 address
>eui 64 is a method not a type of ip address.

#### Global unicast address:
>global unicast address are the type of public address that we have to register to use them they cannot be used without registering them. since they are public it is expected that they are unique over the internet.
>the block of global unique address 2000::/3 to 3FFF::

#### unique local address:
>unique local address are the address that cannot be used over the internet and they are used as private address. they can be used in the internal networks the address block FDFF. they can also be routed in the private networks 

#### Link Local address:
>link local address are the address that are automatically generated on ipv6 enables interface. the command to enable `ipv6 enable`
>FE80.
>link local means that these address are used for communication with in a subnet router will not route packets with a link local destination ipv6 address 

#### Multicast address:
>multicast address are used for one to many communication one source to multiple destination.
>they use a the group FF00/8 FFFF

#### anycast address:
>anycast ipv6 address are the address that is used to for communication to one to one of many 

#### ipv6 header:
>ipv6 has a fixed header of 40 bytes and is much simpler than the ipv4 header:
>1. version field 
>2. traffic class 
>3. flow label 
>4. payload length 
>5. next header
>6. source address
>7. destination address

#### NDP:
>ndp uses icmp v6 and solicited node multicast address to learn the mac address of the other host
>another function of ndp is that it allows host to automatically discover routers on the local network two msgs are used for this:
>1. RS
>2. RA
>rs msgs are sent to the multicast address ff02::2 all routers multicast address when a host is connected to the network and ask all the router on the local link to identify themself 
>ra msgs are sent in response to the rs msgs it uses the icmp v6 type 134 msg type and are sent to the multi cast address ff02::1 all nodes multicast address. however even if the router doesnt recieve an rs msg it will send ra msgs preodically.