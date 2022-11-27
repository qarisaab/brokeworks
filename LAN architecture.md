## some general terms:
#### star:
>when one devices connect to one central devices it is called as a star.

#### full mesh:
>it is when each devices are connected to each other.

#### Partial mesh:
>it is when some devices are connected to each other.

## Two tier design:
#### Access Layer:
> it is the layer that connect to the end host qos marking is also done here. Port security is also done here and poe is also present there.

#### Distribution Layer:
> these switches aggregate connections from access layer 
> this is the border between layer 2 and layer 3
> it is used to connect to service such as wan and the internet. 

#### Core layer:
> In the networks when there is more than three distribution switches we can add a core layer and each distribution switch connects to the core layer connections in core layer is layer 3 no spanning tree is needed.

#### Spine leaf:
>Data center are dedicated spaces and buildings used to store computer systems such as servers and network devices.
>traditional data centers used to use 3 tier network design cuz was the traffic was north south
>with the increase in east west traffic spine leaf was developed 
>in spine leaf every leaf switch is connected to every spine switch
>leaf and spine switches dont connect to each other.

#### small office home office (soho):
>In soho networks there is only a single network device that function as a router and a switch called as wireless router.