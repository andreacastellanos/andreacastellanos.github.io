---
layout: default
title: Chat Room Server and Client
type: project
permalink: projects/chat-room-server-and-client
---

Basic server and client programs. 

Makefile is included, "make server" and "make client" in order to compile both server and client. 

Default port is 0628. Run server first, then run client. You can also use PuTTY as client and connect via port 0628.

In order to send a message use the following format:
 
    SAY <your username> <your message>
    
In order to leave the chat room (this will close the program):

    LEAVE <your username>


`Makefile:`

![makefile](/assets/images/projects/chat room server and client/makefile.png)


`Server:`

![server](/assets/images/projects/chat room server and client/server.png)


`Client:`

![client](/assets/images/projects/chat room server and client/client.png)

[back](./)