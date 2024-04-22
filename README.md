
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
## PROGRAM:
# client:
import socket

s = socket.socket()

s.connect(('local host',8000))

while true:

msg = input("client>")

s.send(msg.encode())

  printf("server>",s.recv(1024).decode())

# server:
import socket

s=socket.socket()

s.bind(('localhost',8000))

s.listen(5)

c,addr=s.accept()

  while True:
 
  ClientMessage=c.recv(1024).decode()
  
  c.send(ClientMessage.encode())
## OUPUT
![image](https://github.com/deepika3095/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/151625159/d6a7246f-2cd5-4d79-91be-364337699584)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
