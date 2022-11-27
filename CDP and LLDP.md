---
#### CDP:
>cdp is known as cisco discovery protocol 
>they are layer 2 discovery protocols. they are used to share information about the connected devices such as device name host name and ip address it is an industry standard protocol ieee 802.1AB.
>cdp messages are sent to mutlicast mac address of 0100.0CCC.CCCC
>cdp messages are sent once every 60 seconds. and they have a hold time of 180 seconds

#### LLDP:
>lldp stands for link layer discovery protocol 
>it is the industry standard protocol 802.1AB
>lldp msgs are sent to multi cast mac address 0180.c200.000e
>these msgs are send once every 30 seconds 
>hold time of lldp is 120 seconds.
>to enable lldp use `lldp run`
>to enable on an interface use `lldp transmit` and `lldp receive`
