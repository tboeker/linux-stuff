Creating Custom KALI Image for Raspi 1

https://gitlab.com/kalilinux/build-scripts/kali-arm
https://www.kali.org/docs/general-use/metapackages/

# clone and install build tools

```
cd ~/
git clone https://gitlab.com/kalilinux/build-scripts/kali-arm
cd ~/kali-arm/
sudo ./common.d/build_deps.sh

# build image
sudo ./rpi1.sh --desktop none --minimal

```