#### LAN:
>A lan is a single broadcast domain. A frame with destination mac of all Fs 

#### Trunk Ports:
>switches will tag traffic that they send over the trunk link this allows the receiving switch to know which vlan the traffic belongs to.

#### Native VLAN:
>dot1q also has a feature called native vlan the native vlan is vlan 1 by default on all trunk ports however this can be manually configured on each trunk port. the switch does not tag the frames in the native vlan. when a switch receives an untagged port it assumes that it belongs to the native vlan.**it is important that the native vlan must match ** 

#### What is a layer 3 switch:
>it is a switch that is cable of routing and switching 