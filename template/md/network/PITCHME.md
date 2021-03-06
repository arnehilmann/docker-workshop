---?image=template/img/network.jpeg

@title[Docker Network]

@snap[north text-black span-100]
@fa[terminal fa-2x](Docker Network)
@snapend

+++
@title[Network drivers]

@snap[north-west]
### Network drivers
@snapend

@snap[north-east]
### [@fa[info]](https://docs.docker.com/network)
@snapend

@snap[west span-100]
@ul[](false)
- bridge
- host
- overlay
- macvlan
- none
- Network Plugin
@ulend
@snapend


+++
@title[bridge]

@snap[north-west]
### Bridge
@snapend

@snap[north-east]
### [@fa[info]](https://docs.docker.com/network/bridge)
@snapend

@snap[west span-100]
@ul[](false)
- Default driver
- Software bridge 
- Isolation from host / other bridges
@ulend
@snapend

+++

@title[Overlay]

@snap[north-west]
### Overlay
@snapend

@snap[north-east]
### [@fa[info]](https://docs.docker.com/network/overlay)
@snapend

@snap[west span-100]
@ul[](false)
- Default driver for Docker Swarm
- On top of host-specific network
- Containers can only communicate across networks
@ulend
@snapend

+++

@title[Network Plugins]

@snap[north-west]
### Network Plugins
@snapend

@snap[north-east]
### [@fa[info]](https://docs.docker.com/engine/extend/plugins_services/#volume-plugins)
@snapend

@snap[west span-100]
@ul[](false)
- Only for Docker Swarm
- Adds encryption and discovery
@ulend
@snapend

+++
@title[Exercise]

@snap[north-west]
### Exercise
@snapend

@snap[west span-100]
@ol[](false)
- Create two networks
- Run a nginx container with name 'web1'
- Start alpine container in same network and curl web1
  (Hint: `apk add curl; curl web1`)
- Start same container again in the other network and try curl
@olend
@snapend

+++?code=template/md/network/example.sh?lang=sh
@title[Answer]
@snap[north-west]
### Exercise (Answer)
@snapend

@[1-3]
@[5-6]
@[8-13]
@[15-19]
