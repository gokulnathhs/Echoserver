# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
## CLIENT:
```
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'GOKUL NATH H , 212222040045')
    print(f'Received: {s.recv(1024)!r}')
```

## SERVER:
```
import socket
host,port='127.0.0.1',65432
with socket.create_server((host,port))as s:
    conn,addr=s.accept()
    with conn:
        print(f'connected by {addr}')
        while data :=conn.recv(1024):
            conn.sendall(data)
```

## OUTPUT:
![Screenshot 2025-03-06 113137](https://github.com/user-attachments/assets/5281c513-757b-4de7-86a5-9047b3229796)



## RESULT:
The program is executed successfully
