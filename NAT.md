
#### nat:
>nat stands for network address translation it is one of the short term solution for the exhaustion of the ipv4 address space the short solutions are:
> 1. cidr
> 2. private ipv4 address
> 3. nat

##### private ipv4 address:
>it includes the range from 10.0.0.0/8 to 10.255.255.255
>172.16.0.0/12 to 172.31.255.255
>192.168.0.0/16 to 192.168.255.255
>private ip address can be used over the internet

#### nat:
>nat is used to modify the source or destination address of the packet when it arrives at the router to a public ip address

#### static source nat:
>it involes mapping one to one address an inside local address is mapped to an inside global address
>inside local is the ip of the inside host from the local network
>inside global is the ip address of the inside host from the outside network

#### Dynamic Nat
>in dynamic nat the router dynamically maps the private address to public address.
>an acl is used to identify which traffic should be translated and which should not be translated.

#### PAT
>pat also called as nat overload translates both the port number and the ip address if necessary
>by using a unique port number for every communication flow a single public ip address can be used by many different hosts. the mapping are one to many.
>same command as the dynamic nat with just the keyword overload.


 
