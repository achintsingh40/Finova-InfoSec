# Bandit 6

## Code input  
ssh bandit6@bandit.labs.overthewire.org -p2220
bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c
cat /var/lib/dpkg/info/bandit7.password
## Notes
1. first we login  with SSH and pass obtained from previous challange 
2. we find the file using file with the specifications
3. we read the file wo which permission is not denied
## Password 
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj


# Bandit 7

## Code input
ssh bandit7@bandit.labs.overthewire.org -p2220
ls 
cat data.txt
cat data.txt | grep millionth
## Notes 
1. we check if there for the word millionth in the output of data.txt using grep 
## Password 
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc


# Bandit 8

## Code input
ssh bandit8@bandit.labs.overthewire.org -p2220
cat data.txt | sort | uniq -c
## Notes 
1. we first sort the text into the ones which are unique. then we count the no of times each text has been repeated.
## Password 
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM


# Bandit 9

## Code input
ssh bandit9@bandit.labs.overthewire.org -p2220
strings data.txt | grep =
## Notes 
1. we write strings for human readable texts and grep is to find texts starting with =
## Password 
 FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey


 # Bandit 10

## Code input
bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ cat data.txt
VGhlIHBhc3N3b3JkIGlzIGR0UjE3M2ZaS2IwUlJzREZTR3NnMlJXbnBOVmozcVJyCg==
bandit10@bandit:~$ cat data.txt | base64 -d
The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr


## Notes 
1. first we read the data.txt file using cat and we get a text which contains base 64 encoded  text. we can identify this by the == at end of the text 
2.  we use cat data.txt | base64 -d to decode where -d stands for decode the base 64 text 
## Password 
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

