### Common Packages on Ubuntu:
```
apt update
apt install -y sudo net-tools openssh-server vim konsole p7zip-full tree
```

### Anydesk
```
sudo su
wget -qO - https://keys.anydesk.com/repos/DEB-GPG-KEY | apt-key add -
echo "deb http://deb.anydesk.com/ all main" > /etc/apt/sources.list.d/anydesk-stable.list
apt update

apt install -y anydesk
apt install -y libcanberra-gtk-module libcanberra-gtk3-module -y
```
