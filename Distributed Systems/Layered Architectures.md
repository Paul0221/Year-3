
Types of layered architectures:

- Pure Layered Organisation 
![[Pasted image 20231018124022.png]]
- Mixed Layered Organisation
![[Pasted image 20231018124107.png]]
- Layered Organisation with Upcalls
![[Pasted image 20231018124203.png]]
	- The handle (installed in Layer N-2) allows Layer N-1 to subscribe to an area of interest in Layer N-2 so that once it is available, an upcall is made to Layer n-1
	- This goes against standard network principles but is allowed in distributed systems

Application Layering using the PAD model:

- Presentation Layer - contains everything required to interface with the user
- Application Layer - processing layer containing core functionality of the system
- Data Layer - responsible for persistent storage of the data on which the application operates

PAD model maps these layers onto a physical client-server architecture in various ways