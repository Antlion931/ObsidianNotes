#programmingChallenges 

[[Socket]] is a endpoint of a communication over internet. It is an abstraction that helps in communication. It is build mainly from 3 things. 
- Local [[IP]]
- Local [[Port]] number
- Which protocol to use in communication for example [[UDP]] or [[TCP]]


It is used in programming as a low level way of interacting with network. Mostly by calling function like:

```
.listen()
.connect()
.write()
.read()
```

![[network_socket.png]]

You can list all of your sockets in use with [[lsof]] command on linux.