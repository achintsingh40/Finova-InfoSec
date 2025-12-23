# Linux Luminrium

## Module 2: Pondering Paths


### Challenge 1 :The Root

**Commands used**
```bash 
/pwn
```

**Output***
```bash 
BOOM!!!
Here is your flag:
pwn.college{MS4_tQX7nGDPLWlpDI2BMKbFcgH.QX4cTO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{MS4_tQX7nGDPLWlpDI2BMKbFcgH.QX4cTO0wiM0EzNzEzW}


### Challenge 2 :Program and Absolute Paths

**Commands used**
```bash 
/challenge/run
```

**Output***
```bash 
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{4f-r4wPKIQLPelN25KQTShSycK0.QX1QTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{4f-r4wPKIQLPelN25KQTShSycK0.QX1QTN0wiM0EzNzEzW}


### Challenge 3 :Position thy self

**Commands used**
```bash 
cd /usr/bin
/challenge/run
```

**Output***
```bash 
/challenge/run
Incorrect...
You are not currently in the /usr/bin directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ \
> cd /usr/bin
hacker@paths~position-thy-self:/usr/bin$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{kglAaI2w9FhR-q9Xm_VQaWdqC2L.QX2QTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{kglAaI2w9FhR-q9Xm_VQaWdqC2L.QX2QTN0wiM0EzNzEzW}


### Challenge 4 :Position elsewhere

**Commands used**
```bash 
cd /proc/140/fd
cd /usr/bin
cd /tmp
cd /sys
cd /home
/challenge/run
```

**Output***
```bash 
Starting level 1.
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 2
Please use the `cd` utility to change directory to /usr/bin
hacker@paths~position-elsewhere:/proc/140/fd$ cd /usr/bin
hacker@paths~position-elsewhere:/usr/bin$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 3
Please use the `cd` utility to change directory to /tmp
hacker@paths~position-elsewhere:/usr/bin$ cd /tmp
hacker@paths~position-elsewhere:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 4
Please use the `cd` utility to change directory to /sys
hacker@paths~position-elsewhere:/tmp$ cd /sys
hacker@paths~position-elsewhere:/sys$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Moving on to level 5
Please use the `cd` utility to change directory to /home
hacker@paths~position-elsewhere:/sys$ cd /home
hacker@paths~position-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{AJ2OdxWdkDxbBZjEmD8cTFVw_N-.QX3QTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{AJ2OdxWdkDxbBZjEmD8cTFVw_N-.QX3QTN0wiM0EzNzEzW}



### Challenge 5 :implicit relative paths, from /

**Commands used**
```bash 
cd /
challenge/run
```

**Output***
```bash 
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{QzumplRNYAsAZAJVs-tRu8fnAbn.QX5QTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{QzumplRNYAsAZAJVs-tRu8fnAbn.QX5QTN0wiM0EzNzEzW}


### Challenge 6 :explicit relative paths, from /

**Commands used**
```bash 
./challenge/run
```

**Output***
```bash
 hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ challenge/run
Incorrect...
This challenge must be called with a relative path that explicitly starts with a `.`!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4L0pVfogA4SZGYg0Hbt31Y02PIs.QXwUTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{4L0pVfogA4SZGYg0Hbt31Y02PIs.QXwUTN0wiM0EzNzEzW}



### Challenge 7 :Implicit relative path

**Commands used**
```bash 
cd /challenge
```

**Output***
```bash 
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{YCf9PEblGC63H4Av8DKynKWKw5g.QXxUTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{YCf9PEblGC63H4Av8DKynKWKw5g.QXxUTN0wiM0EzNzEzW}


### Challenge 8 : home sweet home


**Commands used**
```bash 
/challenge/run ~/h
```

**Output***
```bash 
/challenge/run ~/h
Writing the file to /home/hacker/h!
... and reading it back to you:
pwn.college{AHYHrQgoLZbdSRmNPaEJPVE3okk.QXzMDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{AHYHrQgoLZbdSRmNPaEJPVE3okk.QXzMDO0wiM0EzNzEzW}