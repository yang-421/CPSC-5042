CPSC-5042
This is the repository for team project of CPSC 5042

Items needed for milestone 1:

Server.cpp
	Opens socket (done)
	Binds socket (done)
	Listens for connections (done)
	Validates user login credentials
	Creates new thread for user
	Handles user disconnects gracefully (shuts down threads, sockets etc)
	Stretch goal 1: Support Multiple client connections simultaneously 
	Stretch goal 2: Design/implement RPCs that allow threads to talk for multiplayer
	Stretch goal 3: Hash user credentials and store in/look-up from external file 
Client.cpp
	Client needs to establish connection, run connect(name, password), wait a random amount of time from 1-10 seconds, then run disconnect()
	Connect to server with username and password
		Function signature: int connect(char *userName, char *password)
	Disconnect gracefully from server
	Stretch goal 1: Let client choose 1 player or 2, load appropriate logic from server based on choice
Design a minimum of THREE (3) additional calls/requests between the client and server
	RPC 1: TBD
	RPC 2: TBD
	RPC 3: TBD
Project documentation (Milestone1.PDF)
	Summary of project (2 paragraphs) (done, tentatively)
	Listing of FIVE (5) RPCs including their signatures, input arguments, output and a description
	Screenshot of output from CS1 showing server.cpp and client.cpp running/working
	Makefile info for how to compile the .cpp’s and run the programs.
Milestone1.zip
	Client.cpp
	Server.cpp
	Client executable
	Server executable
	Makefile
	Milestone1.pdf
