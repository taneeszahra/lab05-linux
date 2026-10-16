# Security Detective Challenge

## Question 1: Current user and home folder
**Answer:** I am logged in as taneeszahra. My home folder is /home/lab5user.

**Commands:** `whoami`, `pwd`

## Question 2: Server name and Ubuntu version
**Answer:** The server name is ubuntu-lab05. It runs Ubuntu 24.04.3 LTS.

**Commands:** `hostname`, `cat /etc/os-release`

## Question 3: RAM and free disk space
**Answer:** The server has 1.6Gib. The root filesystem has 236.6Mi available.

**Commands:** `free -h`, `df -h /`

## Question 4: Users with the /bin/bash shell
**Answer:** The following accounts have `/bin/bash` as their login shell: taneeszahra.

**Command:** `grep '/bin/bash$' /etc/passwd`

## Question 5: Number of running processes
**Answer:** The `ps aux` output contains  lines 247 lines.

**Command:** `ps aux | wc -l`

## Question 6: lab5user creation and deletion times
**Answer:** The available security logs show Oct 16 07:11:59 and Oct 16 07:13:29. If a timestamp is unavailable, state that the log did not contain it.

**Commands:** `sudo grep lab5user /var/log/auth.log` and `sudo journalctl | grep lab5user` (use the available log source).
