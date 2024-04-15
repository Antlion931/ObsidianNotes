#programmingChallenges 

Multiple application can work on the same device. And as an result, can use internet, and receive data. But how to know which packet of data, is addressed to which application.

Here comes [[Port]] numbers, they range from 0-65535, but first 1024 are saved for important stuff. So whenever application wants to start using internet it's create some called [[Socket]], and chooses random number from 1024-65535. 

![[how_ports_work.jpg]]

## Where I can find them?
Port numbers are in headers of transport layer, so in [[TCP]] and [[UDP]]. You can also use [[lsof]] command to list them on your device. You could also google some well know port numbers.

![[common_port_nummbers.png]]

- [ ] #todo write note on how to use [[lsof]]