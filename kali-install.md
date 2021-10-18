# Installation of KALI Linux

- No Graphical installation
- On Mount Media Error remount usb to /cdrom
- On WiFi Error search firmware and copy to usb/firmware folder

```
# list mounted devices
mount
# mount usb stick to cdrom
mount /dev/sdb1 /cdrom
```

- Enable SSH after Installation

```
# start ssh service
sudo service ssh start

# check if running
sudo service --status-all
```