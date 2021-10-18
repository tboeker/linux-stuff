# Creating Custom KALI Image for Raspi 1

https://gitlab.com/kalilinux/build-scripts/kali-arm

https://www.kali.org/docs/general-use/metapackages/

```

# clone and install build tools
cd ~/
git clone https://gitlab.com/kalilinux/build-scripts/kali-arm
cd ~/kali-arm/

sudo ./common.d/build_deps.sh

echo 'disable_ipv6="yes"' > ./builder.txt

# build image
sudo ./rpi1.sh --minimal

```


# Download Prebuild Image

https://www.kali.org/get-kali/#kali-arm

https://www.kali.org/docs/arm/raspberry-pi/

```

# check drives
lsblk

# set vars
export VERSION=2021.3
export SD_CARD=/dev/mmcblk0
export IMAGE_FILE=kali-linux-${VERSION}-rpi-armel.img.xz

# download
wget https://kali.download/arm-images/kali-${VERSION}/${IMAGE_FILE}

# copy to sdcard
xzcat ${IMAGE_FILE} | sudo dd of=${SD_CARD} bs=4M status=progress

```
