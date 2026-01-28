# Linux Luminrium

## Module 7: Shell Variables


### Challenge 1 : Printing Variables

**Commands used**
```bash 
echo $FLAG
```

**Output***
```bash 
echo $FLAG
pwn.college{4ohELPHFuW1obzkDnYjm3opRGJP.QX3UTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{4ohELPHFuW1obzkDnYjm3opRGJP.QX3UTN0wiM0EzNzEzW}


### Challenge 2 : Setting Variables

**Commands used**
```bash 
PWN=COLLEGE
```

**Output***
```bash 
PWN=COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{0j-Aw23CzBGEVK7mkJRsVeVkVVT.QX5UTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{0j-Aw23CzBGEVK7mkJRsVeVkVVT.QX5UTN0wiM0EzNzEzW}


### Challenge 3 : Multi-Word Variables

**Commands used**
```bash 
PWN="COLLEGE YEAH"
```

**Output***
```bash 
PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{EaxE2MGVY2ycMZUZ_93epK1kwrd.QXwYTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{EaxE2MGVY2ycMZUZ_93epK1kwrd.QXwYTN0wiM0EzNzEzW}


### Challenge 4 : Exporting Variables

**Commands used**
```bash 
COLLEGE=PWN
export PWN=COLLEGE
/challenge/run
```

**Output***
```bash 
COLLEGE=PWN
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great 
job! Here is your flag:
pwn.college{cmNROF2P9ngEKVqUGcsRZyXH2R1.QXyYTN0wiM0EzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

**Flag:**
pwn.college{cmNROF2P9ngEKVqUGcsRZyXH2R1.QXyYTN0wiM0EzNzEzW}



### Challenge 5 : Printing Exported Variables

**Commands used**
```bash 
env
```

**Output***
```bash 
PWN="COLLEGE YEAH"
env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=WzEzNzE0MiwiZW52IiwiY2xpLWF1dGgtdG9rZW4iXQ.aXoK5Q.n6lf4c2cxRDONZ8Jxuf4OJXDj0s
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{svUcO4fZh3bpbTzPxZwh_k4M3zS.QX4UTN0wiM0EzNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

**Flag:**
pwn.college{svUcO4fZh3bpbTzPxZwh_k4M3zS.QX4UTN0wiM0EzNzEzW}


### Challenge 6 : Storing Command Output

**Commands used**
```bash 
PWN=$(/challenge/run)
echo "$PWN"
```

**Output***
```bash 
PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out 
and submit it!
hacker@variables~storing-command-output:~$ echo "$PWN"
pwn.college{A_4VkuLE8NuByUtR08c0YQ2ShYR.QX1cDN1wiM0EzNzEzW}
```

**Flag:**
pwn.college{A_4VkuLE8NuByUtR08c0YQ2ShYR.QX1cDN1wiM0EzNzEzW}


### Challenge 7 : Reading Input

**Commands used**
```bash 
read PWN
COLLEGE
```

**Output***
```bash 
read PWN
COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{AVLJCPDJlhBfTY8kiqbP8DM0TBd.QX4cTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{AVLJCPDJlhBfTY8kiqbP8DM0TBd.QX4cTN0wiM0EzNzEzW}



### Challenge 8 : Reading Files

**Commands used**
```bash 
read PWN < /challenge/read_me
```

**Output***
```bash 
read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{4ELlr5UjI6nXnZSJRn9azN18mCp.QXwIDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{4ELlr5UjI6nXnZSJRn9azN18mCp.QXwIDO0wiM0EzNzEzW}
