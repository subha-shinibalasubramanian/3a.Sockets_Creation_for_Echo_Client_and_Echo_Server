# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.  

**NAME:SUBHASHINI.B**  
**REGISTER NUMBER :212223040211**  
## PROGRAM
## SERVER

```
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
  ClientMessage=c.recv(1024).decode()
  c.send(ClientMessage.encode())

```
## CILENT

```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())

```
## OUPUT
## CILENT 

![image](https://github.com/subha-shinibalasubramanian/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/164154478/de4eaf19-2929-4c66-96a4-1757743c03ba)

## SERVER

![Screenshot 2024-04-29 132415](https://github.com/subha-shinibalasubramanian/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/164154478/9dc38011-9d65-4f56-9805-2f2cf29cf1fa)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
