# An Epic Filesystem Quest
This was a challenge which required to use all the commands ls, cd, and cat to get to the key. It involved changing into multiple directories and using ls to list and using
cat to read the next clue. I finally found the key in the REVELATION file.
## Command Line
```
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
TRACE  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin    challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat TRACE
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/net/wimax/i2400m

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.4/drivers/net/wimax/i2400m
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/net/wimax/i2400m$ ls -a
.     Kconfig    debug-levels.h  fw.c          netdev.c     sysfs.c             usb-fw.c     usb-tx.c
..    Makefile   debugfs.c       i2400m-usb.h  op-rfkill.c  tx.c                usb-notif.c  usb.c
.TIP  control.c  driver.c        i2400m.h      rx.c         usb-debug-levels.h  usb-rx.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/net/wimax/i2400m$ cat .TIP
Great sleuthing!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/sh/is

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/net/wimax/i2400m$ ls /opt/busybox/busybox-1.33.2/include/config/sh/is
NOTE-TRAPPED  ash.h  hush.h  none.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/net/wimax/i2400m$ cat /opt/busybox/busybox-1.33.2/include/config/sh/is/NOTE-TRAPPED
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/xtensa/include
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/net/wimax/i2400m$ /opt/busybox/busybox-1.33.2/include/config/sh/is^C
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/net/wimax/i2400m$ cd /opt/linux/linux-5.4/arch/xtensa/include
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/xtensa/include$ ls
README  asm  uapi
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/xtensa/include$ cat README
Tubular find!
The next clue is in: /usr/share/racket/pkgs/web-server-lib/web-server/managers

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/xtensa/include$ cd /usr/share/racket/pkgs/web-server-lib/web-server/managers
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/web-server-lib/web-server/managers$ ls
BRIEF  compiled  lru.rkt  manager.rkt  none.rkt  timeouts.rkt
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/web-server-lib/web-server/managers$ cat BRIEF
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/include/config/acpi/system
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/web-server-lib/web-server/managers$ cd /opt/linux/linux-5.4/include/config/acpi/system
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/acpi/system$ ls
WHISPER  power
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/acpi/system$ cat WHISPER
Yahaha, you found me!
The next clue is in: /usr/share/racket/pkgs/distributed-places-lib/racket/place

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/acpi/system$ cd /usr/share/racket/pkgs/distributed-places-lib/racket/place
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/distributed-places-lib/racket/place$ ls
POINTER  compiled  define-remote-server.rkt  distributed  distributed.rkt
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/distributed-places-lib/racket/place$ cat POINTER
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/gpu/drm/amd/display/dc/irq/dcn21
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/distributed-places-lib/racket/place$ cd /opt/linux/linux-5.4/drivers/gpu/drm/amd/display/dc/irq/dcn21
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/amd/display/dc/irq/dcn21$ ls
EVIDENCE  irq_service_dcn21.c  irq_service_dcn21.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/amd/display/dc/irq/dcn21$ cat EVIDENCE
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/arm/mach-nomadik
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/amd/display/dc/irq/dcn21$ cd /opt/linux/linux-5.4/arch/arm/mach-nomadik
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-nomadik$ ls
Kconfig  Makefile  REVELATION  cpu-8815.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-nomadik$ cat REVELATION
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{Iaa2vCo8B-FG6CEbHyilQgps4aE.dljM4QDLxcDN0czW}
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm/mach-nomadik$
```
<img width="818" alt="An Epic Filesystem Quest" src="https://github.com/user-attachments/assets/c29ebdd1-c7cc-42cf-bdd6-4c32c3077f75">
