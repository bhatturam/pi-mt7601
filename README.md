pi-mt7601
=========

The mt7601 driver for the raspberry pi + raspbian binaries (right now for the kernels I am using)

<h3>Binaries</h3>
To install the binaries
```
cp binaries/3.x.x/mt7601Usta.ko /lib/modules/3.x.x/kernel/drivers/net/wireless
mkdir -p /etc/Wireless/RT2870STA/
cp RT2870STA.dat /etc/Wireless/RT2870STA/
```

<h3>Compilation</h3>
The source for the driver is from ralink, I am only hosting it here. I have also applied a patch (not mine again) that enables it to be compiled on the 3.1+ and later kernels.
```
sudo apt-get install linux-headers-rpi
cd src/DPO_MT7601U_LinuxSTA_3.0.0.4_20130913/
make
sudo make install
mkdir -p /etc/Wireless/RT2870STA/
cp RT2870STA.dat /etc/Wireless/RT2870STA/
```
