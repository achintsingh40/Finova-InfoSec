**Level 0**- 
 First we log into the game using SSH < ssh -p 2220 bandit0@bandit.labs.overthewire.org>

 **Level 0-1**
 we used cat command to read the data password in the readme file
<cat readme>
password= ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If   
then we login using the next username bandit1 using <ssh bandit1@bandit.labs.overthewire.org -p2220>

**Level 1-2**
after logging in using the bandit1 username we have to read a file named -
we use cat < -
writing only <cat -> is interpreted as a command
we get the password 263JGJPfgU6LtdEvgfWU1XP5yac29mFx

**Level 2-3**
after logging into bandit2 we have a file named --spaces in this filename--
to read the spaces we use \ before the spaces and ./ before the name to read the hyphens <-->
We enter <cat ./--spaces\ in\ this\ filename-->
we get the password <MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx>

**Level 3-4**
in this after logging in bandit3 
we change directory to 'inhere' using <cd inhere>
to access hidden files we use <ls -a>
we get a file named '...Hiding-From-You'
we use <  cat ...Hiding-From-You> to read it and get the password 
password- 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

**Level 4-5**
after logging in bandit4
we cahnge the driectory to 'inhere' using <cd inhere>
we display all files using ls  , we get 10 files. To find which of the file is human readable we used <find . -type f | xargs file>
(i.e.  find regular file and give a detailed list of their types)
we get 
./-file04: data
./-file08: data
./-file00: data
./-file07: ASCII text
./-file06: data
./-file01: OpenPGP Public Key
./-file03: data
./-file05: data
./-file09: data

we read ./-file07 with <cat ./-file07> as it is the only file with ASCII text
out password is '  4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw '
[we could also go about trial and error for each file ]


**Level 5-6**
after loggin in bandit5
we got to inhere directory
then using ls we get 19 files 
maybehere00  maybehere04  maybehere08  maybehere12  maybehere16
maybehere01  maybehere05  maybehere09  maybehere13  maybehere17
maybehere02  maybehere06  maybehere10  maybehere14  maybehere18
maybehere03  maybehere07  maybehere11  maybehere15  maybehere19
to find not executable, and size 1033 bytes we use command <find . -type f -size 1033c ! -executable>
we get './maybehere07/.file2' as output
accessing this file we get password  'HWasnPhtq9AVKe0dmk45nxy20cvUa6EG'





