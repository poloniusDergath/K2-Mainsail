# K2-Mainsail

Mainsail UI for the K2 Pro

#### This requires root access to be enabled on the printer.

Firmware updates may remove the changes so you may have to run the commands again after a firmware update.

[![https://www.youtube.com/watch?v=V9haiiDYiXg](https://img.youtube.com/vi/V9haiiDYiXg/0.jpg)](https://www.youtube.com/watch?v=V9haiiDYiXg)

https://www.youtube.com/watch?v=V9haiiDYiXg<br>

<hr>

## Install Commands

As the K2 Pro does not have any of the utils needed, we have to copy the files directly via SCP, storing them in the internal memory (that shouldn't get wiped between updates)

```sh
scp -r K2-Mainsail root@192.168.1.100:/mnt/UDISK

```

And then login to the console and run the install command

```sh
chmod +x /mnt/UDISK/K2-Mainsail/*.sh
sh /mnt/UDISK/K2-Mainsail/install.sh
```

<hr>

if you wish to restore the printer to its original configuration then run the commands below

## Restore Commands

```sh
sh /mnt/UDISK/K2-Mainsail/restore.sh

```

<hr>

if you wish to switch between Fluidd or Mainsail and leave the installed files intact

## Switch UI Commands

```sh
sh /mnt/UDISK/K2-Mainsail/switch.sh

```

