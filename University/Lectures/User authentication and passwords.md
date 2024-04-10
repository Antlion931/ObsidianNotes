#cybersecurity #pwr 

# Authentication
![[authentication]]

It is prevalent to use passwords for [[authentication]]. But it only works on some assumptions:
- Server can be trusted
- There is safe communication channel between user and server. No one else can eavesdrop.
## Storing passwords on Server

Data on servers can always be leaked, so it's important to assume that it will be leaked some day. That's why it is vary bad to store passwords in plain text, as data leak would mean immediate access to every user login credentials. To fight against it, people thought about few things:
- Hashing a password, meaning transforming it into different sequence of bits, such that it is impossible to reverse. Then if someone wants to log in into it account, the password user entered is hashed, and compered with that on server. Thanks to that after leaking a data, you still need to do a lot of work to get user's password. What hash function to use is under constant change, GPU are getting better and better, and people finds better and better hash functions. Current recommendation are [here](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html).
- People tends to have short and simple passwords, meaning decryption of a hash is faster. That's why every person in database have his unique **salt**, which is random sequence added to password before hashing. Meaning a bandit have a harder time decrypting a hash, and also some methods, like pre-computing hashes, are not so effective.
- **Salt** is on server, and it still will be leaked. That's why some servers use **pepper**, which is a secret strategy that's adds additional layer of protection. For example after hashing, we will use another function like **HMAC** with **pepper** as an secret key. It is important not to store **pepper** on server. 
## Other problems with passwords
- Short and easy to break passwords
- using the same password in different service
- phising
- If we demand more secure passwords from people, safety get worse. For example with cycle passwords that needs to be changed once per month, people will make very easy passwords because they don't want to waste time.
# Brute force attacks
![[Hashcat]]


- [ ] #todo Continue watching lecture 1 from 40 minute.