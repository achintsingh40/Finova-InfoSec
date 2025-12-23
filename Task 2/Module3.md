# Linux Luminrium

## Module 3: Comprehending Commands


### Challenge 1 :Cat:not the pet, but the command

**Commands used**
```bash 
cat flag
```

**Output***
```bash 
cat flag
pwn.college{wtGtm17nzi84WMLMUADo1cSKsfA.QXxcTN0wiM0EzNzEzW}
```

**Flag:**
pwn.college{wtGtm17nzi84WMLMUADo1cSKsfA.QXxcTN0wiM0EzNzEzW}


### Challenge 2 :catting absolute paths

**Commands used**

```bash 
cat /flag
```

**Output***
```bash 
cat /flag
pwn.college{wvjrDNDwjCBmx9irLvure5NQLjY.QX5ETO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{wvjrDNDwjCBmx9irLvure5NQLjY.QX5ETO0wiM0EzNzEzW}



### Challenge 3 :more catting practice

**Commands used**
```bash 
 cat /usr/share/base-files/flag
```

**Output***
```bash 
cat /usr/share/base-files/flag
pwn.college{QyXh4mRQiwbE2K8k0nATPgP9Dxy.QXwITO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{QyXh4mRQiwbE2K8k0nATPgP9Dxy.QXwITO0wiM0EzNzEzW}



### Challenge 4 :grepping for a needle in a haystack 

**Commands used**
```bash 
grep pwn.college  /challenge/data.txt
```

**Output***
```bash 
grep pwn.college  /challenge/data.txt
pwn.college{A-66T83Pgi4KQWXsMxFkHFK2hPs.QX3EDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{A-66T83Pgi4KQWXsMxFkHFK2hPs.QX3EDO0wiM0EzNzEzW}


### Challenge 5 :comapring files

**Commands used**
```bash 
diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
```

**Output***
```bash 
diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
12a13
pwn.college{Q6b3X3-5gLFv7J57gbO4tHUt2H_.01MwMDOxwiM0EzNzEzW}
```

**Flag:**
pwn.college{Q6b3X3-5gLFv7J57gbO4tHUt2H_.01MwMDOxwiM0EzNzEzW}


### Challenge 6 :listing files

**Commands used**
```bash 
ls /challenge
cat foo.1x.dvi
```

**Output***
```bash 
hacker@commands~listing-files:~$ ls /challenge
18088-renamed-run-23014  DESCRIPTION.md
hacker@commands~listing-files:~$ cd /challenge
hacker@commands~listing-files:/challenge$ cat 18088-renamed-run-23014
#!/opt/pwn.college/bash

echo "Yahaha, you found me! Here is your flag:"
cat /flag
```

**Flag:**
#!/opt/pwn.college/bash


### Challenge 7 :touching files

**Commands used**
```bash 
touch /tmp/pwn
touch /tmp/college
/challenge/run
```

**Output***
```bash 
touch /tmp/pwn
hacker@commands~touching-files:~$ touch /tmp/college
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{oKSr4JXDgPx6_ucvExFZfBE35E3.QXwMDO0wiM0EzNzEzW}

```

**Flag:**
pwn.college{oKSr4JXDgPx6_ucvExFZfBE35E3.QXwMDO0wiM0EzNzEzW}


### Challenge 8 :listing files

**Commands used**
```bash 
rm delete_me
/challenge/check
```

**Output***
```bash 
rm delete_me
hacker@commands~removing-files:~$ /challenge/check 
Excellent removal. Here is your reward:
pwn.college{MrnnPGUMElprFtHo5YZbTtVMZlu.QX2kDM1wiM0EzNzEzW}
```

**Flag:**
pwn.college{MrnnPGUMElprFtHo5YZbTtVMZlu.QX2kDM1wiM0EzNzEzW}



### Challenge 9 :moving files

**Commands used**
```bash 
mv /flag /tmp/hack-the-planet
/challenge/check 
```

**Output***
```bash 
mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check 
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{UsGdWlr_vIyPltedMnv-mCtrU-g.0VOxEzNxwiM0EzNzEzW}
```

**Flag:**
pwn.college{UsGdWlr_vIyPltedMnv-mCtrU-g.0VOxEzNxwiM0EzNzEzW}



### Challenge 10 :copying files

**Commands used**
```bash 
cp /flag /tmp/hack-the-planet 
/challenge/check 
```

**Output***
```bash 
cp /flag /tmp/hack-the-planet 
Correct! Performing 'cp /flag /tmp/hack-the-planet'.
hacker@commands~copying-files:~$ /challenge/check
Congrats! You successfully copied the flag to /tmp/hack-the-planet! Here it is:
pwn.college{IbrBFVoggvhxuLCRnwaNZ3oC1xZ.0lNxQTMywiM0EzNzEzW}
```

**Flag:**
pwn.college{IbrBFVoggvhxuLCRnwaNZ3oC1xZ.0lNxQTMywiM0EzNzEzW}



### Challenge 11 :copying files

**Commands used**
```bash 
ls -a 
cat /.flag-32664313332429 
```

**Output***
```bash 
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-32664313332429  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat /.flag-32664313332429
pwn.college{QwrC4SfFfemOhnKG_y9-1DPG7Ay.QXwUDO0wiM0EzNzEzW}
hacker@commands~hidden-files:/$ 

```

**Flag:**
pwn.college{QwrC4SfFfemOhnKG_y9-1DPG7Ay.QXwUDO0wiM0EzNzEzW}



### Challenge 12 :An Epic Filesystem Quest

**Commands used**
```bash 
cd 
ls -a
cat 
```

**Output***
```bash 
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
..  SNIPPET     boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~an-epic-filesystem-quest:/$ cat SNIPPET
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/babel/messages

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/babel/messages
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/messages$ ls
REVELATION  __init__.py  __pycache__  catalog.py  checkers.py  extract.py  frontend.py  jslexer.py  mofile.py  plurals.py  pofile.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/messages$ ls -a
.  ..  REVELATION  __init__.py  __pycache__  catalog.py  checkers.py  extract.py  frontend.py  jslexer.py  mofile.py  plurals.py  pofile.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/messages$ cat REVELATION
Congratulations, you found the clue!
The next clue is in: /usr/lib/debug/.build-id/4c
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/messages$ cd /usr/lib/debug/.build-id/4c
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ ls -a
.  ..  30eb1af9dbeb05c90d39f02d3ef22378bb7e83.debug  LEAD  a519c57907148c97eb2b806009e51816968568.debug  cfec65a5d176c6ab5c45aba648bc1e6adb897d.debug
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ cat LEAD
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/include/config/preempt

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ ls /opt/linux/linux-5.4/include/config/preempt
INFO-TRAPPED  voluntary.h
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ ls /opt/linux/linux-5.4/include/config/preempt cat INFO-Trapped
/opt/linux/linux-5.4/include/config/preempt:
INFO-TRAPPED  voluntary.h
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ cat /opt/linux/linux-5.4/include/config/preempt/INFO-TRAPPED
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Main/Regular

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ ls -a
.  ..  30eb1af9dbeb05c90d39f02d3ef22378bb7e83.debug  LEAD  a519c57907148c97eb2b806009e51816968568.debug  cfec65a5d176c6ab5c45aba648bc1e6adb897d.debug
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/4c$ cd /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Main/Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Main/Regular$ ls -a
.  ..  .CUE  Main.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Main/Regular$ cat .CUE
Great sleuthing!
The next clue is in: /usr/share/sphinx/locale
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/Main/Regular$ cd /usr/share/sphinx/locale
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale$ ls
TIP  bn  cs  da  el  es  eu  fi  he  hi_IN  hu  it  ko  lv  nb_NO  nl  pt     pt_PT  ru  sk  sr        sv  tr     vi     zh_TW
ar   ca  cy  de  eo  et  fa  fr  hi  hr     id  ja  lt  mk  ne     pl  pt_BR  ro     si  sl  sr@latin  ta  uk_UA  zh_CN
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale$ ls -a
.   TIP  bn  cs  da  el  es  eu  fi  he  hi_IN  hu  it  ko  lv  nb_NO  nl  pt     pt_PT  ru  sk  sr        sv  tr     vi     zh_TW
..  ar   ca  cy  de  eo  et  fa  fr  hi  hr     id  ja  lt  mk  ne     pl  pt_BR  ro     si  sl  sr@latin  ta  uk_UA  zh_CN
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale$ cat TIP
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/include/uapi/linux/hsi
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale$ cd /opt/linux/linux-5.4/include/uapi/linux/hsi
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/uapi/linux/hsi$ ls -a
.  ..  DOSSIER  cs-protocol.h  hsi_char.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/uapi/linux/hsi$ cat DOSSIER
Lucky listing!
The next clue is in: /opt/busybox/busybox-1.33.2/util-linux

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/uapi/linux/hsi$ cd /opt/busybox/busybox-1.33.2/util-linux
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/util-linux$ ls -a
.                   .hexdump.o.cmd      .rdev.o.cmd          acpid.o       fdformat.o     hexdump.o      mesg.c             pivot_root.c    setsid.o
..                  .hexdump_xxd.o.cmd  .readprofile.o.cmd   blkdiscard.c  fdisk.c        hexdump_xxd.c  mesg.o             pivot_root.o    swaponoff.c
.acpid.o.cmd        .hwclock.o.cmd      .renice.o.cmd        blkdiscard.o  fdisk.o        hexdump_xxd.o  minix.h            rdate.c         swaponoff.o
.blkdiscard.o.cmd   .ionice.o.cmd       .rev.o.cmd           blkid.c       fdisk_aix.c    hwclock.c      mkfs_ext2.c        rdate.o         switch_root.c
.blkid.o.cmd        .ipcrm.o.cmd        .rtcwake.o.cmd       blkid.o       fdisk_gpt.c    hwclock.o      mkfs_ext2.o        rdev.c          switch_root.o
.blockdev.o.cmd     .ipcs.o.cmd         .script.o.cmd        blockdev.c    fdisk_osf.c    ionice.c       mkfs_ext2.txt      rdev.o          taskset.c
.built-in.o.cmd     .last_fancy.o.cmd   .scriptreplay.o.cmd  blockdev.o    fdisk_sgi.c    ionice.o       mkfs_ext2_test.sh  readprofile.c   taskset.o
.cal.o.cmd          .lib.a.cmd          .setarch.o.cmd       built-in.o    fdisk_sun.c    ipcrm.c        mkfs_minix.c       readprofile.o   uevent.c
.chrt.o.cmd         .losetup.o.cmd      .setpriv.o.cmd       cal.c         findfs.c       ipcrm.o        mkfs_minix.o       renice.c        uevent.o
.dmesg.o.cmd        .lspci.o.cmd        .setsid.o.cmd        cal.o         findfs.o       ipcs.c         mkfs_reiser.c      renice.o        umount.c
.eject.o.cmd        .lsusb.o.cmd        .swaponoff.o.cmd     chrt.c        flock.c        ipcs.o         mkfs_vfat.c        rev.c           umount.o
.fallocate.o.cmd    .mdev.o.cmd         .switch_root.o.cmd   chrt.o        flock.o        last.c         mkfs_vfat.o        rev.o           unshare.c
.fatattr.o.cmd      .mesg.o.cmd         .taskset.o.cmd       dmesg.c       freeramdisk.c  last_fancy.c   mkswap.c           rtcwake.c       unshare.o
.fbset.o.cmd        .mkfs_ext2.o.cmd    .uevent.o.cmd        dmesg.o       freeramdisk.o  last_fancy.o   mkswap.o           rtcwake.o       volume_id
.fdformat.o.cmd     .mkfs_minix.o.cmd   .umount.o.cmd        eject.c       fsck_minix.c   lib.a          more.c             script.c        wall.c
.fdisk.o.cmd        .mkfs_vfat.o.cmd    .unshare.o.cmd       eject.o       fsck_minix.o   losetup.c      more.o             script.o        wall.o
.findfs.o.cmd       .mkswap.o.cmd       .wall.o.cmd          fallocate.c   fsfreeze.c     losetup.o      mount.c            scriptreplay.c
.flock.o.cmd        .more.o.cmd         Config.in            fallocate.o   fsfreeze.o     lspci.c        mount.o            scriptreplay.o
.freeramdisk.o.cmd  .mount.o.cmd        Config.src           fatattr.c     fstrim.c       lspci.o        mountpoint.c       setarch.c
.fsck_minix.o.cmd   .mountpoint.o.cmd   EVIDENCE             fatattr.o     fstrim.o       lsusb.c        mountpoint.o       setarch.o
.fsfreeze.o.cmd     .nsenter.o.cmd      Kbuild               fbset.c       getopt.c       lsusb.o        nologin.c          setpriv.c
.fstrim.o.cmd       .pivot_root.o.cmd   Kbuild.src           fbset.o       getopt.o       mdev.c         nsenter.c          setpriv.o
.getopt.o.cmd       .rdate.o.cmd        acpid.c              fdformat.c    hexdump.c      mdev.o         nsenter.o          setsid.c
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/util-linux$ cat EVIDENCE
Great sleuthing!
The next clue is in: /usr/lib/python3/dist-packages/sphinx/pycode/__pycache__

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/util-linux$ ls /usr/lib/python3/dist-packages/sphinx/pycode/__pycache__
NUGGET-TRAPPED  __init__.cpython-38.pyc  parser.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/util-linux$ cat /usr/lib/python3/dist-packages/sphinx/pycode/__pycache__/NUGGET-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{kg1yQCgxBnATofS8-SPOsGKQQQm.QX5IDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{kg1yQCgxBnATofS8-SPOsGKQQQm.QX5IDO0wiM0EzNzEzW}


### Challenge 13 :making directories

**Commands used**
```bash 
mkdir
```

**Output***
```bash 
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{gkDLtnlYu4Ou-LtPzxFRO0rbc1C.QXxMDO0wiM0EzNzEzW}
```

**Flag:**
pwn.college{gkDLtnlYu4Ou-LtPzxFRO0rbc1C.QXxMDO0wiM0EzNzEzW}


### Challenge 14: Finding Files

**Commands used**
```bash 
find / -name  flag
```

**Output***
```bash 
hacker@commands~finding-files:~$ find / -name flag
find: ‘/root’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
find: ‘/tmp/tmp.2dyEZcT2Od’: Permission denied
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
/usr/lib/python3/dist-packages/Cython/Build/Tests/__pycache__/flag
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
/nix/store/7ns27apnvn4qj4q5c82x0z1lzixrz47p-radare2-5.9.8/share/radare2/5.9.8/flag
/nix/store/5z3sjp9r463i3siif58hq5wj5jmy5m98-python3.12-pwntools-4.13.1/lib/python3.12/site-packages/pwnlib/flag
/nix/store/5n5lp1m8gilgrsriv1f2z0jdjk50ypcn-rizin-0.7.3/share/rizin/flag
/nix/store/h88mxp2mbgyj06vypwmqpy05idhwimnp-python3.13-pwntools-4.14.1/lib/python3.13/site-packages/pwnlib/flag
/nix/store/s8b49lb0pqwvw0c6kgjbxdwxcv2bp0x4-radare2-5.9.8/share/radare2/5.9.8/flag
/nix/store/bnlabj2vsbljhp597ir29l51nrqhm89w-rizin-0.7.4/share/rizin/flag
/nix/store/1hyxipvwpdpcxw90l5pq1nvd6s6jdi5m-python3.12-pwntools-4.14.1/lib/python3.12/site-packages/pwnlib/flag
/nix/store/5qz6hgb1qzpvjrsw20wyiylx5zw8b9bk-pwntools-4.14.0/lib/python3.13/site-packages/pwnlib/flag
hacker@commands~finding-files:~$ cat /usr/local/lib/python3.8/dist-packages/pwnlib/flag
cat: /usr/local/lib/python3.8/dist-packages/pwnlib/flag: Is a directory
hacker@commands~finding-files:~$ cat /usr/lib/python3/dist-packages/Cython/Build/Tests/__pycache__/flag
pwn.college{UkNsuYu2_1G2XViIBnaGuI5eFt9.QXyMDO0wiM0EzNzEzW}hacker@commands~finding-files:~$ 
```
pwn.college{QuAaO1-fTV_tKjRVcSEXqsCa8e_.QX5ETN1wiM0EzNzEzW}
**Flag:**
pwn.college{UkNsuYu2_1G2XViIBnaGuI5eFt9.QXyMDO0wiM0EzNzEzW}


### Challenge 15 :Linking Files
**Commands used**
```bash 
ln -s
```

**Output***
```bash 
hacker@commands~linking-files:~$ cd /home/hacker
hacker@commands~linking-files:~$ cd /home/hacker/
hacker@commands~linking-files:~$ pwd
/home/hacker
hacker@commands~linking-files:~$ ls
Desktop  college  flag  foo.1x.dvi  h  not-the-flag
hacker@commands~linking-files:~$ ls -l
total 12
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
lrwxrwxrwx 1 hacker hacker  5 Dec 23 13:18 not-the-flag -> /flag
hacker@commands~linking-files:~$ rm not-the-flag 
hacker@commands~linking-files:~$ ls -l
total 8
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
hacker@commands~linking-files:~$ touch not-the-flag 
hacker@commands~linking-files:~$ vim not-the-flag 
hacker@commands~linking-files:~$ cat not-the-flag 
hacker@commands~linking-files:~$ cat "Thia is the file content in not the flag file ?" >> not-the-flag 
cat: 'Thia is the file content in not the flag file ?': No such file or directory
hacker@commands~linking-files:~$ cat "Thia is the file content in not the flag file " >> not-the-flag 
cat: 'Thia is the file content in not the flag file ': No such file or directory
hacker@commands~linking-files:~$ cat "Thia is the file content in not the flag file " > not-the-flag 
cat: 'Thia is the file content in not the flag file ': No such file or directory
hacker@commands~linking-files:~$ cat not-the-flag << "Thia is the file content in not the flag file "
> q
> 
> 
> ^C
hacker@commands~linking-files:~$ cat not-the-flag 
hacker@commands~linking-files:~$ vi not-the-flag 
hacker@commands~linking-files:~$ cat not-the-flag 
This is the content in not the flag file 
hacker@commands~linking-files:~$ vi not-the-flag 
hacker@commands~linking-files:~$ vim not-the-flag 
hacker@commands~linking-files:~$ rm not-the-flag 
hacker@commands~linking-files:~$ ls -l
total 8
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
hacker@commands~linking-files:~$ ln -s /flag not-the-flag
hacker@commands~linking-files:~$ ls -l
total 12
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
lrwxrwxrwx 1 hacker hacker  5 Dec 23 17:17 not-the-flag -> /flag
hacker@commands~linking-files:~$ rm not-the-flag 
hacker@commands~linking-files:~$ vi not-the-fkag
hacker@commands~linking-files:~$ ls -l
total 12
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
-rw-r--r-- 1 hacker hacker 45 Dec 23 17:19 not-the-fkag
hacker@commands~linking-files:~$ cd /challenge
hacker@commands~linking-files:/challenge$ ls
DESCRIPTION.md  catflag
hacker@commands~linking-files:/challenge$ ./catflag 
About to read out the /home/hacker/not-the-flag file!
cat: /home/hacker/not-the-flag: No such file or directory
hacker@commands~linking-files:/challenge$ ls /home/hacker/not-the-fkag 
/home/hacker/not-the-fkag
hacker@commands~linking-files:/challenge$ cd /home/hacker/
hacker@commands~linking-files:~$ mv not-the-fkag not-the-flag 
hacker@commands~linking-files:~$ cd /challenge/
hacker@commands~linking-files:/challenge$ ./catflag
About to read out the /home/hacker/not-the-flag file!
This is not the flag file created by achint`
hacker@commands~linking-files:/challenge$ cd /home/hacker/
hacker@commands~linking-files:~$ mv not-the-flag not-the-flag-bkp 
hacker@commands~linking-files:~$ ls-l
bash: ls-l: command not found
hacker@commands~linking-files:~$ ls -l
total 12
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
-rw-r--r-- 1 hacker hacker 45 Dec 23 17:19 not-the-flag-bkp
hacker@commands~linking-files:~$ ln -s /flag not-the-flag
hacker@commands~linking-files:~$ ls -l
total 16
drwxr-xr-x 1 hacker hacker  0 Sep 22 17:41 Desktop
-rw-r--r-- 1 hacker hacker  0 Sep 27 18:45 college
-rw-r--r-- 1 hacker hacker 17 Dec 23 13:11 flag
-rw-r--r-- 1 hacker hacker  0 Sep 29 14:40 foo.1x.dvi
-rw-r--r-- 1 root   hacker 60 Dec 23 06:41 h
lrwxrwxrwx 1 hacker hacker  5 Dec 23 17:24 not-the-flag -> /flag
-rw-r--r-- 1 hacker hacker 45 Dec 23 17:19 not-the-flag-bkp
hacker@commands~linking-files:~$ /challenge/catflag 
About to read out the /home/hacker/not-the-flag file!
pwn.college{QuAaO1-fTV_tKjRVcSEXqsCa8e_.QX5ETN1wiM0EzNzEzW}
hacker@commands~linking-files:~$ 
```

**Flag:**
pwn.college{QuAaO1-fTV_tKjRVcSEXqsCa8e_.QX5ETN1wiM0EzNzEzW}




