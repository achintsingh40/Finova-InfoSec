# Passwords vs SSH Keys

Passwords and SSH keys both are ways to log into systems, but they work very
differently. A password text or a combination of words that you type to login 
or prove who you are. It is easy to use, but it can be guessed or cracked. SSH 
keys are more secure comapared to passwords because they use a pair of keys: a 
public key stored on the server and a private key kept by the user. SSH keys do
not require typing the password/key every time and are much harder to break, 
making them safer for real-world systems.
 

# Data Transformation vs Data Protection

Data transformation means changing how data looks without trying to keep it
secret or hide it. Examples include converting text to uppercase, removing 
characters sorting lines, or formatting output. Anyone can usually reverse or 
understand transformed data. Data protection, on the other hand, focuses on 
keeping data safe from unauthorized access. This includes encryption, 
passwords, file permissions, and authentication methods. Transformation helps
with processing and readability, while protection ensures confidentiality and 
security. Transforming data does not automatically make it secure.


# PATH Injection / PATH Hijacking

PATH hijacking happens when the system is tricked into running the wrong 
command. Linux uses the PATH variable to decide where to look for programs like
ls or cat. If an attacker places a fake command in a directory that appears 
earlier in PATH, the system may run that instead of the real one. This can be 
dangerous, especially in scripts or privileged programs. Using full command 
paths and carefully setting PATH helps prevent this kind of attack.
   