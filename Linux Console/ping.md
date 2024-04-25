#book 

[[ping]] is a program that will send an echo request to some web server using [[ICMP]] protocol. However some servers block [[ping]] so it might not work, even if connection is possible. After getting response [[ping]] will print a bunch of useful information:
- `from` means which server is answering
- `icmp_seq` is a number of request that got to server
- `ttl` means **time to live**, how many hops a packet can take before it dies, it can be set with arguments and used to measure a distance to server
- `time` how much time it took to go to server and come back. Whenever you see a [[ping]] in a game, it is `time` in ms

## Examples

> [[ping]] google.com -c 10 -a -i 10

- `-c 10` means to send only 10 request, by default it works endlessly
- `-a` a [[terminal]] alarm is generated when getting response 
- `-i 10` sets a interval time between next request, in seconds, by default it is set to 1 second