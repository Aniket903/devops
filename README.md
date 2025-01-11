Docker network

In Docker, networking is a crucial aspect that allows containers to communicate with each other, the host, and the outside world. Docker provides several network drivers, and understanding them is essential to setting up proper communication between containers in a containerized application.



1.	Bridge network:-
In Docker, a bridge network is a private network that containers can connect to for communication. It is the default network type created by Docker if no specific network is specified when running a container.
Note:it is used for comminucating between containers in a network.
2.	Host network:-
In Docker, the host network is a special network mode that allows a container to share the host system's network stack. When a container runs with the host network, it directly uses the host's network interfaces, bypassing Docker's networking abstraction.
Note:it is used for communicating with localhost (root).it doesn’t have ip address assigned.
3.	Overlay network:-
In Docker, an overlay network enables communication between containers across multiple Docker hosts. It is commonly used in Docker Swarm or with Docker Compose in a Swarm mode setup.
Note:it is used   for communicating between different networks. 
4.	None network:-
In Docker, the none network is a special network mode that completely disables networking for a container. When a container is run with the none network mode, it has no network interfaces except for the lo (loopback) interface.
Note:if we don’t want our container to communicate with any other container with network we can use none network.  
5.	Macvlan network:-
In Docker, a macvlan network allows containers to appear as physical devices on the host's network. Each container connected to a macvlan network gets its own unique MAC address and appears as a separate device on the physical network. This is useful for scenarios where containers need direct access to the network and must bypass the host’s network stack.
![image](https://github.com/user-attachments/assets/c6b618b4-8816-46ba-8294-8da58895bd57)
![image](https://github.com/user-attachments/assets/a5812ec8-8d6f-449b-984e-c3995cffe786)



 

 
