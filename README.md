# toolkit
Random selection of things I found useful 
## index

1. [rpiLocaleFix](https://github.com/gntouts/toolkit/blob/master/README.md#rpilocalefixsh)
2. [RaspiCast](https://github.com/gntouts/toolkit/blob/master/README.md#raspicast)<br>
3. [Raspotify](https://github.com/gntouts/toolkit/blob/master/README.md#raspotify)<br>
4. [Headless AnyDesk Install](https://github.com/gntouts/toolkit/blob/master/README.md#headless-anydesk)
5. [Disable specific website in Chromium](https://github.com/gntouts/toolkit/blob/master/README.md#disable-website)

## rpiLocaleFix.sh

How to fix perl warning "setting locale failed" in Raspbian.

The warnings this script fixed for me:
```
perl: warning: Setting locale failed.
perl: warning: Please check that your locale settings:
LC_**="en_GB.UTF-8"
are supported and installed on your system.

perl: warning: Falling back to the standard locale ("C").
locale: Cannot set LC_**** to default locale: No such file or directory
```
#### **edit**: This problem occured while using SSH from another computer

This is a fault on the SSH client.

To fix this, edit /etc/ssh/ssh_config on the SSH client (your computer) and remove the line<br>
```
SendEnv LANG LC_*
```

Source: [bredman](https://www.raspberrypi.org/forums/viewtopic.php?f=50&t=11870)


## RaspiCast

Just follow the [article](https://thepi.io/how-to-use-your-raspberry-pi-as-a-chromecast-alternative/) and download the RaspiCast App for easy Youtube Playback.

## Raspotify

Use this awesome [Raspotify](https://github.com/dtcooper/raspotify) Client! <br>

Getting started: <br>
Open a terminal and install Raspotify with the following command:
```
curl -sL https://dtcooper.github.io/raspotify/install.sh | sh
```
<br> That's it, you will now discover your Raspberry as an available speaker.<br>
To change the name, or modify any other settings use:<br>
```
sudo nano /etc/default/raspotify
```

Restart Raspotify:

```
sudo systemctl restart raspotify
```

Enjoy your WiFi speaker and consider to donate to [dtcooper](https://github.com/dtcooper/raspotify#donations)!!!
<br>
## Headless AnyDesk
Connect to your RPi via SSH.<br>
```
ssh username@your.RPi.IP
```

Go to your Downloads folder and download AnyDesk for RPi via: 
```
wget https://download.anydesk.com/rpi/anydesk_2.9.4-1_armhf.deb?_ga=2.247598279.1909187070.1558275522-1898915190.1558275522
```
<br>Install AnyDesk and its dependencies with:
```
sudo dpkg -i anydesk_*.*.*-*_armhf.deb
sudo apt-get -f install
sudo dpkg -i anydesk_*.*.*-*_armhf.deb
```
Once the installation is complete, restart the SSH connection using:
```
exit
ssh -X username@your.RPi.IP
```
Start AnyDesk using:
```
anydesk
```
Enable unattended access, configure your password and change Interactive Access to Always Allow. 
<br>
Enjoy!
<br><br>
## Disable Website
We all hate a site or two. We hate finding it in our Google search results, we hate visiting it by mistake, we hate to be reminded that it exists. Thanks to Chrome extensions it is very easy to block that site completely.<br>
- **Step 1: Block the site in Google Search Results**
  - Install the [uBlacklist](https://chrome.google.com/webstore/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe "uBlacklist") extension.
  - Right-click the extension icon and go to **Options**. Add the URL pattern you want to block, for example:
  ```
  *://*.pinterest.com/*
  *://*pinterest.com/*
  ```
- **Step 2: Block the site in your Browser**
  - Install the [Block Site](https://chrome.google.com/webstore/detail/block-site-website-blocke/eiimnmioipafcokbfikbljfdeojpcgbh "Block Site - Website Blocker for Chrome™") extension.
  - Right-click the extension icon and go to **Options**. Click **Block by word** and add the wordpattern you want to block, for example:
  ```
  pinterest.c*
  ```
  
  That's it!
<br><br><br>
#### TODO<br>

-[https://devhints.io/bash](Bash Scripts Cheatsheet)
