# client_server_tcp

Language:

C ANSI 99


Assignment:

* Develop a client server tool to send files via TCP socket.


Specifications for the client:

* Command line utility.
* Receives three parameters
  * Full path to the file to send
  * Destination IP
  * Destination Port
* Prints out to standard output each file sent including the bytes sent.
* Prints out to standard error any errors.
* Written in ANSI C 99


Specifications for the server:

* Command line utility.
* No multithreaded/concurrency required.
* Receives three parameters:
  * Folder where the received files will be stored.
  * Listening IP
  * Listening Port
* Preserves the original name of the received file but not the path.
* Prints out to standard output each file reception including the file name and its size.
* Prints out to standard error any errors.
* Written in ANSI C 99


Deliverables:

* Code (or git)
* Live demo
* Walkthrough, Q&A session


Build and Run

Server:
-Enter the server folder and type the following command:
> gcc server.c -o server && ./server [folder name]/ [your ip address] [port number]

Client:
-Enter the client folder and type the folloing command:
> gcc client.c -o client && ./client [file name] [destination ip] [destination port]
