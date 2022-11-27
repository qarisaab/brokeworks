#### DTP:
>DTP is a cisco protocol that allows cisco switches to dynamically determine their interface status like trunk or access without manual configuration.
>dtp has two modes dynamic auto and desirable
>disable dtp with this command `switchport nonegotiate` 

#### VTP:
>vtp allows you to configure vlans on a central server switch and other client switches will sync their data base to the server switch.
>switches operate in vtp server mode by default
>will increase the revision number every time a vlan is added or deleted 
>will advertise the latest version of the vlan data base on trunk interfaces and the vtp client will sync the database to it 
>vtp server also functions as vtp clients
>and a vtp server can also sync to another vtp server with the high ***revision number***
>
