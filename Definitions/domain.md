#cybersecurity 

Every server have it's [[IP]] address, however writing and remembering long numbers to our favourite websites can become tedious. That's why people made [[domain]]s, these are human friendly strings that can represent a server. To make it work you firstly need to ask a [[DNS]] server for a [[IP]] address.

![[howdomainswork.png]]

## How domain names are build
[[domain]]s name are build from multiple parts:
1. TLD (Top-Level Domain), examples: `.pl` for polish server, `.gov` for USA government.
2. SLD (Second-Level Domain), the most basic domain, example is `google`, however it could be used to do more hierarchy, like in `gov.pl`, `gov` is SLD and `gov.pl` means polish government servers.
3. More layers, For example `pwr.edu.pl` is server of Wrocław University of Science and Technology in Poland.
4. Subdomain, every domain owner can set some subdomains, to better organise a website. Like `mail.google.com` have a subdomain `mail`.

Subdomains are different from layers, because they do not distinguished between different servers, but all leads to the same server. 

## How to get domain
You need to buy one from some domain registrator, every one can have different prices and policies. Then you can connect your domain to some [[IP]] address.