pi-mt7601
=========

The mt7601 driver for the raspberry pi + raspbian binaries (right now for the kernels I am using)

<h2>Source</h2>
The source for the driver is from ralink, I am only hosting it here. I have also applied a patch (not mine again) that enables it to be compiled on the 3.1+ kernels.
<br/>
For compile instructions (on a pi running raspbian - not cross compile) refer to the excellent guide in
http://groenholdt.net/Computers/RaspberryPi/MediaTek-MT7601-USB-WIFI-on-the-Raspberry-Pi/MediaTek-MT7601-USB-WIFI-on-the-Raspberry-Pi.html
<br/>

<h2>Binaries</h2>
To install the binaries
```
cp binaries/3.x.x/mt7601Usta.ko /lib/modules/3.x.x/kernel/drivers/net/wireless
mkdir -p /etc/Wireless/RT2870STA/
cp binaries/3.x.x/RT2870STA.dat /etc/Wireless/RT2870STA/
```
