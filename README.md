# Day-3-Excersise-2
###############################################################
#                          WARNING!!!!                        #
# This is a sandbox environment. Using personal credentials   #
# is HIGHLY! discouraged. Any consequences of doing so are    #
# completely the user's responsibilites.                      #
#                                                             #
# The PWD team.                                               #
###############################################################
[node1] (local) root@192.168.0.13 ~
$ pwd
/root
[node1] (local) root@192.168.0.13 ~
$ cd /home
[node1] (local) root@192.168.0.13 /home
$ mkdir -p home/ nicolette
[node1] (local) root@192.168.0.13 /home
$ ls
dockremap  home       nicolette
[node1] (local) root@192.168.0.13 /home
$ cd /home/nicolette
[node1] (local) root@192.168.0.13 /home/nicolette
$ echo "A few words in the first directory" > first_directory
[node1] (local) root@192.168.0.13 /home/nicolette
$ cat first_directory
A few words in the first directory
[node1] (local) root@192.168.0.13 /home/nicolette
$ cd ~
[node1] (local) root@192.168.0.13 ~
$ sudo adduser nicolette
Changing password for nicolette
New password: 
Bad password: too weak
Retype password: 
passwd: password for nicolette changed by root
[node1] (local) root@192.168.0.13 ~
$ cat /etc/passwd
root:x:0:0:root:/root:/bin/bash
bin:x:1:1:bin:/bin:/sbin/nologin
daemon:x:2:2:daemon:/sbin:/sbin/nologin
adm:x:3:4:adm:/var/adm:/sbin/nologin
lp:x:4:7:lp:/var/spool/lpd:/sbin/nologin
sync:x:5:0:sync:/sbin:/bin/sync
shutdown:x:6:0:shutdown:/sbin:/sbin/shutdown
halt:x:7:0:halt:/sbin:/sbin/halt
mail:x:8:12:mail:/var/mail:/sbin/nologin
news:x:9:13:news:/usr/lib/news:/sbin/nologin
uucp:x:10:14:uucp:/var/spool/uucppublic:/sbin/nologin
operator:x:11:0:operator:/root:/sbin/nologin
man:x:13:15:man:/usr/man:/sbin/nologin
postmaster:x:14:12:postmaster:/var/mail:/sbin/nologin
cron:x:16:16:cron:/var/spool/cron:/sbin/nologin
ftp:x:21:21::/var/lib/ftp:/sbin/nologin
sshd:x:22:22:sshd:/dev/null:/sbin/nologin
at:x:25:25:at:/var/spool/cron/atjobs:/sbin/nologin
squid:x:31:31:Squid:/var/cache/squid:/sbin/nologin
xfs:x:33:33:X Font Server:/etc/X11/fs:/sbin/nologin
games:x:35:35:games:/usr/games:/sbin/nologin
cyrus:x:85:12::/usr/cyrus:/sbin/nologin
vpopmail:x:89:89::/var/vpopmail:/sbin/nologin
ntp:x:123:123:NTP:/var/empty:/sbin/nologin
smmsp:x:209:209:smmsp:/var/spool/mqueue:/sbin/nologin
guest:x:405:100:guest:/dev/null:/sbin/nologin
nobody:x:65534:65534:nobody:/:/sbin/nologin
dockremap:x:100:101:Linux User,,,:/home/dockremap:/sbin/nologin
nicolette:x:1000:1000:Linux User,,,:/home/nicolette:/bin/bash
[node1] (local) root@192.168.0.13 ~
$ chown nicolette /home/nicolette
[node1] (local) root@192.168.0.13 ~
$ ls -ld /home/nicolette
