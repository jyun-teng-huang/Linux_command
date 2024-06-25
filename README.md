# Linux Common Command Line
### Common Packages on Ubuntu:
```
sudo apt update
sudo apt install -y sudo net-tools openssh-server vim konsole p7zip-full tree
sudo apt install -y chrome-gnome-shell

```
### Install Anydesk
```
sudo su
wget -qO - https://keys.anydesk.com/repos/DEB-GPG-KEY | apt-key add -
echo "deb http://deb.anydesk.com/ all main" > /etc/apt/sources.list.d/anydesk-stable.list
apt update
apt install -y anydesk
apt install -y libcanberra-gtk-module libcanberra-gtk3-module -y
```
### Vitis dependencies packages:
```
sudo apt-get install gcc-multilib g++-multilib -y
sudo apt-get install ocl-icd-libopencl1 -y
sudo apt-get install ocl-icd-opencl-dev -y
sudo apt-get install opencl-headers -y
sudo apt install libstdc++6 -y
sudo apt install libncurses5 -y
```
### Petalinux dependencies packages:
```
sudo apt install gawk
sudo apt install xterm -y
sudo apt install autoconf -y
sudo apt install libtool -y
sudo apt install texinfo -y
sudo apt install libncurses5-dev libncursesw5-dev -y.
sudo apt install zlib1g:i386 -y
```
### Install Git
```
sudo apt install git git-lfs -y
```
> Git common push flow
```
git init
git lfs track AAA
git add AAA
git add BBB
git commit -m "update"
git branch -m main
git remote add origin repo@url
git push origin main
```
### Install vscode:
```
sudo apt update
sudo apt install software-properties-common apt-transport-https wget -y
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code
```
> Change the preset editor at ubuntu:
```
sudo update-alternatives --config editor
editor
```
> **Src site:**
>1. https://phoenixnap.com/kb/install-vscode-ubuntu
>2. https://samwhelp.github.io/book-ubuntu-basic-skill/book/content/editor/select-editor.html
### X11 Install
>X11 Client Installation
```
sudo apt-get install xauth
```
>X11 Server Installation
```
sudo apt-get install xorg
sudo apt-get install openbox
```
> **Config**
>Check particular Modeline
```
cvt 1920 1080 60
```
>Config X11
```
vim /etc/X11/xorg.conf.d/dummy_screen.conf
```
>Section "Monitor"  
>        Identifier "dummy_monitor"  
>        HorizSync 28.0-80.0  
>        VertRefresh 48.0-75.0  
>        Modeline "1920x1080" 172.80 1920 2040 2248 2576 1080 1081 1084 1118  
>EndSection  
>  
>Section "Device"  
>        Identifier "dummy_card"  
>        VideoRam 256000  
>        Driver "dummy"  
>EndSection  
>  
>Section "Screen"  
>        Identifier "dummy_screen"  
>        Device "dummy_card"  
>        Monitor "dummy_monitor"  
>        SubSection "Display"  
>        EndSubSection  
>EndSection  
