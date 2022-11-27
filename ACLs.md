---

#### what are acls:
>They are used to control the access to the network in which what device should access what in the network.
>acls are used to function as packet filter instructing the router to discard or permit the traffic
>acls can filter traffic based on source and destination ip and port 
>there is an invisible entry at the called as the implicit deny

#### standard ACLs:
>standard acls are the acls that match based on the source ip address there are also two types of standard acls:
>- standard numbered acls 
>- standard named acls
>numbered acls are identified with a number acl1, acl2 and acl3
>different type of acls have a different range of numbers that can be used standard acls use from 1-99 and 1300-1999 
>A good rules is that standard acls should be applied as close to the destination as possible.

#### standard named acls:
>standard named acls are also the standard acls that filters the traffic using the source ip address of the packet ,
>instead of the number they are identified by using a name rather than the number.

#### Extendend ACLs:
>entries can easily be deleted with the acl config mode with no and then the sequence number
>you can new entries in between other entries by specifying the sequence number 
>there is also a function that is used to resequence acls `ip access list resequence`
>extended acls have range from 100-199 and 2000-2699
>however they can match more parameters.

|ports|number|
|---|---|
|22|ssh|
|20|ftp data|
