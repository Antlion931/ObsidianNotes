#cybersecurity #pwr 

**S**ender **P**olicy **F**ramework records list all [[IP]] adreses and servers that are allowed to send mails from some domain. To check if email that you have recived is really from domain it claims to be, you can fallow this steps:

## 1. Check [[IP]] of sender
If you are a server, it is pretty simple, but if you want to check [[IP]] of sender in your mailbox, you could use option called `original message` or something like that. Then find a line that tells you about [[SPF]]

> spf=pass (google.com: domain of 0102018f10d1841b-bdc413f0-f630-484d-be45-d139151a7ed6-000000@eu-west-1.amazonses.com designates 54.240.106.159 as permitted sender) smtp.mailfrom=0102018f10d1841b-bdc413f0-f630-484d-be45-d139151a7ed6-000000@eu-west-1.amazonses.com;

There you can see that [[SPF]] test have passed, and `54.240.106.159` is permitted sender. 

## 2. Check from which domain it claims to be
To check that you need 


- [ ] #todo Write about [[SPF]] 