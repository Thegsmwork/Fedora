### Termux-x11 Fedora
![Screenshot_2024-02-29-18-24-25-397_com termux x11](https://github.com/wahasa/Alpine/assets/69626847/95a01efb-0e17-41c3-972b-9147c7336385)

---
#### Commands in Termux

* Install Package
```
pkg install termux-x11-nightly nano -y
```

* Download App Termux-x11

- [x] [Link Download](https://github.com/termux/termux-x11/releases)

* Edit and remove the sign (#)
```
nano .termux/termux.properties
```

Save : ctrl + x, click Y enter.

Example :

![Screenshot_2024-01-22-07-33-37-878_com termux](https://github.com/wahasa/Kali-Nethunter/assets/69626847/4dc5b01f-ea37-4b86-80c4-e8709734ea73)

---
Add new session :</br>
Swipe the screen from left to right in termux, click 'New Session'.

#### Commands in Fedora
> dnf install nano -y

* Edit script
```
nano /usr/local/bin/termux-x11
```

* Add script
```
#!/bin/sh
export DISPLAY=:1
export PULSE_SERVER=127.0.0.1
rm -rf /run/dbus/dbus.pid
#dbus-launch $HOME/.vnc/xstartup

# --XFCE-- #
startxfce4

# --LXDE-- #
#startlxde

# --LXQT-- #
#startlxqt

# --KDE-- #
#startplasma-x11

# --END-- #
```

Save : ctrl + x, click Y enter.

Note :</br>
Remove the sign (#) on the desktop you are installing now.

* Enable script
```
chmod +x /usr/local/bin/termux-x11
```

---
## Termux-x11
* Start termux-x11

In session 1(termux), run this command
```
termux-x11 :1
```

In session 2 (fedora), run this command
```
termux-x11
```

Open app termux-x11
</br></br>

---
* Stop termux-x11

Close app termux-x11

In session 2 (fedora), run this command
> Click Ctrl+c, enter (2X)

In session 1 (termux), run this command
> Click Ctrl+c, enter
</br>

---
<p align="center">Good Luck</p>

---
