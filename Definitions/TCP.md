#programmingChallenges 

**T**ransmission **C**ontrol **P**rotocol is used in web to send files, browse internet and sending mails. It ensures that no information is lost, but in trade of speed. [[TCP]] requires establishing connection by three-way handshake.

![[TCP_Three_way_handshake-3127118050.jpg]]

## Why three-way handshake?

It is because of how this protocol works. Both of host have some number that they use to tell the other side what they have received and what they need. Read it as:

>Alice ---> Bob   '**SYN**chronize with my Initial Sequence Number of X'
Alice <--- Bob    'I received syn, I **ACK**nowledge that I am ready for X+1'
Alice <--- Bob    '**SYN**chronize with my Initial Sequence Number of Y'
Alice ---> Bob    'I received syn, I **ACK**nowledge that I am ready for Y+1'

Where X and Y are some random numbers

## Differences to [[UDP]]

- [ ] #todo Write about differences between [[TCP]] and [[UDP]].
