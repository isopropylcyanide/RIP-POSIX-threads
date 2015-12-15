This is a very light implementation of Routing Information Protocol (Networking) using POSIX Threads.

The idea is to have some n number of files in the directory names ($n.txt). These files represent routers. 
In each file there are three space separated columns.

Col-1 Col-2 Col-3

Col-1: This is the name of the router file. 
Col-2: This is the distance between the router whose name is specified in col-1        and with the router whose file you have currently opened. 
	If this distance is:
		"1" : directly connected
		"2" : connected at a distance of 2 metres. (1 metre for directly connected)
		...
		"16": not reachable, infinite distance.

	Hence, the maximum distance reachable is 15

Col-3: This specifies the next hop destination to reach the router whose name is specifies in Col-1. A hop of 0 , means no hop is required. Initially, there are obviously no hops


#Things you can do currently ( First Release)

*****MENU*******

1: Add a router: 

2: Fail a link:

3: Add a link:

4: Invalidate a router

5: Revalidate a router

0: Exit simulation:

All of these actions have been carefully studies and implemented. I would appreciate if someone could come up with their bugs or an efficient code perhaps.

Note: 1: Add a router => You don't create a new file. The new router remains in memory. The initial router files are just for initiation since I needed File Handling as the initialisation approach.


You are free to suggest changes.
