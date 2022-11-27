#### DHCP snooping:
>securtiy feature of switches that filter dhcp messages on the trusted ports.
>uplink ports should be trusted and downlinks port should be left untrusted.

#### DHCP exhaustion:
>when an attacker uses a spoofed mac address to flood dhcp discover msgs the dhcp server pool becomes full resulting in a dos.

#### DHCP Poisoning:
>when an attacker run a dhcp software in local network and the legit  dhcp server is in remote network a spurious dhcp server can reply to the client dhcp discover msgs and assign them ip address but makes them use the spurious dhcp servers ip as the default gateway. this will cause the clients to send the traffic to the attacker as it is there default gateway

#### DHCP messages:
>when dhcp snooping filters msgs it differentiate between the server and client msgs 
>dhcp server msg on untrusted ports are discarded 
>dhcp clients msgs on untrusted ports are inspected
>dhcp server msg:
>1. offer
>2. ack
>3. nak
>dhcp client msg:
>1. Discover
>2. Request
>3. Release
>4. Decline

#### DHCP snooping operation:
>* if a dhcp msg is received on a trusted port it is forwarded as normal
>* if a dhcp msg is received on an untrusted port it is inspected
>* dhcp server msg are declined
>* mac address in the chaddr and source mac field should match
>* for release/decline msg check if the source ip and dhcp binding table match

##### Important commands:
>`no ip dhcp snooping information option`




