# Glenn INFO

## [Caffeine](https://www.zhornsoftware.co.uk/caffeine/index.html#home)
> [Prevent your computer from going to sleep, click HERE to download the program](https://www.zhornsoftware.co.uk/caffeine/caffeine.zip)


### _To keep your Microsoft Teams status active._


#### Method 1: Manually Change Your Status to Available
```
Open your Microsoft Teams app or use the web version.
Log into your account by entering your username and password.
Click on your Profile icon.
Click on your current status below your name and choose ‘Available’ from the list.
```

#### Method 2: Use Status Message
```
Open the Microsoft Teams app or use the web version.
Log into your Teams account by using your username and password.
Now, click on your Profile icon from the top-right corner of the screen.
Click on ‘Set status message.’
Now, type your status in the message box, and tick the checkbox next to ‘show when people message me’ to show your status message to people messaging you on teams.
Finally, click on ‘Done’ to save the changes.
```

#### Method 3: Use Third-Party Software or Tools There are several third-party tools that can help you keep your Teams status active. Here are a few suggestions from the community:
```
Caffeine: This is an app that keeps your computer from going idle, and thus keeps your Teams status active.
Mouse Jiggler: This is a device that you can buy which moves your mouse slightly every few seconds to keep your computer from going idle.
AutoHotKey: This is a scripting language for Windows that you can use to automate tasks on your computer. You could write a script that moves your mouse slightly every few minutes to keep your Teams status active.
```




## NextCloud

```
docker exec -it nextcloud bash
apt-get update
apt-get install smbclient -y
exit
docker restart nextcloud
dpkg --list|grep 'samba\|smb'

```

## Cloudflare tunnel need to be update.

Mobile app called WiseView

Go to “Main Menu” ; “Parameter” ; “Network” ; “RTSP”. Set User Name 
and Password to view video by PC software VLC
•	 RTSP Enable: Enable/Disable
•	 Verify: Enable/Disable
•	 RTSP Port: 554
•	 Instruction:rtsp: //IP:Port/chA/B
•	 A: 01(ch1), 02(ch2)...
•	 B: 0(main stream),1(sub stream)

VLC
Network Protol
Network URL
rtsp://192.168.1.22:554/ch01/0


https://support.hanwhavisionamerica.com/hc/en-us/articles/22959999056411-Using-VLC-to-view-RTSP-streams-from-Devices


#



# STEP1:
# nano /etc/network/interfaces

```
GNU nano 7.2                                                                                                                                                    
auto lo
iface lo inet loopback

iface enp0s25 inet manual

auto vmbr0
iface vmbr0 inet static                        <---------   Change it from DHCP to static
        address 192.168.1.241/24               <---------   Add this line
        gateway 192.168.1.1                    <---------   Add this line
        bridge-ports enp0s25
        bridge-stp off
        bridge-fd 0

iface wlp62s0 inet manual
source /etc/network/interfaces.d/*
```

# After making the changes save it by pressing the following keys

# Press CTRL O then Press ENTER KEY
# Press CTRL X
# Now type in
# reboot then Press ENTER KEY





