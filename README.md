# update-motd
A collection of scripts for /etc/update-motd.d

I probably got a wee bit carried away so it may be a bit excessive to get the entire printout each time you SSH in.
*However*, you can simply disable the option to print the motd in your SSH config. You are still left with the generated output in `/var/run/motd.dynamic` which is a convenient way to get a brief overview of your system.

Here is what the output looks like  (refactored for privacy)

```
### Distro information ###
Linux.Distro="Ubuntu 16.04.3 LTS"
Linux.Release=2.6.32-042stab127.2"

### System uptime ###
System.uptime="3 days, 1 hour, 30 minutes"

### UTC date/time ###
System.Time="01/10/18 02:22:47"

### Root Filesystem ####
Filesystem.Device="/dev/simfs"
Filesystem.Size=12G
Filesystem.Used=655M
Filesystem.Avail=12G
Filesystem.Usage=6%

### Memory Usage ###
Memory.Total=128M
Memory.Used=16M
Memory.Free=41M
Memory.Shared=6.9M
Memory.Buffered=69M
Memory.Available=49M

### Host IP addresses ###
IP.Address="192.0.2.154"

### Traffic count on primary interface ###
RX="9.3MB"
TX="12.9MB"

### Established connections ###
192.0.2.154:ssh  203.0.113.198:46440
192.0.2.154:ssh  203.0.113.198:45350

### Latest entries in auth log ###
 pam_unix(sshd:session): session opened for user root by (uid=0)
 pam_unix(cron:session): session opened for user root by (uid=0)
 pam_unix(cron:session): session closed for user root
```
