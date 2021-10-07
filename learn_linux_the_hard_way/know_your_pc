# Linux General Command
## Know your CPU

```
lscpu
```

display:

```
jeremy@jeremy-CQ:~$ lscpu
Architecture:          i686
CPU op-mode(s):        32-bit, 64-bit
Byte Order:            Little Endian
CPU(s):                2
On-line CPU(s) list:   0,1
Thread(s) per core:    1
Core(s) per socket:    2
Socket(s):             1
Vendor ID:             GenuineIntel
CPU family:            6
Model:                 23
Model name:            Pentium(R) Dual-Core CPU       T4200  @ 2.00GHz
Stepping:              10
CPU MHz:               1200.000
CPU max MHz:           2000.0000
CPU min MHz:           1200.0000
BogoMIPS:              3990.60
L1d cache:             32K
L1i cache:             32K
L2 cache:              1024K
...
```

## Memory

```
free -h
```
`h` = human readable

display:(memory usage)

```
              total        used        free      shared  buff/cache   available
Mem:           3.0G        526M        1.8G         39M        610M        2.1G
Swap:          3.0G          0B        3.0G
```

## Disk

```
sudo fdisk -l
```
#information about the disk: (RAM has be ignored below)

```
Disk /dev/sda: 59.6 GiB, 64023257088 bytes, 125045424 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
Disklabel type: dos
Disk identifier: 0x31e523b9

Device     Boot     Start       End   Sectors  Size Id Type
/dev/sda1  *         2048 118759423 118757376 56.6G 83 Linux
/dev/sda2       118761470 125044735   6283266    3G  5 Extended
/dev/sda5       118761472 125044735   6283264    3G 82 Linux swap / Solaris

Disk /dev/sdb: 232.9 GiB, 250059350016 bytes, 488397168 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
Disklabel type: dos
Disk identifier: 0xbf972b39

Device     Boot     Start       End   Sectors  Size Id Type
/dev/sdb1  *           63  83891429  83891367   40G  c W95 FAT32 (LBA)
/dev/sdb2        83891430 272637066 188745637   90G  7 HPFS/NTFS/exFAT
/dev/sdb3       272639115 406472064 133832950 63.8G  c W95 FAT32 (LBA)
/dev/sdb4       406472702 486746111  80273410 38.3G  5 Extended
/dev/sdb5       406472704 486744063  80271360 38.3G  c W95 FAT32 (LBA)
```

## Linux Version

```
jeremy@jeremy-CQ:~$ uname -a # Linux version
Linux jeremy-CQ 4.8.0-36-generic #36~16.04.1-Ubuntu SMP Sun Feb 5 09:39:41 UTC 2017 i686 i686 i686 GNU/Linux
```

## ifconfig: network interface


```
jeremy@jeremy-CQ:~$ ifconfig
enp5s0    Link encap:Ethernet  HWaddr 00:23:5a:40:0f:fa  
          UP BROADCAST MULTICAST  MTU:1500  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:0 (0.0 B)  TX bytes:0 (0.0 B)

lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:65536  Metric:1
          RX packets:23736 errors:0 dropped:0 overruns:0 frame:0
          TX packets:23736 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1 
          RX bytes:1357766 (1.3 MB)  TX bytes:1357766 (1.3 MB)

wlan0     Link encap:Ethernet  HWaddr 00:24:2b:d2:73:6a  
          inet addr:192.168.xx.xxx  Bcast:192.168.xx.xxx  Mask:255.255.255.0
          inet6 addr: fe80::a0c6:54c2:1e36:f592/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:1500  Metric:1
          RX packets:28990 errors:0 dropped:0 overruns:0 frame:0
          TX packets:13838 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:12531888 (12.5 MB)  TX bytes:1722700 (1.7 MB)
```

## Log

2021.10.07
