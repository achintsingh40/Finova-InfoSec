# Bandit 11

## Code input
ssh bandit11@bandit.labs.overthewire.org -p2220
ls -a
cat data.txt
## Notes 
1. After entering, we get a few unreadable words, it seems like the password.
2. on the website it is told that the letters are rotated by 13 letters. thus we go to the rot13 website and enter our text and we get 'The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4'
 
## Password 
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

# Bandit 12

## Code input
ssh bandit12@bandit.labs.overthewire.org -p2220
ls -a
cat data8.bin
gzip -d data8.bin.gz
file data8.bin
tar -xzf data8.bin.tar.gz
bunzip2 data6.bin

## Notes 
1. After entering, we get a datatxt which has text written in hexdump which has been comressed multiple times. we create a new directory, copy the file there, then we unzip the comressed files. theya re compressed in multiple different types of zips like gzip, binzip2 etc.

## Password 
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

# Bandit 13

## Code input
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.privatecat authorized_keys
ls 
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220

## Notes 
1. we enter the bandit 14 using 'ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220',  we enter bandit 14 and look around using ls and cat and get our password.   
  
## Password 
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS



# Bandit 14

## Code input
nc localhost 30000


## Notes 
1. After entering the 14th bandit, we are asked to submit the password of the current level on the port 30000 on localhost.. then we get the passwrod of the next level.   
  
## Password 
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo


# Bandit 15

## Code input
openssl s_client localhost:30001

## Notes 
1. After entering, we write the above command, then enter the password and we get our required password.      
  
## Password 
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx


# Bandit 16

## Code input


## Notes 
1.      
  
## Password 
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx