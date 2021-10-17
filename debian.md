# Tools

```
# midnight commander
apt install mc 


# shutdown
su
systemctl poweroff -i




```


# Change Keyboard Settings

https://wiki.debian.org/Keyboard

```
apt update
apt install keyboard-configuration console-setup

```

# Create Admin User

https://www.codecheef.org/article/create-new-user-and-add-ssh-login-in-linux-server

```

# add user after installation
su
useradd -m -d /home/admin admin
ls -lad
passwd admin

```