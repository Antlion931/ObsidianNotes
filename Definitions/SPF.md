#cybersecurity #pwr 

**S**ender **P**olicy **F**ramework records list all [[IP]] adreses and servers that are allowed to send mails from some domain. To check if email that you have recived is really from domain it claims to be, you can fallow this steps:

## 1. Check [[IP]] of sender
If you are a server, it is pretty simple, but if you want to check [[IP]] of sender in your mailbox, you could use option called `original message` or something like that. Then find a line that tells you about [[SPF]]

> spf=pass (google.com: domain of 0102018f10d1841b-bdc413f0-f630-484d-be45-d139151a7ed6-000000@eu-west-1.amazonses.com designates 54.240.106.159 as permitted sender) smtp.mailfrom=0102018f10d1841b-bdc413f0-f630-484d-be45-d139151a7ed6-000000@eu-west-1.amazonses.com;

There you can see that [[SPF]] test have passed, and `54.240.106.159` is permitted sender. 

## 2. Ask [[DNS]] server
For example using a command:

>[[dig]] netflix.com txt

We can get access to information about allowed [[IP]] address, here is a line that we are looking for:

>netflix.com.		129	IN	TXT	"v=spf1 include:_spf_ipv4.netflix.com include:_spf.google.com include:amazonses.com include:servers.mcsv.net include:_spf.salesforce.com include:_spf.createsend.com -all"

There is no `54.240.106.159`, however it says that allowed [[IP]] addresses are borrowed from other domains, like `amazonses.com`. And after:

>[[dig]] amazonses.com txt

we get:

> amazonses.com.		900	IN	TXT	"v=spf1 ip4:199.255.192.0/22 ip4:199.127.232.0/22 ip4:54.240.0.0/18 ip4:69.169.224.0/20 ip4:23.249.208.0/20 ip4:23.251.224.0/19 ip4:76.223.176.0/20 ip4:52.82.172.0/22 ip4:54.240.64.0/19 ip4:54.240.96.0/19 ip4:76.223.128.0/19 ip4:216.221.160.0/19 -all"

And `ip4:54.240.96.0/19` is what we are looking for, because `54.240.106.159` is contained in `54.240.96.0/19`.
