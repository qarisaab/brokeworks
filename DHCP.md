#### DHCP:
>dhcp is used to allow hosts to automatically learn various aspects of their network configuration such as ip address, subnet masks, default gateway, dns server etc without manual/static configuration.
>dhcp is an essential part of the modern network 
>dhcp is used for client devices
>devices such as servers, routers are manually configured 
>dhcp server use upd 67
>dhcp clients use udp 68

#### relay:
>some network engineers might choose to configure a centralized dhcp server if the dhcp server is centralized it wont receive dhcp msgs outside of the local subnet cuz broadcast traffic is dropped by the router to fix this we can use a router to act as a dhcp relay agent the router will forward the client broadcast dhcp msgs to the remote dhcp server as a unicast msg
>to configure the relay agent use the command on the interface connected to the clients
>`ip helper address` 
