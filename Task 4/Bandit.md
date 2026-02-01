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
 nmap localhost -p 31000-32000
 ncat --ssl 31790
notepad bandit17.key
icacls bandit17.key /inheritance:r
 icacls bandit17.key /grant:r SONIA:F
ssh -i bandit17.key bandit17@bandit.labs.overthewire.org -p 2220

## Notes 
1. on the windows terminal we login to bandit 16.
2. we check the ports 31000-32000 which are open using  ncat --ssl 31790.(only 2 ports are accessible from which one just echos what we write ) 
3. We get a RSA key from 31790 ports and save it on notepad as bandit17.key
4. then we set the persmissions using : icacls bandit17.key /inheritance:r     & icacls bandit17.key /grant:r SONIA:F
(in the linux setup we would use chmod 600 bandit17.key after saving it in a file)
5. ssh -i bandit17.key bandit17@bandit.labs.overthewire.org -p 2220
6. then we login to badnit 17 with the key we stored. 
  
## Password 
no password we logged in to bandit 17 using a SSH key


# Bandit 17

## Code input
diff passwords.old  passwords.new


## Notes 
1. We just find the difference between both the passwords.    
  
## Password 
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

# Bandit 18

## Code input
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme


## Notes 
1. when we try to enter we get logged out immediately. Thus, wwe run the command to read the readme file over ssh. then we enter the password.  
  
## Password 
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8


# Bandit 19

## Code input
ls -l bandit20-do 
output : -rwsr-x--- 1 bandit20 bandit19 14884 Oct 14 09:26 bandit20-do

./bandit20-do cat /etc/bandit_pass/bandit20
output:0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO


## Notes 
1. setuid binaries allow controlled privilege escalation. (The s in the output of ls -l bandit20-do. s means setuid ) 

  
## Password 
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO


# Bandit 20

## Code input
nc -l -p 4444
./suconnect 4444


## Notes 
1. Start a TCP listener using nc
2. Execute suconnect to connect to that port( in a second terminal after connecting to bandit 20)
3. Send the bandit20 password and we revieve our password

  
## Password 
EeoULMCra2q0dSkYj561DX7s1CpBuOBt


# Bandit 21

## Code input
ls /etc/cron.d
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv



## Notes 
1. In this level, the password for the next level was leaked through a cron job. By listing the cron configuration directory (/etc/cron.d), a scheduled task running as bandit22 was identified.

  
## Password 
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

# Bandit 22

## Code input
ls /etc/cron.d
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh


## Notes 
1. In this level, a cron job running as bandit23 was identified.The cron script generated a filename using an MD5 hash of a predictable string (I am user bandit23)and stored the password in /tmp. By recreating the hash, the password file was located and read to obtain the password for bandit23

  
## Password 
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga