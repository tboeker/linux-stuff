# Download Image

https://wiki.debian.org/RaspberryPiImages

```
# check drives
lsblk

sudo bash
export RPI_MODEL=1
export SD_CARD=/dev/mmcblk0
export DEBIAN_RELEASE=buster

wget https://raspi.debian.net/daily/raspi_${RPI_MODEL}_${DEBIAN_RELEASE}.img.xz

xzcat raspi_${RPI_MODEL}_${DEBIAN_RELEASE}.img.xz | dd of=${SD_CARD} bs=64k oflag=dsync status=progress
```