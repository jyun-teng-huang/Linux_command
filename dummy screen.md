# Setup dummy screen
### Install
>X11 Client Installation
```
sudo apt-get install xauth
```
>X11 Server Installation
```
sudo apt-get install xorg
sudo apt-get install openbox
```
### Config
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