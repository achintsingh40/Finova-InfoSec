# Linux Luminrium

## Module 6: Practicing Piping


### Challenge 1 : Redirecting Output 

**Commands used**
```bash 
echo PWN > COLLEGE
```

**Output***
```bash 
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your 
flag:
pwn.college{sDM5sOPKukM2fGFPNKfqXqU9GFl.QX0YTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{sDM5sOPKukM2fGFPNKfqXqU9GFl.QX0YTN0wiM0EzNzEzW}


### Challenge 2 : Redirecting more Output 

**Commands used**
```bash 
/challenge/run > myflag
cat myflag
```

**Output***
```bash 
/challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{A6zivMG0jHibEcwr0lJCd9y8Ert.QX1YTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{A6zivMG0jHibEcwr0lJCd9y8Ert.QX1YTN0wiM0EzNzEzW}




### Challenge 3 : Appending Output 

**Commands used**
```bash 
cat /home/hacker/the-flag
/challenge/run >> /home/hacker/the-flag```

**Output***
```bash 
/challenge/run >> /home/hacker/the-flag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /home/hacker/the-flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] Good luck!

[TEST] You should have redirected my stdout to a file called /home/hacker/the-flag. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
I will write the flag in two parts to the file /home/hacker/the-flag! I'll do 
the first write directly to the file, and the second write, I'll do to stdout 
(if it's pointing at the file). If you redirect the output in append mode, the 
second write will append to (rather than overwrite) the first write, and you'll 
get the whole flag!
cat /home/hacker/the-flag
 | 
\|/ This is the first half:
 v 
pwn.college{ktntE6hpexjDyRcv8PIMdrFHMa7.QX3ATO0wiM0EzNzEzW}
                              ^
     that is the second half /|\
                              |

If you only see the second half above, you redirected in *truncate* mode (>) 
rather than *append* mode (>>), and so the write of the second half to stdout 
overwrote the initial write of the first half directly to the file. Try append 
mode!
```

**Flag:**
pwn.college{ktntE6hpexjDyRcv8PIMdrFHMa7.QX3ATO0wiM0EzNzEzW}


### Challenge 4 : Redirecting errors 

**Commands used**
```bash 
/challenge/run > myflag 2> instructions 
cat myflag
```

**Output***
```bash 
[FLAG] Here is your flag:
[FLAG] pwn.college{ofBau5nuW-IJxlYzAYzjJfu8_35.QX3YTN0wiM0EzNzEzW}
flag:
pwn.college{ofBau5nuW-IJxlYzAYzjJfu8_35.QX3YTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{sDM5sOPKukM2fGFPNKfqXqU9GFl.QX0YTN0wiM0EzNzEzW}




### Challenge 5 : Redirecting Input 

**Commands used**
```bash 
echo COLLEGE > PWN
/challenge/run < PWN
```

**Output***
```bash 
echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ cat PWN
COLLEGE
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read 
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{IJjiC7FNzxkA_OEHuPyp_1EHX2T.QXwcTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{IJjiC7FNzxkA_OEHuPyp_1EHX2T.QXwcTN0wiM0EzNzEzW}



### Challenge 6 : Grepping Stored Values     

**Commands used**
```bash 
/challenge/run > /tmp/data.txt
grep "pwn.college" /tmp/data.txt
```

**Output***
```bash 
/challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep "pwn.college" /tmp/data.txt
pwn.college{c7k9U28ItOnwt1VPL1PT0yGACjP.QX4EDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{c7k9U28ItOnwt1VPL1PT0yGACjP.QX4EDO0wiM0EzNzEzW}


### Challenge 7 : Grepping Live output

**Commands used**
```bash 
/challenge/run | grep "pwn.college"
```

**Output***
```bash 
/challenge/run | grep "pwn.college"
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/737jwbhw8ji13x9s88z3wpp8pxaqla92-gnugrep-3.12/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{Qj4dlJvUvSQbBBgunlJ4lkb6dOG.QX5EDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{Qj4dlJvUvSQbBBgunlJ4lkb6dOG.QX5EDO0wiM0EzNzEzW}


### Challenge 8 : Grepping errors

**Commands used**
```bash 
/challenge/run 2>&1 | grep "pwn.college"
```

**Output***
```bash 
/challenge/run 2>&1 | grep "pwn.college"
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/737jwbhw8ji13x9s88z3wpp8pxaqla92-gnugrep-3.12/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{ARPMyzGIu0gVgsh0RpPWt9c5bdD.QX1ATO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{ARPMyzGIu0gVgsh0RpPWt9c5bdD.QX1ATO0wiM0EzNzEzW}



### Challenge 9 : Filtering with grep -v

**Commands used**
```bash 
/challenge/run | grep -v DECOY
```

**Output***
```bash 
/challenge/run | grep -v DECOY
pwn.college{UgE5fzenTA2pMNJj6vPlVDoj0b0.0FOxEzNxwiM0EzNzEzW}
```

**Flag:**
pwn.college{UgE5fzenTA2pMNJj6vPlVDoj0b0.0FOxEzNxwiM0EzNzEzW}


### Challenge 10 : Filtering with sed 

**Commands used**
```bash 
/challenge/run | sed "s/FAKEFLAG//g"
```

**Output***
```bash 
/challenge/run | sed "s/FAKEFLAG//g"
pwn.college{0dIqaJFH1RKZFGaaDOy1aCDyATf.01NxQTMywiM0EzNzEzW}hacker@piping~filtering-with-sed:~$ 
```

**Flag:**
pwn.college{0dIqaJFH1RKZFGaaDOy1aCDyATf.01NxQTMywiM0EzNzEzW}



### Challenge 11 : Duplicating Pipedd data with tee 

**Commands used**
```bash 
/challenge/pwn | tee intercepted | /challenge/college
cat intercepted
/challenge/pwn --secret IYvWB1Cx | /challenge/college
```

**Output***
```bash 
/challenge/pwn | tee intercepted | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code 
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the 
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat intercepted
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "IYvWB1Cx"
hacker@piping~duplicating-piped-data-with-tee:~$ ^C
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret IYvWB1Cx | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{IYvWB1CxYliIAb3VXtS60sQLn0G.QXxITO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{IYvWB1CxYliIAb3VXtS60sQLn0G.QXxITO0wiM0EzNzEzW}


### Challenge 12 : Process substitution for input  

**Commands used**
```bash 
diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
```

**Output***
```bash 
diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
56a57
> pwn.college{cESpL9Dt2PYGqKu2xS1IgRhGWr5.0lNwMDOxwiM0EzNzEzW}
```

**Flag:**
pwn.college{cESpL9Dt2PYGqKu2xS1IgRhGWr5.0lNwMDOxwiM0EzNzEzW}


### Challenge 13 : Writing to multiple programs  

**Commands used**
```bash 
/challenge/hack | tee >(/challenge/the) >(/challenge/planet)
```

**Output***
```bash 
/challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and 
/challenge/planet. Don't try to copy-paste it; it changes too fast.
1993310643615513555
Congratulations, you have duplicated data into the input of two programs! Here 
is your flag:
pwn.college{Eam6igppsoEVvog9xepV-ytvgjd.QXwgDN1wiM0EzNzEzW}
```

**Flag:**
pwn.college{Eam6igppsoEVvog9xepV-ytvgjd.QXwgDN1wiM0EzNzEzW}



### Challenge 14 : Split-piping stderr and stdout  

**Commands used**
```bash 
/challenge/hack \
   > >(/challenge/planet) \
  2> >(/challenge/the)
```

**Output***
```bash 

hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack \
>   > >(/challenge/planet) \
>  2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts 
struggle with! Here is your flag:
pwn.college{cbh8y9Ng1h46Hoizhec22fVj9Je.QXxQDM2wiM0EzNzEzW}
hacker@piping~split-piping-stderr-and-stdout:~$ 
```

**Flag:**
pwn.college{cbh8y9Ng1h46Hoizhec22fVj9Je.QXxQDM2wiM0EzNzEzW}



### Challenge 15 : Named Pipes

**Commands used**
```bash 
*Termianl 1*
mkfifo /tmp/flag_fifo
cat /tmp/flag_fifo
*terminal 2*
/challenge/run > /tmp/flag_fifo

```

**Output***
```bash 
*termianl1*
mkfifo /tmp/flag_fifo 
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{k4jr-5BV1c9FN_5W1kaKAd4_ri-.01MzMDOxwiM0EzNzEzW}

*Terminal 2*
 /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo! 
Bash will now try to open the FIFO for writing, to pass it as the stdout of 
/challenge/run. Recall that operations on FIFOs will *block* until both the 
read side and the write side is open, so /challenge/run will not actually be 
launched until you start reading from the FIFO!

```

**Flag:**
pwn.college{k4jr-5BV1c9FN_5W1kaKAd4_ri-.01MzMDOxwiM0EzNzEzW}
