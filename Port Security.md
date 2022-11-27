#### Port Security:
>it is the security feature of the cisco switches. It allows which source mac address are allowed to enter the switch port per interface. If an unauthorized frames enter the port the port is set to an err disable state. by default only one mac address is allowed on the interface and you can configure it manually.
>port security is useful because it allows the admins to allow which devices are able to access the network.
>port security can be applied only on access and trunk ports mode and in static mode dtp is not allowed.
>sticky secure mac address are the address that will never age even if the static aging is enabled

#### Commands:
>`show port security interface `
>`errdisable recovery cause psecure violation`
>`errdisable recovery interval`

Violation mode:
>threre are three violation mode 
>1. shutdown: disable the port and generate a syslog msg
>2. restrict: discards the  unauthorized traffic and generate a syslog msg and violation counter is incremented by 1.
>3. Protect: discard the unauthorized the traffic and silently discards the traffic