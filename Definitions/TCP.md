#programmingChallenges 

**T**ransmission **C**ontrol **P**rotocol is used in web to send files, browse internet and sending mails. It ensures that no information is lost, but in trade of speed. [[TCP]] requires establishing connection by three-way handshake.

![[TCP_Three_way_handshake-3127118050.jpg]]

## Why three-way handshake?

It is because of how this protocol works. Both of host have some number that they use to tell the other side what they have received and what they need. Read it as:

>Alice ---> Bob  '**SYN**chronize with my Initial Sequence Number of `X`'
Alice <--- Bob   'I received syn, I **ACK**nowledge that I am ready for `X+1`'
Alice <--- Bob   '**SYN**chronize with my Initial Sequence Number of `Y`'
Alice ---> Bob   'I received syn, I **ACK**nowledge that I am ready for `Y+1`'

Both `X` and `Y` start at 0, and are then increased by length of the data.
# About [[TCP]] Header

![[header.png]]

Most commonly [[TCP]] is used in par with [[IP]].

![[flags.png]]

Type of message is set by corresponding flags, There are other feature like Checksum.

# Window size
Name is misleading, because [[TCP]] is layer of sending data, and size of users windows is not in the interest of [[TCP]]. What's more it could be used to communicate between two devices, that doesn't use any output for users. 

So what does it mean? It means how much data can be send without acknowledge. If Everything is okey, it will grow. If there are a lot of problems, like missing packets, it will shrink. So that [[TCP]] could speed up. If connection is great, It will send more packets because it knows more of them will be received. And the other side will not be flooded with out of order packets when connection is bad.

# How it deals with problems
![[ack_and_syn.png]]

After sending a data we increase our sequence number, and after every received data, we need to respond with our **acknowledged number** increased by length of data.

![[ack.png]]

If receiver didn't acknowledge anything after some time. Perhaps data was lost. That's why we will send it again.

![[tcp_waiting.png]]

But what if receiver will get multiple or out of order packets? It's simple, firstly it check what **acknowledge number** it last sent. If it is smaller then **sequence number**, then we need to wait for some packet. If it is the same, our **acknowledge response** did not come, perhaps is lost. That why we should send it once again.

# Ending Connection
Similarity to establishing connection, but with different flag.

![[tcp_closing.png]]

# Differences to [[UDP]]

- [ ] #todo Write about differences between [[TCP]] and [[UDP]].

