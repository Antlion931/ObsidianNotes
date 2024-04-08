#cybersecurity #pwr 

# Authentication
![[authentication]]

It is prevalent to use passwords for [[authentication]]. But it only works on some assumptions:
- Server can be trusted
- There is safe communication channel between user and server. No one else can eavesdrop.
## Storing passwords on Server

Data on servers can always be leaked, so it's important to assume that it will be leaked some day. That's why it is vary bad to store passwords in plain text, as data leak would mean immediate access to every user login credentials. 

- [ ] #todo Write about salt and hashing passwords, then continue watching lecture 1 from 30 minute.