[[Hashcat]] is a command line tool used to break hashed passwords.
## Examples

> hashcat -a 3 -m 0 -w 4 -i simple.hash -1 '?d?l' '?1?1?1?1?1?1?1?1' --potfile-disable

- `-a 3` means which attack type we want to execute. Mode 3 is brute force which will try all passwords of some pattern. There is also hybrid attack that let's you supple some word list and mask (for example 3 digits at the end). Noteworthy is that, some mode let's you specify rules, like try change letter `a` to `@`, making this tool very flexible.
- `-m 0` means which hash function was used. 0 stands for MD5, There are a lot's of them, and every one of them have a lot's of variants, namly:
    - Using the same function twice. 2600 means md5(md5($pass)).
    - Using salt, before, after or both. 3800 means md5(\$salt.\$pass.\$salt)
- `-w 4` changes workload, the 4 is the fastest. However power consumption will skyrocket, and you machine will became unusable for other staff.
- `-i` is connected to attack mode and pattern. It will iteratively take more and more characters from pattern. Firstly trying first letter, then first two, and so on.
- `simple.hash` is a path to file containing a hash to break.
- ``-1 `?d?l`

- [ ] #todo write what have you learned about hashcat while doing exercises for University