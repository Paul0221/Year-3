
![[Pasted image 20231023233100.png]]

- Not intended for the internet
- Applies to general networks

The 7-layer OSI Reference Model uses a 7 layer stack:

- Application layer - contains user-facing protocols (e.g. ftp, http, smtp)
- Presentation layer - interprets data and includes compression, encryption protocols and data description
- Session layer - organises and structures dialogue between apps (i.e. delimiting and synchronisation)
- Transport layer - accepts & splits session data into packets for Network layer or receives & constructs data segments for Session layer (i.e. host-to-host communication)
- Network layer - controls the operation of the sub-network between hosts by determining how datagrams are routed dynamically
- Link layer - handles movement of packets from node-to-node along the route (e.g. ethernet, Wi-Fi etc)
- Physical layer - handles movement at bit level and is purely hardware (e.g. copper wire, fibre optic, radio waves etc)

Advantages of OSI model:

- Clearly defined layers and protocols
- Can be applied to any network (e.g. defence, cash machines etc)

Disadvantages of OSI model:

- Often overly complex
- Presentation and Session layers could be merged as they have minimal functionality