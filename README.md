# ETTTP
This is 5*5 tic-tac-toe game w/ chatting board~!

~ENJOY~


2025.05.11 troubleshooting : 
1. both ready(hold)...
2. only one side chatting

### HOW TO RUN GAME
1. python ETTTP_Server_skeletion.py
2. python ETTTP_Client_skeleton.py

## Preview..
![img.png](img.png)
## Project Goal: Online Tic-Tac-Toe game

▫ Socket: Client – Server (TCP connection)

▫ Functionality: Peer-to-Peer

▫ We will say Peer that take role of Server as Server Peer and Client as Client Peer

▫ Based on an application message protocol called Ewha Tic-Tac-Toe Protocol (ETTTP)

   - Exchange my new move with peer in real-time
 
   - Send the final result poll for verifying the winner

## Project Specification – Overall Flow

1) Client-Server TCP Connection 
    - Use port number of 12000
2) Once TCP connection is established, open the GUI window at each client and server
3) Server randomly selects who is going to be the first mover (Mark: X) and shares with the client
4) Only the user with the correct turn can click on a certain area
    - Invalid user’s input should neither change the board status nor send any message to the peer
    - If the selection is valid, send message to peer
5) Each client or server needs to continously check whether the game is over
6) Then, the result is shared with the peer
7) Both server and client double-check if the results are same, and then, the game is over
