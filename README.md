# toolkit
Random selection of things I found useful 
## index

1. [rpiLocaleFix](https://github.com/gntouts/toolkit/blob/master/README.md#rpilocalefixsh)
2. [RaspiCast](https://github.com/gntouts/toolkit/blob/master/README.md#raspicast)<br>
3. [Raspotify]((https://github.com/gntouts/toolkit/blob/master/README.md#raspotify)<br>

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
`SendEnv LANG LC_*`<br>
[source: bredman from RPi Forum](https://www.raspberrypi.org/forums/viewtopic.php?f=50&t=11870)



## RaspiCast

Just follow the [article](https://thepi.io/how-to-use-your-raspberry-pi-as-a-chromecast-alternative/) and download the RaspiCast App for easy Youtube Playback.

## Raspotify

Use this awesome [Raspotify](https://github.com/dtcooper/raspotify) Client! 
