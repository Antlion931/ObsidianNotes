#programmingChallenges 

[[lsof]] is command used to **L**i**s**t **o**pen **f**iles. However it is noteworthy that everything in Linux is a file. Making it very useful.
## Examples
> [[sudo]] [[lsof]] -i tcp | [[less]]

- `sudo` some files require a special privileges to be showed
- `-i tcp` it says to only prints file for internet networking that uses [[TCP]] protocol
- `| less` there could be a lot of them, so to make it easier to look at, we will pipe a output to a [[less]]

> [[sudo]] [[lsof]] -u avahi | [[less]]

- `-u avahi` it means to show only files opened by user `avahi` which is a part of a [[avahi daemon]]
