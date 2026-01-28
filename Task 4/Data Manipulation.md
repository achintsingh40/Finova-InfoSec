# Linux Luminrium

## Module 8: Data Manipulation


### Challenge 1 : Translating Characters 

**Commands used**
```bash 
/challenge/run | tr 'a-zA-Z' 'A-Za-z'
```

**Output***
```bash 
/challenge/run | tr 'a-zA-Z' 'A-Za-z'
yOUR CASE-SWAPPED FLAG:
pwn.college{4qIV1gv1fB4zB9Kim0igC0Z9kOZ.01MxEzNxwiM0EzNzEzW}
```

**Flag:**
pwn.college{4qIV1gv1fB4zB9Kim0igC0Z9kOZ.01MxEzNxwiM0EzNzEzW}


### Challenge 2 : Deleting Characters

**Commands used**
```bash 
/challenge/run | tr -d '^%'
```

**Output***
```bash 
/challenge/run | tr -d '^%'
Your character-stuffed flag:
pwn.college{QweRfQfYavQPgT80fGOvtBrOcQz.0FNxEzNxwiM0EzNzEzW}
```

**Flag:**
pwn.college{QweRfQfYavQPgT80fGOvtBrOcQz.0FNxEzNxwiM0EzNzEzW}


### Challenge 3 : Deleting new lines

**Commands used**
```bash 
/challenge/run | tr -d '\n'```

**Output***
```bash 
/challenge/run | tr -d '\n'
Your line-split flag: pwn.college{cVG9HlTN_83ZuVJYmRjOUqwJ2JP.0VNxEzNxwiM0EzNzEzW}hacker@data~deleting-newlines:~$ 
```

**Flag:**
pwn.college{cVG9HlTN_83ZuVJYmRjOUqwJ2JP.0VNxEzNxwiM0EzNzEzW}

### Challenge 4 : Extracting the first lines with head  

**Commands used**
```bash 
/challenge/pwn | head -n 7 | /challenge/college
```

**Output***
```bash 
/challenge/pwn | head -n 7 | /challenge/college
\
Congratulations, you piped the right codes!
pwn.college{kA6UPnXHMxWZWyiodhbarNkPLX1.0lNxEzNxwiM0EzNzEzW}
```

**Flag:**
pwn.college{kA6UPnXHMxWZWyiodhbarNkPLX1.0lNxEzNxwiM0EzNzEzW}


### Challenge 5 : Extracting specific sections of text 

**Commands used**
```bash 
/challenge/run | cut -d " " -f 2 | tr -d "\n"```

**Output***
```bash 
/challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{wGWzsPoMJzW1N2Axj9glRH1iT1N.01NxEzNxwiM0EzNzEzW}hacker@data~extracting-specific-sections-of-text:~$ 
```

**Flag:**
pwn.college{wGWzsPoMJzW1N2Axj9glRH1iT1N.01NxEzNxwiM0EzNzEzW}

### Challenge 6 : Sorting Data


**Commands used**
```bash 
sort /challenge/flags.txt | tail -n 1
```

**Output***
```bash 
sort /challenge/flags.txt | tail -n 1
pwn.college{Im7h6IBCm_bGXk10U_Dz3jJxOW2.0FM0MDOxwiM0EzNzEzW}
```

**Flag:**
pwn.college{Im7h6IBCm_bGXk10U_Dz3jJxOW2.0FM0MDOxwiM0EzNzEzW}

