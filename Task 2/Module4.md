# Linux Luminrium

## Module 4: Digesting Documentation


### Challenge 1 :  Learning from Documentation 

**Commands used**
```bash 
/challenge/challenge --giveflag
```

**Output***
```bash 
/challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{UW0BnoCEt4yagHO-Ni2wnHAKOBy.QX0ITO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{UW0BnoCEt4yagHO-Ni2wnHAKOBy.QX0ITO0wiM0EzNzEzW}



### Challenge 2 :  Learning Complex Usage 

**Commands used**
```bash 
find / -name flag
/challenge/challenge --printfile /flag
```

**Output***
```bash 
find / -name flag
find: ‘/root’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
find: ‘/tmp/tmp.2dyEZcT2Od’: Permission denied
/usr/local/lib/python3.8/dist-packages/pwnlib/flag



/home/hacker/flag
find: ‘/var/cache/apt/archives/partial’: Permission denied
find: ‘/var/cache/ldconfig’: Permission denied
find: ‘/var/cache/private’: Permission denied
find: ‘/var/log/private’: Permission denied
find: ‘/var/log/apache2’: Permission denied
find: ‘/var/log/mysql’: Permission denied
find: ‘/var/lib/apt/lists/partial’: Permission denied
find: ‘/var/lib/mysql-keyring’: Permission denied
find: ‘/var/lib/php/sessions’: Permission denied
find: ‘/var/lib/private’: Permission denied
find: ‘/var/lib/mysql-files’: Permission denied
find: ‘/var/lib/mysql’: Permission denied
find: ‘/run/mysqld’: Permission denied
find: ‘/run/sudo’: Permission denied
find: ‘/proc/tty/driver’: Permission denied
find: ‘/proc/1/task/1/fd’: Permission denied
find: ‘/proc/1/task/1/fdinfo’: Permission denied
find: ‘/proc/1/task/1/ns’: Permission denied
find: ‘/proc/1/fd’: Permission denied
find: ‘/proc/1/map_files’: Permission denied
find: ‘/proc/1/fdinfo’: Permission denied
find: ‘/proc/1/ns’: Permission denied
find: ‘/proc/7/task/7/fd’: Permission denied
find: ‘/proc/7/task/7/fdinfo’: Permission denied
find: ‘/proc/7/task/7/ns’: Permission denied
find: ‘/proc/7/fd’: Permission denied
find: ‘/proc/7/map_files’: Permission denied
find: ‘/proc/7/fdinfo’: Permission denied
find: ‘/proc/7/ns’: Permission denied
/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
/flag
/nix/store/7ns27apnvn4qj4q5c82x0z1lzixrz47p-radare2-5.9.8/share/radare2/5.9.8/flag
/nix/store/5z3sjp9r463i3siif58hq5wj5jmy5m98-python3.12-pwntools-4.13.1/lib/python3.12/site-packages/pwnlib/flag
/nix/store/5n5lp1m8gilgrsriv1f2z0jdjk50ypcn-rizin-0.7.3/share/rizin/flag
/nix/store/h88mxp2mbgyj06vypwmqpy05idhwimnp-python3.13-pwntools-4.14.1/lib/python3.13/site-packages/pwnlib/flag
/nix/store/s8b49lb0pqwvw0c6kgjbxdwxcv2bp0x4-radare2-5.9.8/share/radare2/5.9.8/flag
/nix/store/bnlabj2vsbljhp597ir29l51nrqhm89w-rizin-0.7.4/share/rizin/flag
/nix/store/1hyxipvwpdpcxw90l5pq1nvd6s6jdi5m-python3.12-pwntools-4.14.1/lib/python3.12/site-packages/pwnlib/flag
/nix/store/5qz6hgb1qzpvjrsw20wyiylx5zw8b9bk-pwntools-4.14.0/lib/python3.13/site-packages/pwnlib/flag
/challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{oTYjGlj7-cztkm9euz1iAtgqQwW.QX1ITO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{oTYjGlj7-cztkm9euz1iAtgqQwW.QX1ITO0wiM0EzNzEzW}


### Challenge 3 :  Reading Manuals 

**Commands used**
```bash 
man challenge
/challenge/challenge --addhhx 856
```

**Output***
```bash 
man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --addhhx 856
Correct usage! Your flag: pwn.college{8L5Na62dd0TZWWhYhLxsUKFc-qd.QX0EDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{8L5Na62dd0TZWWhYhLxsUKFc-qd.QX0EDO0wiM0EzNzEzW}

### Challenge 4 :   Searching Manuals

**Commands used**
```bash 
man challenge
/challenge/challenge --addhhx 856
```

**Output***
```bash 
man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --addhhx 856
Correct usage! Your flag: pwn.college{8L5Na62dd0TZWWhYhLxsUKFc-qd.QX0EDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{8L5Na62dd0TZWWhYhLxsUKFc-qd.QX0EDO0wiM0EzNzEzW}




### Challenge 5 : Searching for manuals 

**Commands used**
```bash 
man man
```

**Output***
```bash 
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
dqpgxbsgwi (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man dqpgxbsgwi
hacker@man~searching-for-manuals:~$ /challenge/challenge  --dqpgxb 789
Correct usage! Your flag: pwn.college{Yd_qpXgIAQxUJJLR7bFM8sgA9DA.QX2EDO0wiM0EzNzEzW}
hacker@man~searching-for-manuals:~$
```

**Flag:**
pwn.college{Yd_qpXgIAQxUJJLR7bFM8sgA9DA.QX2EDO0wiM0EzNzEzW}



### Challenge 6 :  Helpful Programs 

**Commands used**
```bash 
/challenge/challenge --help
/challenge/challenge -p
```

**Output***
```bash 
/challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 90
hacker@man~helpful-programs:~$ /challenge/challenge -g 90
Correct usage! Your flag: pwn.college{0GAnOm9ZuK0T0uoGsnBUFhlU0QZ.QX3IDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{0GAnOm9ZuK0T0uoGsnBUFhlU0QZ.QX3IDO0wiM0EzNzEzW}


### Challenge 7 : Help for Builtins 

**Commands used**
```bash 
help challenge
challenge --secret M-za_8Nr
```

**Output***
```bash 
help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "M-za_8Nr".
hacker@man~help-for-builtins:~$ challenge --secret M-za_8Nr
Correct! Here is your flag!
pwn.college{M-za_8NrCmmHwuVOlUyxrEZbHIR.QX0ETO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{M-za_8NrCmmHwuVOlUyxrEZbHIR.QX0ETO0wiM0EzNzEzW}


