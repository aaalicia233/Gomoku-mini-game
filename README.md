# Gomoku battle game

# Introduction 


# Environment
A Gomoku battle mini-game that runs on Linux.

# Install
To install the game on a Linux system, you can directly extract the downloaded project and then execute the following two commands:
If you are playing over a LAN, you need to modify the IP address in client.c (line 10), changing it to the server's IP address.
```bash
make -f makefile_server
make -f makefile_client


```
# Usage
After installation, you can start the project by executing the following commands.
Note: If you are playing against yourself, you will need to open two terminal windows to start the server and client separately (make sure to start the server before the client).
```bash
./bin/server
./bin/client
```

```
PORT:8888 IP:127.0.0.1
0 1 2 3 4 5 6 7 8 9
1 _ _ _ _ _ _ _ _ _
2 _ _ _ _ _ _ _ _ _
3 _ _ _ _ _ _ _ _ _
4 _ _ _ _ _ _ _ _ _
5 _ _ _ _ _ _ _ _ _
6 _ _ _ _ _ _ _ _ _
7 _ _ _ _ _ _ _ _ _
8 _ _ _ _ _ _ _ _ _
9 _ _ _ _ _ _ _ _ _
Gomoku game starts
Please wait for the client to make a move
0 1 2 3 4 5 6 7 8 9
1 _ _ _ _ _ _ _ _ _
2 _ _ 0 _ _ _ _ _ _
3 _ _ _ _ _ _ _ _ _
4 _ _ _ _ _ _ _ _ _
5 _ _ _ _ _ _ _ _ _
6 _ _ _ _ _ _ _ _ _
7 _ _ _ _ _ _ _ _ _
8 _ _ _ _ _ _ _ _ _
9 _ _ _ _ _ _ _ _ _
Server, please make a move:
4 3
0 1 2 3 4 5 6 7 8 9
1 _ _ _ _ _ _ _ _ _
2 _ _ 0 _ _ _ _ _ _
3 _ _ _ _ _ _ _ _ _
4 _ _ * _ _ _ _ _ _
5 _ _ _ _ _ _ _ _ _
6 _ _ _ _ _ _ _ _ _
7 _ _ _ _ _ _ _ _ _
8 _ _ _ _ _ _ _ _ _
9 _ _ _ _ _ _ _ _ _
```

# TODO 
* Separate the server component to allow multiple clients to connect
* Support for multiplayer battles
